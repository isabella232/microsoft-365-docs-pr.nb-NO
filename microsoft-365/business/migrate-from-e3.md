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
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="31de9-103">Overføre fra Office 365 E3 til Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="31de9-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span>

<span data-ttu-id="31de9-104">Microsoft 365 Business Premium har alt du trenger for småbedrifter, og kombinerer de beste skybaserte produktivitetsappene med enkel enhetsadministrasjon og sikkerhet.</span><span class="sxs-lookup"><span data-stu-id="31de9-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="31de9-105">Hvis du for øyeblikket har et Office 365 E3-abonnement, men ikke har mer enn 300 ansatte, kan du vurdere å bytte til Microsoft 365 Business Premium for ekstra sikkerhetsfunksjoner.</span><span class="sxs-lookup"><span data-stu-id="31de9-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="31de9-106">Overføring er enkelt: Først bytter du lisenser, og all data og brukerinformasjon i det gjeldende abonnementet vedlikeholdes.</span><span class="sxs-lookup"><span data-stu-id="31de9-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="31de9-107">Etter overføringen må du konfigurere funksjonene som er lagt til i Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="31de9-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="31de9-108">Forskjeller mellom Office 365 E3 og Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="31de9-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="31de9-109">Denne tabellen viser forskjellene mellom Microsoft 365 Business Premium og Office 365 E3.</span><span class="sxs-lookup"><span data-stu-id="31de9-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="31de9-110">Funksjon</span><span class="sxs-lookup"><span data-stu-id="31de9-110">Feature</span></span>    | <span data-ttu-id="31de9-111">Støtte i Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="31de9-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="31de9-112">Støtte i Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="31de9-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="31de9-113">**Lokalt**</span><span class="sxs-lookup"><span data-stu-id="31de9-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="31de9-114">Office apper<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="31de9-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="31de9-115">Microsoft 365 Apps for business</span><span class="sxs-lookup"><span data-stu-id="31de9-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="31de9-116">Microsoft 365-apper for enterprise</span><span class="sxs-lookup"><span data-stu-id="31de9-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="31de9-117">**Skyproduktivitetsapper**</span><span class="sxs-lookup"><span data-stu-id="31de9-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="31de9-118">Exchange Online og Outlook</span><span class="sxs-lookup"><span data-stu-id="31de9-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="31de9-119">Lagringsgrense på 50 GB per postboks og ubegrenset Exchange Online Archiving</span><span class="sxs-lookup"><span data-stu-id="31de9-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="31de9-120">100 GB lagringsgrense per postboks og ubegrenset Exchange Online Archiving</span><span class="sxs-lookup"><span data-stu-id="31de9-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="31de9-121">Team</span><span class="sxs-lookup"><span data-stu-id="31de9-121">Teams</span></span>    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="31de9-124">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="31de9-124">OneDrive for Business</span></span>    | <span data-ttu-id="31de9-125">1 TB lagringsgrense per bruker</span><span class="sxs-lookup"><span data-stu-id="31de9-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="31de9-126">Ubegrenset</span><span class="sxs-lookup"><span data-stu-id="31de9-126">Unlimited</span></span> | 
| <span data-ttu-id="31de9-127">Yammer, SharePoint Online, Planner, Stream</span><span class="sxs-lookup"><span data-stu-id="31de9-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="31de9-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="31de9-130">StaffHub</span></span>    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="31de9-133">MileIQ</span><span class="sxs-lookup"><span data-stu-id="31de9-133">MileIQ</span></span>    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="31de9-135">**Trusselbeskyttelse**</span><span class="sxs-lookup"><span data-stu-id="31de9-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="31de9-136">Defender for Office 365 Plan 1</span><span class="sxs-lookup"><span data-stu-id="31de9-136">Defender for Office 365 Plan 1</span></span> | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="31de9-138">Ikke inkludert, men kan legges til på</span><span class="sxs-lookup"><span data-stu-id="31de9-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="31de9-139">**Identitetsbehandling**</span><span class="sxs-lookup"><span data-stu-id="31de9-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="31de9-140">Selvbetjent tilbakestilling av passord for hybride Azure Active Directory (Azure AD)-kontoer, Azure AD-godkjenning med flere faktorer (MFA), betinget tilgang, tilbakeskriving av passord for lokale identiteter</span><span class="sxs-lookup"><span data-stu-id="31de9-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure AD multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| <span data-ttu-id="31de9-142">**Enhets- og appbehandling**</span><span class="sxs-lookup"><span data-stu-id="31de9-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="31de9-143">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="31de9-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="31de9-145">Aktivering av delt datamaskin</span><span class="sxs-lookup"><span data-stu-id="31de9-145">Shared computer activation</span></span>|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png)| 
| <span data-ttu-id="31de9-148">Oppgradere rettigheter til Windows 10 Pro fra Win 7/8.1 Pro lisenser</span><span class="sxs-lookup"><span data-stu-id="31de9-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    || 
| <span data-ttu-id="31de9-150">**Informasjonsbeskyttelse**</span><span class="sxs-lookup"><span data-stu-id="31de9-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="31de9-151">Office 365 Hindring av datatap</span><span class="sxs-lookup"><span data-stu-id="31de9-151">Office 365 Data Loss Prevention</span></span>|    ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)|![Inkludert i Office 365 E3](../media/check-mark.png)|
|<span data-ttu-id="31de9-154">Azure Information Protection Plan 1, BitLocker håndhevelse</span><span class="sxs-lookup"><span data-stu-id="31de9-154">Azure Information Protection Plan 1, BitLocker enforcement</span></span>|![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="31de9-156">Azure Information Protection Plan 1, Følsomhetsetiketter</span><span class="sxs-lookup"><span data-stu-id="31de9-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="31de9-158">**Klienttilgangslisens (CAL-rettigheter)**</span><span class="sxs-lookup"><span data-stu-id="31de9-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="31de9-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="31de9-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Inkludert i Office 365 E3](../media/check-mark.png)|

