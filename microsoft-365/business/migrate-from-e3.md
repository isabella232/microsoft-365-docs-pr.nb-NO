---
title: Overføre til Microsoft 365 Business fra Office 365 E3
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
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
description: Lær hvordan du flytter bedriften til Microsoft 365 Business Premium fra Office 365 E3.
ms.openlocfilehash: f08b054473fdd63ec2372e81c776a1b64f89fe9d
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/06/2021
ms.locfileid: "52244840"
---
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a>Overføre fra Office 365 E3 til Microsoft 365 Business Premium

Microsoft 365 Business Premium har alt du trenger for småbedrifter, og kombinerer de beste skybaserte produktivitetsappene med enkel enhetsadministrasjon og sikkerhet. Hvis du for øyeblikket har et Office 365 E3-abonnement, men ikke har mer enn 300 ansatte, kan du vurdere å bytte til Microsoft 365 Business Premium for ekstra sikkerhetsfunksjoner.

Overføring er enkelt: Først bytter du lisenser, og all data og brukerinformasjon i det gjeldende abonnementet vedlikeholdes. Etter overføringen må du konfigurere funksjonene som er lagt til i Microsoft 365 Business Premium.

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a>Forskjeller mellom Office 365 E3 og Microsoft 365 Business Premium

Denne tabellen viser forskjellene mellom Microsoft 365 Business Premium og Office 365 E3.

| Funksjon    | Støtte i Microsoft 365 Business Premium    | Støtte i Office 365 E3 | 
|:-------|:-----|:-----|
| **Lokalt**        | | | 
| Office apper<sup>1</sup>    | Microsoft 365 Apps for business    | Microsoft 365-apper for enterprise | 
| **Skyproduktivitetsapper**        | | | 
| Exchange Online og Outlook    | Lagringsgrense på 50 GB per postboks og ubegrenset Exchange Online Archiving    | 100 GB lagringsgrense per postboks og ubegrenset Exchange Online Archiving | 
| Team    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png) | 
| OneDrive for Business    | 1 TB lagringsgrense per bruker    | Ubegrenset | 
| Yammer, SharePoint Online, Planner, Stream    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png) | 
| StaffHub    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png) | 
| MileIQ    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Trusselbeskyttelse**        | | | 
| Defender for Office 365 Plan 1 | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | Ikke inkludert, men kan legges til på | 
| **Identitetsbehandling**        | | | 
| Selvbetjent tilbakestilling av passord for hybride Azure Active Directory (Azure AD)-kontoer, Azure AD-godkjenning med flere faktorer (MFA), betinget tilgang, tilbakeskriving av passord for lokale identiteter|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| **Enhets- og appbehandling**        | | |
| Microsoft Intune, Windows AutoPilot|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| Aktivering av delt datamaskin|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png)| 
| Oppgradere rettigheter til Windows 10 Pro fra Win 7/8.1 Pro lisenser|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    || 
| **Informasjonsbeskyttelse**        | | |
|Office 365 Hindring av datatap|    ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)|![Inkludert i Office 365 E3](../media/check-mark.png)|
|Azure Information Protection Plan 1, BitLocker håndhevelse|![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)||
|Azure Information Protection Plan 1, Følsomhetsetiketter|![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)||
|**Klienttilgangslisens (CAL-rettigheter)**|||
|Enterprise CAL Suite (Exchange, SharePoint, Skype)||![Inkludert i Office 365 E3](../media/check-mark.png)|

<sup>1</sup> Microsoft 365 Business Premium-versjonen av Office-appene inkluderer ikke volumaktivering gjennom gruppepolicy, apptemetri, oppdateringskontroller, regnearksammenligning og spørring eller forretningsintelligens.

## <a name="migration"></a>Overføring

Hvis du vil overføre abonnementet, kan du se Endre [abonnementer](../commerce/subscriptions/change-plans-manually.md) manuelt for instruksjoner hvis du vil flytte bare noen få personer til Microsoft 365 Business Premium. Du kan også [oppgradere alle automatisk](../commerce/subscriptions/upgrade-to-different-plan.md), eller samarbeide med en partner for å flytte E3-abonnementet og lisensene til et Microsoft 365 Business Premium abonnement.
Avsnittene nedenfor beskriver eventuelle endringer du må gjøre, og hva du kan gjøre etter overføringen.

### <a name="office-365-e3-subscription-configuration-and-data"></a>Office 365 Konfigurasjon og data for E3-abonnement
Du trenger ikke å gjøre noen endringer i det gjeldende abonnementet eller dataene før du overfører, som omfatter:

