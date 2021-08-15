---
title: Aktiver domene-sammenføyde Windows 10-enheter som skal administreres av Microsoft 365 for bedrifter
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
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
description: Lær hvordan du aktiverer Microsoft 365 å beskytte lokale Active-Directory-sammenføyde Windows 10 enheter med bare noen få trinn.
ms.openlocfilehash: 777a86313957920661e613f77afba3aaf4ea6292f252e445f308e3669de663d6
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53831411"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Aktiver domeneføyde Windows 10 enheter som skal administreres av Microsoft 365 Business Premium

Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business Premium til å beskytte Windows 10-enhetene, samtidig som du beholder tilgang til lokale ressurser som krever lokal godkjenning.
Hvis du vil konfigurere denne beskyttelsen, kan du implementere **Hybrid Azure AD-sammenføyde enheter.** Disse enhetene er koblet til både den lokale Active Directory og Azure Active Directory.

## <a name="watch-configure-hybrid-azure-active-directory-join"></a>Se: Konfigurere hybrid Azure Active Directory bli med

Denne videoen beskriver trinnene for hvordan du konfigurerer dette for det vanligste scenarioet, som også er beskrevet i fremgangsmåten nedenfor.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="before-you-begin"></a>Før du starter

- Synkroniser brukere med Azure AD med Azure AD Koble til.
- Fullfør Azure AD Koble til Organizational Unit (OU)-synkronisering.
- Kontroller at alle domenebrukerne du synkroniserer, har lisenser for å Microsoft 365 Business Premium.

Se [Synkronisere domenebrukere til Microsoft](manage-domain-users.md) for å se fremgangsmåten.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Bekreft MDM Authority i Intune

Gå til [Endpoint Manager,](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) og på Microsoft Intune velger du Enhetsregistrering **,** og  deretter kontrollerer du at **MDM-autoritet** er Intune på **Oversikt-siden.**

- Hvis **MDM-autoritet** **er Ingen,** klikker du **MDM-instansen** for å sette den til **Intune**.
- Hvis **MDM-autoritet** er **Microsoft Office 365,** går du til Enheter Registrere enheter og bruker dialogboksen Legg til MDM-autoritet til høyre for å legge til  >   **Intune MDM-autoritet** (dialogboksen Legg til **MDM-autoritet** er bare tilgjengelig hvis **MDM-myndigheten** er satt til  Microsoft Office 365).

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Kontroller at Azure AD er aktivert for sammenføyning av datamaskiner

- Gå til administrasjonssenteret på, og Azure Active Directory (velg Vis alle hvis Azure Active Directory ikke er synlig) i listen <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **over administrasjonssentre.**  
- I **administrasjonssenteret Azure Active Directory** går du **til Azure Active Directory** , **velger Enheter** og deretter **Enhetsinnstillinger**.
- Kontroller **at brukere kan bli med i enheter til Azure AD** er aktivert 
    1. Hvis du vil aktivere alle brukere, setter du til **Alle**.
    2. Hvis du vil aktivere bestemte brukere, setter du til **Valgt** for å aktivere en bestemt gruppe brukere.
        - Legg til de ønskede domenebrukerne synkronisert i Azure AD i en [sikkerhetsgruppe.](../admin/create-groups/create-groups.md)
        - Velg **Velg grupper for** å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Kontroller at Azure AD er aktivert for MDM

- Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> på, og velg  Endepunktadministrasjon t (velg Vis **alle hvis** Endpoint Manager ikke er synlig)
- Gå til **Windows** Windows registrering automatisk registrering i  >  **Microsoft Endpoint Manager**  >    >  **administrasjonssenteret**.
- Kontroller at MDM-brukeromfang er aktivert.

    1. Hvis du vil registrere  alle datamaskinene, setter du til Alle til å registrere automatisk alle brukerdatamaskiner som er sammenføyd med Azure AD og nye datamaskiner når brukerne legger til en jobbkonto Windows.
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
> Det anbefales at du installerer denne modulen på Windows server som kjører Azure AD Koble til.

Hvis du vil opprette det nødvendige tjenestetilkoblingspunktet og gruppepolicyen, starter du cmdleten [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Du trenger den Microsoft 365 Business Premium administratorlegitimasjon når du utfører denne oppgaven. Når du er klar til å opprette ressursene, kan du aktivere følgende:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

Den første kommandoen etablerer en tilkobling til Microsoft-skyen, og når du blir bedt om det, angir Microsoft 365 Business Premium den globale administratorlegitimasjonen.

## <a name="5-link-the-group-policy"></a>5. Koble gruppepolicyen

1. Høyreklikk plasseringen der du vil koble policyen, i konsollen for gruppepolicybehandling (GPMC), og velg Koble et eksisterende *gruppepolicyobjekt...* fra hurtigmenyen.
2. Velg policyen som ble opprettet i trinnet ovenfor, og klikk deretter **OK**.

## <a name="get-the-latest-administrative-templates"></a>Få de nyeste administrative malene

Hvis du ikke ser policyen Aktivere automatisk **MDM-registrering** ved hjelp av standard Azure AD-legitimasjon, kan det være fordi du ikke har ADMX installert for Windows 10, versjon 1803 eller nyere. Følg disse trinnene for å løse problemet (Merk: den nyeste MDM.admx er bakoverkompatibel):

1. Last ned: [Administrative maler (ADMX) for Windows 10 oktober 2020 Update (20H2)](https://www.microsoft.com/download/102157).
2. Installer pakken på en domenekontroller.
3. Naviger, avhengig av administrative maler-versjonen til mappen: **C:\Programfiler (x86)\Microsoft Gruppepolicy\Windows 10 oktober 2020 Update (20H2)**.
4. Gi nytt **navn til Policydefinisjoner-mappen** i banen ovenfor til **PolicyDefinitions**.
5. Kopier **PolicyDefinitions-mappen** til sysvol-ressursen som standard plassert på **C:\Windows\SYSVOL\domain\Policies**.
   - Hvis du planlegger å bruke et sentralt policylager for hele domenet, legger du til innholdet i PolicyDefinitions der.
6. Hvis du har flere domenekontrollere, venter du til SYSVOL replikerer for at policyene skal være tilgjengelige. Denne fremgangsmåten fungerer også for alle fremtidige versjoner av de administrative malene.

På dette tidspunktet skal du kunne se policyen Aktivere automatisk **MDM-registrering** ved hjelp av standard Azure AD-legitimasjon som er tilgjengelig.

## <a name="related-content"></a>Beslektet innhold

[Synkroniser domenebrukere Microsoft 365](manage-domain-users.md) (artikkel)\
[Opprette en gruppe i administrasjonssenteret](../admin/create-groups/create-groups.md) (artikkel)\
[Opplæring: Konfigurere hybrid Azure Active Directory for administrerte domener](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (artikkel)