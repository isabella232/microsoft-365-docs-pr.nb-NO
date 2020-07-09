---
title: Overføre til Microsoft 365 Business fra Office 365 E3
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
description: Finn ut hvordan du flytter bedriften til Microsoft 365 Business Premium fra Office 365 E3.
ms.openlocfilehash: d72f0c52a745ff973868b6fdaa95efa1a37a3dbd
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/18/2020
ms.locfileid: "45081882"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Overføre fra Office 365 E3 til Microsoft 365 Business Premium 

Microsoft 365 Business Premium har alt du trenger for småbedrifter, og kombinerer de best i klassen skybaserte produktivitetsapper med enkel enhetsadministrasjon og sikkerhet. Hvis du for øyeblikket har et Office 365 E3-abonnement, men ikke har mer enn 300 ansatte, kan du vurdere å bytte til Microsoft 365 Business Premium for ekstra sikkerhetsfunksjoner.

Det er enkelt å overføre: Først bytter du lisenser, og all data- og brukerinformasjon i det gjeldende abonnementet opprettholdes. Etter overføringen må du konfigurere funksjonene som er lagt til i Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Forskjeller mellom Office 365 E3 og Microsoft 365 Business Premium

Denne tabellen viser forskjellene mellom Microsoft 365 Business Premium og Office 365 E3.

| Funksjon    | Støtte i Microsoft 365 Business Premium    | Støtte i Office 365 E3 | 
|:-------|:-----|:-----|
| **Lokalt**        | | | 
| Office-apper<sup>1</sup>    | Microsoft 365-apper for bedrifter    | Microsoft 365-apper for bedrifter | 
| **Skyproduktivitetsapper**        | | | 
| Exchange Online og Outlook    | 50 GB lagringsgrense per postboks og ubegrenset Exchange Online-arkivering    | 100 GB lagringsgrense per postboks og ubegrenset Exchange Online-arkivering | 
| Lag    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Office 365 E3](../media/check-mark.png) | 
| OneDrive for Business    | 1 TB lagringsgrense per bruker    | Ubegrenset | 
| Yammer, SharePoint Online, Planlegger, Strøm    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Office 365 E3](../media/check-mark.png) | 
| AnsatteHub    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Office 365 E3](../media/check-mark.png) | 
| Kundeansvarlig for Outlook, MileIQ    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Beskyttelse mot trusler**        | | | 
| Office 365 Avansert trusselbeskyttelse (ATP)-plan 1 | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | Ikke inkludert, men kan legges til på | 
| **Identitetsadministrasjon**        | | | 
| Selvbetjent tilbakestilling av passord for hybride Azure Active Directory-kontoer (Azure AD), Azure multifaktorautentisering (MFA), Betinget tilgang, passordskriving for lokale identiteter|     ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| **Administrasjon av enheter og apper**        | | |
| Microsoft Intune, Windows AutoPilot|     ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| Aktivering av delt datamaskin|     ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Office 365 E3](../media/check-mark.png)| 
| Oppgrader rettigheter til Windows 10 Pro fra Win 7/8.1 Pro-lisenser|     ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    || 
| **Beskyttelse av informasjon**        | | |
|Forebygging av tap av data i Office 365|    ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)|![Følger med Office 365 E3](../media/check-mark.png)|
|Azure Information Protection Plan 1, Bitlocker-håndhevelse|![Følger med Microsoft 365 Business Premium](../media/check-mark.png)||
|Azure Information Protection Plan 1, Følsomhetsetiketter|![Følger med Microsoft 365 Business Premium](../media/check-mark.png)||
|**Klienttilgangslisens (CAL-rettigheter)**|||
|Enterprise CAL Suite (Exchange, SharePoint, Skype)||![Følger med Office 365 E3](../media/check-mark.png)|

<sup>1</sup> Microsoft 365 Business Premium-versjonen av Office-appene inkluderer ikke volumaktivering via gruppepolicy, apptelemetri, oppdateringskontroller, regnearksammenligning og forespørsel eller forretningsintelligens.

## <a name="migration"></a>Migrasjon

