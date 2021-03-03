---
title: Aktiver domenekøyde Windows 10-enheter som skal administreres av Microsoft 365 for bedrifter
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
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
description: Lær hvordan du aktiverer Microsoft 365 for å beskytte lokale Windows 10-enheter som er sammenføyd med Active Directory, med bare noen få trinn.
ms.openlocfilehash: 0b597110447272be128bfe1866234ac25a8e67e6
ms.sourcegitcommit: 070724118be25cd83418d2a56863da95582dae65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/03/2021
ms.locfileid: "50407082"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Aktiver domenekøyde Windows 10-enheter som skal administreres av Microsoft 365 Business Premium

Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business Premium til å beskytte Windows 10-enheter samtidig som du opprettholder tilgang til lokale ressurser som krever lokal godkjenning.
Hvis du vil konfigurere denne beskyttelsen, kan du implementere **hybridenheter som er med i Azure AD.** Disse enhetene er sammenføyd med både din lokale Active Directory og Azure Active Directory.

Denne videoen beskriver trinnene for hvordan du konfigurerer dette for det vanligste scenarioet, som også er beskrevet i fremgangsmåten nedenfor.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Før du begynner, må du passe på at du fullfører disse trinnene:
- Synkroniser brukere med Azure AD med Azure AD Connect.
- Fullfør synkronisering av Organisasjonsenhet for Azure AD Connect (OU).
- Kontroller at alle domenebrukerne du synkroniserer, har lisenser til Microsoft 365 Business Premium.

Se [fremgangsmåten for å synkronisere domenebrukere](manage-domain-users.md) til Microsoft.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Verifiser MDM-autoritet i Intune

Gå til [Endepunktbehandling,](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) og velg Enhetsregistrering på Microsoft Intune-siden. Kontroller deretter at  **MDM-autoritet** er Intune på **Oversikt-siden.** 

- Hvis **MDM-autoritet** er **Ingen,** klikker du **MDM-sertifiseringsinstansen** for å sette den til **Intune.**
- Hvis **MDM-autoritet** er Microsoft Office  **365,** går du til Enheter registrere enheter og bruker dialogboksen Legg til MDM-autoritet til høyre for å legge til  >   **Intune MDM-autoritet** (dialogboksen Legg til **MDM-autoritet** er bare tilgjengelig hvis **MDM-myndighetene** er satt til Microsoft Office 365). 

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Kontroller at Azure AD er aktivert for å koble sammen datamaskiner

- Gå til administrasjonssenteret på, og velg Azure Active Directory (velg Vis alt hvis Azure Active Directory ikke er synlig) i listen <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **over administrasjonssentre.**  
- Gå til **Azure Active Directory,** velg Enheter  og deretter **Enhetsinnstillinger** i administrasjonssenteret for Azure Active **Directory.**
- Kontroller **at brukere kan bli med i enheter med Azure AD** er aktivert 
    1. Hvis du vil aktivere alle brukere, setter du til **Alle.**
    2. Hvis du vil aktivere bestemte brukere, setter du **til Valgt** for å aktivere en bestemt gruppe med brukere.
        - Legg til de ønskede domenebrukerne som er synkronisert i Azure AD, i en [sikkerhetsgruppe.](../admin/create-groups/create-groups.md)
        - Velg **Velg grupper for** å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Kontroller at Azure AD er aktivert for MDM

- Gå til administrasjonssenteret på, <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  og velg **Endpoint Managemen** t **(velg Vis alt** hvis **Endepunktbehandling** ikke er synlig)
- Gå til Enheter med automatisk registrering for Windows-registrering i administrasjonssenteret for **Microsoft Endpoint**  >    >    >  **Manager.**
- Kontroller at brukeromfanget for MDM er aktivert.

    1. Hvis du vil registrere  alle datamaskinene, er satt til Alle til automatisk å registrere alle brukerdatamaskiner som er sammenføyd til Azure AD og nye datamaskiner, når brukerne legger til en jobbkonto i Windows.
    2. Sett til **Noen** for å registrere datamaskinene til en bestemt gruppe brukere.
        -  Legg til de ønskede domenebrukerne som er synkronisert i Azure AD, i en [sikkerhetsgruppe.](../admin/create-groups/create-groups.md)
        -  Velg **Velg grupper for** å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.

## <a name="4-create-the-required-resources"></a>4. Opprette de nødvendige ressursene 

De nødvendige oppgavene for å konfigurere hybrid Azure AD-sammenføyning er forenklet gjennom bruken av [Initialize-SecMgmtHybirdDeviceEnrollment-cmdleten](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) som finnes i [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell-modulen. [](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) Når du starter denne cmdleten, opprettes og konfigureres det nødvendige koblingspunktet og gruppepolicyen for tjenesten.

Du kan installere denne modulen ved å aktivere følgende fra en forekomst av PowerShell:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Det anbefales at du installerer denne modulen på Windows Server som kjører Azure AD Connect.

Hvis du vil opprette det nødvendige koblingspunktet og gruppepolicyen for tjenesten, starter du cmdleten [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) Du trenger legitimasjonen for global administrator for Microsoft 365 Business Premium når du utfører denne oppgaven. Når du er klar til å opprette ressursene, kan du aktivere følgende:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

Den første kommandoen oppretter en tilkobling til Microsoft-skyen, og når du blir bedt om det, angir du legitimasjonen for global administrator i Microsoft 365 Business Premium.

## <a name="5-link-the-group-policy"></a>5. Koble gruppepolicyen

1. Høyreklikk plasseringen der du vil koble policyen, i konsollen for gruppepolicybehandling (GPMC), og velg Koble et eksisterende *gruppepolicyobjekt...* fra hurtigmenyen.
2. Velg policyen som ble opprettet i trinnet ovenfor, og klikk deretter **ok.**

## <a name="get-the-latest-administrative-templates"></a>Få de nyeste administrative malene

Hvis du ikke ser policyen Aktivere automatisk **MDM-registrering** ved hjelp av standard Azure AD-legitimasjon, kan det være fordi du ikke har ADMX installert for Windows 10, versjon 1803 eller nyere. Følg disse trinnene for å løse problemet (Merk: den nyeste MDM.admx er bakoverkompatibel):

1.  Last ned: [Administrative maler (.admx) for Windows 10 oktober 2020 Update (20H2)](https://www.microsoft.com/download/102157).
2.  Installer pakken på en domenekontroller.
3.  Naviger, avhengig av administrative maler til mappen: **C:\Programfiler (x86)\Microsoft Gruppepolicy\Windows 10 Oktober 2020 Update (20H2)**.
4.  Gi nytt **navn til mappen Policydefinisjoner** i banen ovenfor til **PolicyDefinitions.**
5.  Kopier **PolicyDefinitions-mappen** til den delte SYSVOL-ressursen som standard på **C:\Windows\SYSVOL\domain\Policies.** 
    -   Hvis du har tenkt å bruke et sentralt policylager for hele domenet, legger du til innholdet i PolicyDefinitions der.
6.  I tilfelle du har flere domenekontrollere, venter du til SYSVOL replikerer til policyene er tilgjengelige. Denne fremgangsmåten fungerer også for alle fremtidige versjoner av de administrative malene.

På dette tidspunktet skal du kunne se policyen Aktivere automatisk MDM-registrering ved hjelp av standard **Azure AD-legitimasjon som er** tilgjengelig.
