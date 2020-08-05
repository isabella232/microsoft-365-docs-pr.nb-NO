---
title: Aktivere domene-sammenføyde Windows 10-enheter som skal administreres av Microsoft 365 for bedrifter
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
description: Lær hvordan du aktiverer Microsoft 365 til å beskytte lokale Active-Directory-tilkoblede Windows 10-enheter med bare noen få trinn.
ms.openlocfilehash: 6275c6c4be9cd9631ab095f8b0e1b39683022bb2
ms.sourcegitcommit: d988faa292c2661ffea43c7161aef92b2b4b99bc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/04/2020
ms.locfileid: "46560847"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Aktivere domeneblede Windows 10-enheter som skal administreres av Microsoft 365 Business Premium

Hvis organisasjonen bruker lokal Windows Server Active Directory, kan du konfigurere Microsoft 365 Business Premium til å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgangen til lokale ressurser som krever lokal godkjenning.
Hvis du vil konfigurere denne beskyttelsen, kan du implementere **Hybrid Azure AD sammenføyde enheter**. Disse enhetene er koblet til både den lokale Active Directory og Azure Active Directory.

Denne videoen beskriver fremgangsmåten for hvordan du konfigurerer dette for det vanligste scenariet, som også er beskrevet i trinnene som følger.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Før du kommer i gang, må du sørge for at du fullfører disse trinnene:
- Synkroniser brukere til Azure AD med Azure AD Connect.
- Fullfør Azure AD Connect Organizational Unit (OU)-synkronisering.
- Kontroller at alle domenebrukerne du synkroniserer, har lisenser til Microsoft 365 Business Premium.

Se [Synkronisere domenebrukere til Microsoft](manage-domain-users.md) for fremgangsmåten.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Kontroller MDM-myndigheten i Intune

Gå til [Endpoint Manager,](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) og velg **Enhetsregistrering**på Siden Microsoft Intune , og kontroller deretter at **MDM-myndighet** er **Intune**på **Siden Oversikt.**

- Hvis **MDM-myndighet** er **Ingen**, klikker du **MDM-myndigheten** for å sette den til **Intune**.
- Hvis **MDM-myndighet** er **Microsoft Office 365**, går du til **Enheter**  >  **Registrer enheter** og bruker dialogboksen Legg til **MDM-myndighet** til høyre for å legge til **Intune MDM-myndighet** (dialogboksen **Legg til MDM Authority** er bare tilgjengelig hvis **MDM Authority** er satt til Microsoft Office 365).

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Kontroller at Azure AD er aktivert for sammenføyning av datamaskiner

- Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> på, og velg **Azure Active Directory** (velg Vis alle hvis Azure Active Directory ikke er synlig) i listen over **administrasjonssentre.** 
- Gå til **Azure Active Directory** i **administrasjonssenteret**for Azure Active Directory , velg **Enheter** og deretter **Enhetsinnstillinger**.
- Kontroller at**brukere kan koble enheter til Azure AD** er aktivert 
    1. Hvis du vil aktivere alle brukere, setter du til **Alle**.
    2. Hvis du vil aktivere bestemte brukere, setter du til **Valgt** for å aktivere en bestemt gruppe brukere.
        - Legg til de ønskede domenebrukerne som er synkronisert i Azure AD i en [sikkerhetsgruppe](../admin/create-groups/create-groups.md).
        - Velg **Velg grupper** for å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Kontroller at Azure AD er aktivert for MDM

- Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> på, og velg **Endepunktsbehandler**t (velg **Vis alt** hvis **Endpoint Manager** ikke er synlig)
- Gå til **Enheter**Automatisk registrering av Windows **Microsoft Endpoint Manager admin center**  >  **Windows**  >  **Windows-registrering**  >  **Automatic Enrollment**i administrasjonssenteret for Microsoft Endpoint Manager .
- Kontroller at MDM-brukeromfang er aktivert.

    1. Hvis du vil registrere alle datamaskiner, kan du sette til **Alle** for å registrere alle brukerdatamaskiner som er koblet til Azure AD og nye datamaskiner når brukerne legger til en arbeidskonto i Windows.
    2. Sett til **Noen** for å registrere datamaskinene til en bestemt gruppe brukere.
        -  Legg til de ønskede domenebrukerne som er synkronisert i Azure AD i en [sikkerhetsgruppe](../admin/create-groups/create-groups.md).
        -  Velg **Velg grupper** for å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.

## <a name="4-create-the-required-resources"></a>4. Opprett de nødvendige ressursene 

Utføre de nødvendige oppgavene for å [konfigurere hybrid Azure AD-sammenføyning](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) er forenklet ved bruk av cmdleten [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) som finnes i [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell-modulen. Når du starter denne cmdleten, opprettes og konfigurerer den nødvendige servicetilkoblingspunktet og gruppepolicyen.

Du kan installere denne modulen ved å påkalle følgende fra en forekomst av PowerShell:

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> Det anbefales at du installerer denne modulen på Windows Server som kjører Azure AD Connect.

Hvis du vil opprette den nødvendige tjenestetilkoblingspunktet og gruppepolicyen, vil du starte cmdleten [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) . Du trenger den globale administratorlegitimasjonen for Microsoft 365 Business Premium når du utfører denne oppgaven. Når du er klar til å opprette ressursene, starter du følgende:

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

Den første kommandoen oppretter en tilkobling til Microsoft-skyen, og når du blir bedt om det, angir du den globale administratorlegitimasjonen for Microsoft 365 Business Premium.

## <a name="5-link-the-group-policy"></a>5. Koble til gruppepolicyen

1. Høyreklikk plasseringen der du vil koble policyen i Group Policy Management Console (GPMC), og velg *Koble et eksisterende Gruppepolicyobjekt...* fra hurtigmenyen.
2. Velg policyen som er opprettet i trinnet ovenfor, og klikk deretter **OK**.

## <a name="get-the-latest-administrative-templates"></a>Få de nyeste administrative malene

Hvis du ikke ser policyen **Aktiver automatisk MDM-registrering ved hjelp av standard Azure AD-legitimasjon**, kan det skyldes at du ikke har ADMX installert for Windows 10, versjon 1803, versjon 1809 eller versjon 1903. Hvis du vil løse problemet, følger du denne fremgangsmåten (Merk: Den nyeste MDM.admx er bakoverkompatibel):

1.  Last ned: [Administrative maler (ADMX) for Windows 10 mai 2019 Oppdatering (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).
2.  Installere pakken på den primære domenekontrolleren (PDC).
3.  Naviger, avhengig av hvilken versjon til mappen: **C:\Programfiler (x86)\Microsoft gruppepolicy\Windows 10 Mai 2019 Oppdatering (1903) v3**.
4.  Gi nytt navn til **policydefinisjoner-mappen** i banen ovenfor til **PolicyDefinitions**.
5.  Kopier **PolicyDefinitions-mappen** til **C:\Windows\SYSVOL\domain\Policies**. 
    -   Hvis du planlegger å bruke et sentralt policylager for hele domenet, legger du til innholdet i PolicyDefinitions der.
6.  Start den primære domenekontrolleren på nytt for at policyen skal være tilgjengelig. Denne prosedyren vil fungere for alle fremtidige versjoner også.

På dette tidspunktet bør du kunne se policyen **Aktiver automatisk MDM-registrering ved hjelp av standard Azure AD-legitimasjon** tilgjengelig.