- Abonnementskonfigurasjon, for eksempel DNS-poster og domenenavn.
- Bruker- og gruppekontoer og godkjenningsinnstillinger, for eksempel godkjenning med flere faktorer eller policyer for betinget tilgang.
- Produktivitetstjenestekonfigurasjoner og deres data, for eksempel Teams, Exchange Online postbokser, SharePoint Nettsteder, OneDrive for Business mapper og OneNote notatblokker.
- Office programmer skaleres automatisk. Office 365 moderne lisensiering kontrollerer brukerens lisenstilordning hver 72. time og konverterer Office programmer til versjonen som samsvarer med brukerabonnementet.

### <a name="windows-10"></a>Windows 10

Hvis Windows ikke allerede er på Windows Pro Creator-oppdateringen, kan du oppgradere dem til Windows Pro [Creators Update](upgrade-to-windows-pro-creators-update.md).

### <a name="set-up-policies-to-protect-user-devices-and-files"></a>Konfigurere policyer for å beskytte brukerenheter og filer

> [!NOTE]
> Hvis du konfigurerer Office 365 MDM-policyer og -enheter, vises  disse enhetene på Enheter-siden i Microsoft 365 administrasjonssenteret. Eventuelle policyer du konfigurerer, vises i listen over klassiske policyer i [Intune-portalen.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)

Når du har tilordnet lisenser til Microsoft 365 Business Premium, kan du begynne å beskytte brukernes enheter og filer.

Hvis du oppgraderte alle i organisasjonen til Microsoft 365 Business Premium, ser du installasjonsveiviseren på hjemmesiden, og du kan følge fremgangsmåten konfigurer [Microsoft 365 Business Premium](set-up.md) i konfigurasjonsveiviseren for å beskytte filer og mobile enheter.

Du kan også fullføre disse trinnene på Enheter-siden:
  
1. Gå til Policyer for enheter i det venstre navigasjonsfeltet i **administrasjonssenteret.** \> 
    
2. Velg Legg **til på siden Enhetspolicyer.** 
    
3. Gi **policyen et** navn i legg til policy-ruten, og velg deretter en **policytype** fra rullegardinlisten. 
    
     Du kan konfigurere programpolicyer for å beskytte filer på Android- og iPhone-enheter samt Windows 10, og du kan konfigurere policyer for enhetskonfigurasjon for firmaeide Windows 10 enheter. Se følgende koblinger for mer informasjon:
    
  - [Angi innstillinger for appbeskyttelse på Android- eller iOS-enheter](app-protection-settings-for-android-and-ios.md)
    
  - [Angi innstillinger for appbeskyttelse for Windows 10-enheter](protection-settings-for-windows-10-devices.md)
    
  - [Angi innstillinger for enhetsbeskyttelse for Windows 10 PC-er](protection-settings-for-windows-10-pcs.md)
  
4. Når du har konfigurert policyer, kan du og de ansatte konfigurere enheter:
    
  - Se [Konfigurere Windows for Microsoft 365 Business Premium for](set-up-windows-devices.md) trinn for Windows enheter. 
    
  - Se [Konfigurere mobile enheter for Microsoft 365 Business Premium for](set-up-mobile-devices.md) trinn for Android-telefoner og iPhone. 
  
### <a name="mailbox-size"></a>Postboksstørrelse

Microsoft 365 Business Premium har en lagringsgrense på 50 GB, da den bruker Exchange Online Plan 1. Når du overfører til Microsoft 365 Business Premium, anbefales det at du tilordner denne brukeren en Exchange Online Plan 2 og fjerner Exchange Online Plan 1 fordi det ikke er mulig å tilordne begge.


### <a name="threat-protection"></a>Trusselbeskyttelse

Etter at du har Microsoft 365 Business Premium, har du Defender for Office 365. Se [Microsoft Defender for Office 365](../security/office-365-security/defender-for-office-365.md) for en oversikt. Hvis du vil konfigurere dette, [kan](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)du se Konfigurere klarerte koblinger, konfigurere [klarerte](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)vedlegg og konfigurere [Phishing-phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)i Defender for Office 365 .

### <a name="sensitivity-labels"></a>Følsomhetsetiketter

Hvis du vil begynne å bruke følsomhetsetiketter, kan du se [Oversikt over følsomhetsetiketter](../compliance/sensitivity-labels.md) [og opprette og behandle følsomhetsetiketter.](../business-video/create-sensitivity-labels.md)
