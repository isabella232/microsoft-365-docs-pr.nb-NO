---
title: Overfør til Microsoft 365 Business fra Office 365 E3
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Lær hvordan du flytter virksomheten til Microsoft 365 Business Premium fra Office 365 E3.
ms.openlocfilehash: b8aa58f1f050ec6247479ed02e142507a2df45fc
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842164"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Overføre fra Office 365 E3 til Microsoft 365 Business Premium 

Microsoft 365 Business Premium har alt du trenger for å bruke små bedrifter til å kombinere de beste Sky BAS ert produktivitets appene med enkel enhets administrasjon og sikkerhet. Hvis du for øyeblikket har et Office 365-E3-abonnement, men ikke har mer enn 300 med arbeidere, kan du vurdere å bytte til Microsoft 365 Business Premium for å få nye sikkerhets funksjoner.

Det er enkelt å overføre: først bytter du lisenser, og alle dataene og bruker opplysningene i det gjeldende abonnementet beholdes. Etter overføringen må du konfigurere funksjonene som er lagt til i Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Forskjeller mellom Office 365 E3 og Microsoft 365 Business Premium

Denne tabellen viser forskjellene mellom Microsoft 365 Business Premium og Office 365 E3.

| Funksjon    | Støtte i Microsoft 365 Business Premium    | Støtte i Office 365 E3 | 
|:-------|:-----|:-----|
| **Lokalt**        | | | 
| Office-apper<sup>1</sup>    | Microsoft 365-apper for bedrifter    | Microsoft 365-apper for enterprise | 
| **Produktivitets programmer for skyen**        | | | 
| Exchange Online og Outlook    | lagrings grensen på 50 GB per post boks og ubegrenset Exchange Online-arkivering    | lagrings grensen på 100 GB per post boks og ubegrenset Exchange Online-arkivering | 
| Team    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png) | 
| OneDrive for Business    | 1 TB lagrings grense per bruker    | Uendelige | 
| Yammer, SharePoint Online, Planner, dataflyt    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png) | 
| StaffHub    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png) | 
| Outlook Customer Manager, MileIQ    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Trussel beskyttelse**        | | | 
| Defender for Office 365 plan 1 | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | Ikke inkludert, men kan legges til på | 
| **Identitets behandling**        | | | 
| Selv betjent tilbakestilling av passord for hybride Azure Active Directory-kontoer (Azure AD), Azure multi-Factor Authentication (MFA), betinget tilgang, passord bakgrunn for lokale identiteter|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| **Enhets-og app-behandling**        | | |
| Microsoft Intune, Windows autopilot|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| Aktivering av delt data maskin|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png)| 
| Oppgraderings rettigheter til Windows 10 Pro fra Win 7/8.1 Pro-lisenser|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    || 
| **Informasjons beskyttelse**        | | |
|Office 365 datatap-hindring|    ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)|![Inkludert i Office 365 E3](../media/check-mark.png)|
|Azure Information Protection Plan 1, BitLocker-håndhevelse|![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)||
|Azure Information Protection Plan 1, følsomhet-etiketter|![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)||
|**Klient adgangs lisens (CAL-rettigheter)**|||
|Enterprise CAL-programserie (Exchange, SharePoint, Skype)||![Inkludert i Office 365 E3](../media/check-mark.png)|

<sup>1</sup> Microsoft 365 Business Premium-versjonen av Office-appene omfatter ikke volum aktivering via gruppe policy, telemetribehandling for apper, oppdaterings kontroller, regne ark sammenligning og forespørsel eller forretnings intelligens.

## <a name="migration"></a>Medlemsserver

Hvis du vil overføre abonnementet, kan du se [endre planer manuelt](../commerce/subscriptions/change-plans-manually.md) hvis du vil flytte bare noen få personer til Microsoft 365 Business Premium. Du kan også [oppgradere alle automatisk](../commerce/subscriptions/upgrade-to-different-plan.md), eller arbeide med en partner for å flytte E3-abonnementet og-lisensene til et Microsoft 365 Business Premium-abonnement.
De følgende avsnittene beskriver endringene du trenger for å gjøre, og hva du kan gjøre etter overføringen.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Konfigurasjon og data for E3-abonnement for Office 365
Du trenger ikke å gjøre endringer i gjeldende abonnement eller data før du overfører, som omfatter følgende:

- Abonnements konfigurasjon, for eksempel DNS-poster og domene navn.
- Bruker-og gruppe kontoer og godkjennings innstillinger, for eksempel godkjenning for flere faktorer eller policyer for betinget tilgang.
- Produktivitets tjeneste konfigurasjoner og tilhørende data, for eksempel team, Exchange Online-postbokser, SharePoint Online-nettsteder, OneDrive for Business-mapper og OneNote-notatblokker.
- Office-programmer skalerer automatisk. Office 365 moderne lisensiering vil kontrollere brukerens lisens tilordning hver 72 timer, og vil konvertere Office-programmer til versjonen som Sams varer med bruker abonnementet.

### <a name="windows-10"></a>Windows 10

Hvis Windows ikke allerede er på Windows Pro Creator-oppdateringen, [oppgraderer du dem til Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Konfigurere policyer for å beskytte bruker enheter og filer

> [!NOTE]
> Hvis du konfigurerer Office 365 MDM-policyer og-enheter, vil disse enhetene være oppført på **enheter** -siden i administrasjons senteret for Microsoft 365. Policyer du konfigurerer, vises i listen over klassiske policyer i [Intune-portalen](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).

Når du har tilordnet lisenser til Microsoft 365 Business Premium, kan du begynne å beskytte brukernes enheter og filer.

Hvis du har oppgradert alle i organisasjonen til Microsoft 365 Business Premium, ser du konfigurasjons vei viseren på Starts IDen, og du kan følge [konfigureringen av Microsoft 365 Business Premium i vei viseren for konfigurasjon av installasjons programmet](set-up.md) for å beskytte filer og mobile enheter.

Du kan også fullføre disse trinnene på enheter-siden:
  
1. Gå til **enhets** policyer i den venstre ruten i administrasjons senteret \> **Policies**.
    
2. Velg **Legg til** på siden **enhets policyer** .
    
3. I **Legg til policy** -ruten gir du policyen et navn, og deretter velger du en **policy type** fra rulle gardin listen. 
    
     Du kan konfigurere program policyer for å beskytte filer på Android-og iPhone-enheter, i tillegg til Windows 10, og du kan konfigurere policyer for enhets konfigurasjon for firmaet som eier Windows 10-enheter. Se følgende koblinger for mer informasjon:
    
  - [Angi innstillinger for appbeskyttelse på Android- eller iOS-enheter](app-protection-settings-for-android-and-ios.md)
    
  - [Angi innstillinger for appbeskyttelse for Windows 10-enheter](protection-settings-for-windows-10-devices.md)
    
  - [Angi innstillinger for enhets beskyttelse for Windows 10-PC-er](protection-settings-for-windows-10-pcs.md)
  
4. Når du har konfigurert policyer, kan du og de ansatte konfigurere enheter:
    
  - Se [konfigurere Windows-enheter for Microsoft 365 Business Premium-brukere](set-up-windows-devices.md) for trinn for Windows-enheter. 
    
  - Se [konfigurere mobile enheter for Microsoft 365 Business Premium-brukere](set-up-mobile-devices.md) for trinn for Android-telefoner og-iPhone. 
  
### <a name="mailbox-size"></a>Post boks størrelse

Microsoft 365 Business Premium har en lagrings grense på 50 GB fordi den bruker Exchange Online plan 1. Når du overfører til Microsoft 365 Business Premium, anbefales det at du tilordner denne brukeren en Exchange Online-plan 2 og fjerner Exchange Online-planen 1 som det ikke er mulig å tilordne begge, hvis noen av brukerne overskrider 50 GB.


### <a name="threat-protection"></a>Trussel beskyttelse

Når du har overført til Microsoft 365 Business Premium, har du Defender for Office 365. Se [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for en oversikt. Hvis du vil konfigurere, kan du se [konfigurere sikre koblinger](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [konfigurere sikre vedlegg](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)og [konfigurere anti-phishing i Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).

### <a name="sensitivity-labels"></a>Følsomhetsetiketter

Hvis du vil begynne å bruke følsomhet etiketter, kan du se [Oversikt over følsomhet](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) og [opprette og behandle](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video om følsomhet-etiketter.