<span data-ttu-id="31de9-161"><sup>1</sup> Microsoft 365 Business Premium-versjonen av Office-appene inkluderer ikke volumaktivering gjennom gruppepolicy, apptemetri, oppdateringskontroller, regnearksammenligning og spørring eller forretningsintelligens.</span><span class="sxs-lookup"><span data-stu-id="31de9-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="31de9-162">Overføring</span><span class="sxs-lookup"><span data-stu-id="31de9-162">Migration</span></span>

<span data-ttu-id="31de9-163">Hvis du vil overføre abonnementet, kan du se Endre [abonnementer](../commerce/subscriptions/change-plans-manually.md) manuelt for instruksjoner hvis du vil flytte bare noen få personer til Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="31de9-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="31de9-164">Du kan også [oppgradere alle automatisk](../commerce/subscriptions/upgrade-to-different-plan.md), eller samarbeide med en partner for å flytte E3-abonnementet og lisensene til et Microsoft 365 Business Premium abonnement.</span><span class="sxs-lookup"><span data-stu-id="31de9-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="31de9-165">Avsnittene nedenfor beskriver eventuelle endringer du må gjøre, og hva du kan gjøre etter overføringen.</span><span class="sxs-lookup"><span data-stu-id="31de9-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="31de9-166">Office 365 Konfigurasjon og data for E3-abonnement</span><span class="sxs-lookup"><span data-stu-id="31de9-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="31de9-167">Du trenger ikke å gjøre noen endringer i det gjeldende abonnementet eller dataene før du overfører, som omfatter:</span><span class="sxs-lookup"><span data-stu-id="31de9-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="31de9-168">Abonnementskonfigurasjon, for eksempel DNS-poster og domenenavn.</span><span class="sxs-lookup"><span data-stu-id="31de9-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="31de9-169">Bruker- og gruppekontoer og godkjenningsinnstillinger, for eksempel godkjenning med flere faktorer eller policyer for betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="31de9-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="31de9-170">Produktivitetstjenestekonfigurasjoner og deres data, for eksempel Teams, Exchange Online postbokser, SharePoint Nettsteder, OneDrive for Business mapper og OneNote notatblokker.</span><span class="sxs-lookup"><span data-stu-id="31de9-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="31de9-171">Office programmer skaleres automatisk.</span><span class="sxs-lookup"><span data-stu-id="31de9-171">Office applications will scale automatically.</span></span> <span data-ttu-id="31de9-172">Office 365 moderne lisensiering kontrollerer brukerens lisenstilordning hver 72. time og konverterer Office programmer til versjonen som samsvarer med brukerabonnementet.</span><span class="sxs-lookup"><span data-stu-id="31de9-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="31de9-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="31de9-173">Windows 10</span></span>