Hvis du vil overføre abonnementet, kan du se [Endre planer manuelt](../commerce/subscriptions/change-plans-manually.md) for instruksjoner hvis du vil flytte bare noen få personer til Microsoft 365 Business Premium. Du kan også [oppgradere alle automatisk](../commerce/subscriptions/upgrade-to-different-plan.md), eller arbeide med en partner for å flytte E3-abonnementet og lisensene til et Microsoft 365 Business Premium-abonnement.
Avsnittene nedenfor beskriver endringene du må gjøre, om noen, og hva du kan gjøre etter overføringen.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Konfigurasjon og data for Office 365 E3-abonnement
Du trenger ikke å gjøre endringer i gjeldende abonnement eller data før du overfører, som inkluderer:

- Abonnementskonfigurasjon, for eksempel DNS-poster og domenenavn.
- Bruker- og gruppekontoer og godkjenningsinnstillinger, for eksempel godkjenning med flere faktorer eller policyer for betinget tilgang.
- Produktivitetstjenestekonfigurasjoner og deres data, for eksempel Teams, Exchange Online-postbokser, SharePoint Online-områder, OneDrive for Business-mapper og OneNote-notatblokker.
- Office-programmer skaleres automatisk. Moderne lisensiering for Office 365 kontrollerer brukerens lisenstilordning hver 72.

### <a name="windows-10"></a>Windows 10

Hvis Windows ikke allerede er på Windows Pro Creator-oppdateringen, [kan du oppgradere dem til Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Konfigurere policyer for å beskytte brukerenheter og filer

> [!NOTE]
> Hvis du konfigurerer Office 365 MDM-policyer og -enheter, vises disse enhetene på **Enheter-siden** i administrasjonssenteret for Microsoft 365. Alle policyer du konfigurerer, vises i listen over klassiske policyer i [Intune-portalen](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).

Når du har tilordnet lisenser til Microsoft 365 Business Premium, kan du begynne å beskytte brukernes enheter og filer.

Hvis du oppgraderte alle i organisasjonen til Microsoft 365 Business Premium, ser du installasjonsveiviseren på Hjem-siden, og kan følge [trinnene Konfigurer Microsoft 365 Business Premium i installasjonsveiviseren](set-up.md) for å beskytte filer og mobile enheter.

Du kan også fullføre disse trinnene på Enheter-siden:
  
1. Gå til **Devices** \> **Enhetspolicyer**i navigasjonsenheten til venstre.
    
2. Velg **Legg til**på Siden **Enhetspolicyer.**
    
3. I ruten **Legg til policy** gir du policyen et navn, og deretter velger du en **policytype** fra rullegardinlisten. 
    
     Du kan konfigurere programpolicyer for å beskytte filer på Android- og iPhone-enheter, i tillegg til Windows 10, og du kan konfigurere enhetskonfigurasjonspolicyer for bedriftseide Windows 10-enheter. Se følgende koblinger for mer informasjon:
    
  - [Angi innstillinger for appbeskyttelse på Android- eller iOS-enheter](app-protection-settings-for-android-and-ios.md)
    
  - [Angi innstillinger for appbeskyttelse for Windows 10-enheter](protection-settings-for-windows-10-devices.md)
    
  - [Angi innstillinger for enhetsbeskyttelse for Windows 10-PCer](protection-settings-for-windows-10-pcs.md)
  
4. Når du har konfigurert policyer, kan du og de ansatte konfigurere enheter:
    
  - Se [Konfigurere Windows-enheter for Microsoft 365 Business Premium-brukere](set-up-windows-devices.md) for trinn for Windows-enheter. 
    
  - Se [Konfigurere mobile enheter for Microsoft 365 Business Premium-brukere](set-up-mobile-devices.md) for trinn for Android-telefoner og iPhoner. 

### <a name="threat-protection"></a>Beskyttelse mot trusler

Når du har overført til Microsoft 365 Business Premium, har du Office 365 ATP. Se [Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for en oversikt. Hvis du vil konfigurere, kan du se [konfigurere ATP-sikre koblinger](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [konfigurere ATP-sikre vedlegg](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)og konfigurere [ATP-anti-phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).

### <a name="sensitivity-labels"></a>Følsomhetsetiketter

Hvis du vil begynne å bruke følsomhetsetiketter, kan du se [Oversikt over følsomhetsetiketter](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) og [opprette og administrere følsomhetsetiketter](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.
