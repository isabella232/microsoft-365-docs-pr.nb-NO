---
title: Aktiver domenekretserte Windows 10-enheter som skal administreres av Microsoft 365 for bedrifter
f1.keywords:
- CSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Lær hvordan du aktiverer Microsoft 365 for å beskytte lokale Active-Directory-sammenføyde Windows 10-enheter med bare noen få trinn.
ms.openlocfilehash: c9f5a21d993200abcf9ecf1fa236879245e1c153
ms.sourcegitcommit: 4076b43a4b661de029f6307ddc1a989ab3108edb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2021
ms.locfileid: "51939506"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Aktiver domenekretserte Windows 10-enheter som skal administreres av Microsoft 365 Business Premium

Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business Premium til å beskytte Windows 10-enhetene dine, samtidig som du beholder tilgang til lokale ressurser som krever lokal godkjenning.
Hvis du vil konfigurere denne beskyttelsen, kan du implementere **Hybrid Azure AD-sammenføyde enheter.** Disse enhetene er koblet til både den lokale Active Directory og Azure Active Directory.

Denne videoen beskriver trinnene for hvordan du konfigurerer dette for det vanligste scenarioet, som også er beskrevet i fremgangsmåten nedenfor.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Før du kommer i gang, må du passe på at du fullfører disse trinnene:
- Synkroniser brukere med Azure AD med Azure AD Connect.
- Fullfør Synkronisering av Organisasjonsenhet for Azure AD Connect (OU).
- Kontroller at alle domenebrukerne du synkroniserer, har lisenser til Microsoft 365 Business Premium.

Se [Synkronisere domenebrukere til Microsoft](manage-domain-users.md) for å se fremgangsmåten.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Bekreft MDM Authority i Intune

Gå til [Endepunktbehandling,](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) og velg Enhetsregistrering på Microsoft Intune-siden, og kontroller deretter at  **MDM-instansen** er Intune på Oversikt-siden. 

- Hvis **MDM-autoritet** **er Ingen,** klikker du **MDM-instansen** for å sette den til **Intune**.
- Hvis **MDM-myndighet** er **Microsoft Office 365,** går du til Enheter Registrere enheter og bruker dialogboksen Legg til MDM-autoritet til høyre for å legge   >   til **Intune MDM-autoritet** (dialogboksen Legg til MDM-autoritet er bare tilgjengelig hvis  **MDM-myndigheten** er angitt til Microsoft Office 365). 

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Kontroller at Azure AD er aktivert for sammenføyning av datamaskiner

- Gå til administrasjonssenteret på, og velg Azure Active Directory (velg Vis alle hvis Azure Active Directory ikke er synlig) i listen <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **over administrasjonssentre.**  
- Gå til **Azure Active Directory** i administrasjonssenteret for Azure **Active Directory,** velg **Enheter** og deretter **Enhetsinnstillinger**.
- Kontroller **at brukere kan bli med i enheter til Azure AD** er aktivert 
    1. Hvis du vil aktivere alle brukere, setter du til **Alle**.
    2. Hvis du vil aktivere bestemte brukere, setter du til **Valgt** for å aktivere en bestemt gruppe brukere.
        - Legg til de ønskede domenebrukerne synkronisert i Azure AD i en [sikkerhetsgruppe.](../admin/create-groups/create-groups.md)
        - Velg **Velg grupper for** å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Kontroller at Azure AD er aktivert for MDM

- Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  på, og velg **Endepunktbehandling** t (velg **Vis alle** hvis **Endepunktbehandling** ikke er synlig)
- Gå til Enheter    >    >  **Windows-registrering**  >  automatisk registrering i administrasjonssenteret for Microsoft Endpoint Manager .
- Kontroller at MDM-brukeromfang er aktivert.

    1. Hvis du vil registrere  alle datamaskinene, setter du til Alle til å registrere automatisk alle brukerdatamaskiner som er sammenføyd med Azure AD og nye datamaskiner når brukerne legger til en jobbkonto i Windows.
    2. Sett til **Noen for** å registrere datamaskinene til en bestemt gruppe brukere.
        -  Legg til de ønskede domenebrukerne synkronisert i Azure AD i en [sikkerhetsgruppe.](../admin/create-groups/create-groups.md)
        -  Velg **Velg grupper for** å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.