<span data-ttu-id="31de9-174">Hvis Windows ikke allerede er på Windows Pro Creator-oppdateringen, kan du oppgradere dem til Windows Pro [Creators Update](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="31de9-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="31de9-175">Konfigurere policyer for å beskytte brukerenheter og filer</span><span class="sxs-lookup"><span data-stu-id="31de9-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="31de9-176">Hvis du konfigurerer Office 365 MDM-policyer og -enheter, vises  disse enhetene på Enheter-siden i Microsoft 365 administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="31de9-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="31de9-177">Eventuelle policyer du konfigurerer, vises i listen over klassiske policyer i [Intune-portalen.](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview)</span><span class="sxs-lookup"><span data-stu-id="31de9-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="31de9-178">Når du har tilordnet lisenser til Microsoft 365 Business Premium, kan du begynne å beskytte brukernes enheter og filer.</span><span class="sxs-lookup"><span data-stu-id="31de9-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="31de9-179">Hvis du oppgraderte alle i organisasjonen til Microsoft 365 Business Premium, ser du installasjonsveiviseren på hjemmesiden, og du kan følge fremgangsmåten konfigurer [Microsoft 365 Business Premium](set-up.md) i konfigurasjonsveiviseren for å beskytte filer og mobile enheter.</span><span class="sxs-lookup"><span data-stu-id="31de9-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="31de9-180">Du kan også fullføre disse trinnene på Enheter-siden:</span><span class="sxs-lookup"><span data-stu-id="31de9-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="31de9-181">Gå til Policyer for enheter i det venstre navigasjonsfeltet i **administrasjonssenteret.** \> </span><span class="sxs-lookup"><span data-stu-id="31de9-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="31de9-182">Velg Legg **til på siden Enhetspolicyer.** </span><span class="sxs-lookup"><span data-stu-id="31de9-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="31de9-183">Gi **policyen et** navn i legg til policy-ruten, og velg deretter en **policytype** fra rullegardinlisten.</span><span class="sxs-lookup"><span data-stu-id="31de9-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="31de9-184">Du kan konfigurere programpolicyer for å beskytte filer på Android- og iPhone-enheter samt Windows 10, og du kan konfigurere policyer for enhetskonfigurasjon for firmaeide Windows 10 enheter.</span><span class="sxs-lookup"><span data-stu-id="31de9-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="31de9-185">Se følgende koblinger for mer informasjon:</span><span class="sxs-lookup"><span data-stu-id="31de9-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="31de9-186">Angi innstillinger for appbeskyttelse på Android- eller iOS-enheter</span><span class="sxs-lookup"><span data-stu-id="31de9-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="31de9-187">Angi innstillinger for appbeskyttelse for Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="31de9-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="31de9-188">Angi innstillinger for enhetsbeskyttelse for Windows 10 PC-er</span><span class="sxs-lookup"><span data-stu-id="31de9-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="31de9-189">Når du har konfigurert policyer, kan du og de ansatte konfigurere enheter:</span><span class="sxs-lookup"><span data-stu-id="31de9-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="31de9-190">Se [Konfigurere Windows for Microsoft 365 Business Premium for](set-up-windows-devices.md) trinn for Windows enheter.</span><span class="sxs-lookup"><span data-stu-id="31de9-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="31de9-191">Se [Konfigurere mobile enheter for Microsoft 365 Business Premium for](set-up-mobile-devices.md) trinn for Android-telefoner og iPhone.</span><span class="sxs-lookup"><span data-stu-id="31de9-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="31de9-192">Postboksstørrelse</span><span class="sxs-lookup"><span data-stu-id="31de9-192">Mailbox Size</span></span>

<span data-ttu-id="31de9-193">Microsoft 365 Business Premium har en lagringsgrense på 50 GB, da den bruker Exchange Online Plan 1.</span><span class="sxs-lookup"><span data-stu-id="31de9-193">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="31de9-194">Når du overfører til Microsoft 365 Business Premium, anbefales det at du tilordner denne brukeren en Exchange Online Plan 2 og fjerner Exchange Online Plan 1 fordi det ikke er mulig å tilordne begge.</span><span class="sxs-lookup"><span data-stu-id="31de9-194">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>


### <a name="threat-protection"></a><span data-ttu-id="31de9-195">Trusselbeskyttelse</span><span class="sxs-lookup"><span data-stu-id="31de9-195">Threat protection</span></span>

<span data-ttu-id="31de9-196">Etter at du har Microsoft 365 Business Premium, har du Defender for Office 365.</span><span class="sxs-lookup"><span data-stu-id="31de9-196">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="31de9-197">Se [Microsoft Defender for Office 365](../security/office-365-security/defender-for-office-365.md) for en oversikt.</span><span class="sxs-lookup"><span data-stu-id="31de9-197">See [Microsoft Defender for Office 365](../security/office-365-security/defender-for-office-365.md) for an overview.</span></span> <span data-ttu-id="31de9-198">Hvis du vil konfigurere dette, [kan](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)du se Konfigurere klarerte koblinger, konfigurere [klarerte](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)vedlegg og konfigurere [Phishing-phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)i Defender for Office 365 .</span><span class="sxs-lookup"><span data-stu-id="31de9-198">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="31de9-199">Følsomhetsetiketter</span><span class="sxs-lookup"><span data-stu-id="31de9-199">Sensitivity labels</span></span>

<span data-ttu-id="31de9-200">Hvis du vil begynne å bruke følsomhetsetiketter, kan du se [Oversikt over følsomhetsetiketter](../compliance/sensitivity-labels.md) [og opprette og behandle følsomhetsetiketter.](../business-video/create-sensitivity-labels.md)</span><span class="sxs-lookup"><span data-stu-id="31de9-200">To start using sensitivity labels, see [Overview of sensitivity labels](../compliance/sensitivity-labels.md) and [create and manage sensitivity labels](../business-video/create-sensitivity-labels.md) video.</span></span>