## <a name="4-create-the-required-resources"></a>4. Opprett de nødvendige ressursene 

Utføring av de nødvendige oppgavene for å konfigurere hybrid Azure AD-sammenføyning har blitt forenklet ved bruk av cmdleten [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) som ble funnet i [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell-modulen. [](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) Når du starter denne cmdleten, opprettes og konfigureres det nødvendige koblingspunktet og gruppepolicyen for tjenesten.

Du kan installere denne modulen ved å aktivere følgende fra en forekomst av PowerShell:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Det anbefales at du installerer denne modulen på Windows Server som kjører Azure AD Connect.

Hvis du vil opprette det nødvendige tjenestetilkoblingspunktet og gruppepolicyen, starter du cmdleten [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Du trenger den globale administratorlegitimasjonen for Microsoft 365 Business Premium når du utfører denne oppgaven. Når du er klar til å opprette ressursene, kan du aktivere følgende:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

Den første kommandoen oppretter en tilkobling til Microsoft-skyen, og når du blir bedt om det, angir du den globale administratorlegitimasjonen for Microsoft 365 Business Premium.

## <a name="5-link-the-group-policy"></a>5. Koble gruppepolicyen

1. Høyreklikk plasseringen der du vil koble policyen, i konsollen for gruppepolicybehandling (GPMC), og velg Koble et eksisterende *gruppepolicyobjekt...* fra hurtigmenyen.
2. Velg policyen som ble opprettet i trinnet ovenfor, og klikk deretter **OK**.

## <a name="get-the-latest-administrative-templates"></a>Få de nyeste administrative malene

Hvis du ikke ser policyen Aktivere automatisk **MDM-registrering** ved hjelp av standard Azure AD-legitimasjon, kan det være fordi du ikke har ADMX installert for Windows 10, versjon 1803 eller nyere. Følg disse trinnene for å løse problemet (Merk: den nyeste MDM.admx er bakoverkompatibel):

1.  Last ned: [Administrative maler (ADMX) for Windows 10 Oktober 2020 Update (20H2)](https://www.microsoft.com/download/102157).
2.  Installer pakken på en domenekontroller.
3.  Naviger, avhengig av administrative maler-versjonen til mappen: **C:\Programfiler (x86)\Microsoft Gruppepolicy\Windows 10 Oktober 2020 Update (20H2)**.
4.  Gi nytt **navn til Policydefinisjoner-mappen** i banen ovenfor til **PolicyDefinitions**.
5.  Kopier **PolicyDefinitions-mappen** til sysvol-ressursen som standard plassert på **C:\Windows\SYSVOL\domain\Policies**. 
    -   Hvis du planlegger å bruke et sentralt policylager for hele domenet, legger du til innholdet i PolicyDefinitions der.
6.  Hvis du har flere domenekontrollere, venter du til SYSVOL replikerer for at policyene skal være tilgjengelige. Denne fremgangsmåten fungerer også for alle fremtidige versjoner av de administrative malene.

På dette tidspunktet skal du kunne se policyen Aktivere automatisk **MDM-registrering** ved hjelp av standard Azure AD-legitimasjon som er tilgjengelig.

## <a name="related-content"></a>Relatert innhold

[Synkronisere domenebrukere til Microsoft 365](manage-domain-users.md) [(artikkel)](../admin/create-groups/create-groups.md) Opprette en gruppe i administrasjonssenteret (artikkel) Opplæring: Konfigurere hybrid Azure Active Directory-sammenføyning for administrerte [domener](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (artikkel)