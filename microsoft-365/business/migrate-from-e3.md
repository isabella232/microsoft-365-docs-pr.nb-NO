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
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="f8213-103">Overføre fra Office 365 E3 til Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="f8213-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span> 

<span data-ttu-id="f8213-104">Microsoft 365 Business Premium har alt du trenger for småbedrifter, og kombinerer de best i klassen skybaserte produktivitetsapper med enkel enhetsadministrasjon og sikkerhet.</span><span class="sxs-lookup"><span data-stu-id="f8213-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="f8213-105">Hvis du for øyeblikket har et Office 365 E3-abonnement, men ikke har mer enn 300 ansatte, kan du vurdere å bytte til Microsoft 365 Business Premium for ekstra sikkerhetsfunksjoner.</span><span class="sxs-lookup"><span data-stu-id="f8213-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="f8213-106">Det er enkelt å overføre: Først bytter du lisenser, og all data- og brukerinformasjon i det gjeldende abonnementet opprettholdes.</span><span class="sxs-lookup"><span data-stu-id="f8213-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="f8213-107">Etter overføringen må du konfigurere funksjonene som er lagt til i Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="f8213-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="f8213-108">Forskjeller mellom Office 365 E3 og Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="f8213-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="f8213-109">Denne tabellen viser forskjellene mellom Microsoft 365 Business Premium og Office 365 E3.</span><span class="sxs-lookup"><span data-stu-id="f8213-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="f8213-110">Funksjon</span><span class="sxs-lookup"><span data-stu-id="f8213-110">Feature</span></span>    | <span data-ttu-id="f8213-111">Støtte i Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="f8213-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="f8213-112">Støtte i Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="f8213-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="f8213-113">**Lokalt**</span><span class="sxs-lookup"><span data-stu-id="f8213-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="f8213-114">Office-apper<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="f8213-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="f8213-115">Microsoft 365-apper for bedrifter</span><span class="sxs-lookup"><span data-stu-id="f8213-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="f8213-116">Microsoft 365-apper for bedrifter</span><span class="sxs-lookup"><span data-stu-id="f8213-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="f8213-117">**Skyproduktivitetsapper**</span><span class="sxs-lookup"><span data-stu-id="f8213-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="f8213-118">Exchange Online og Outlook</span><span class="sxs-lookup"><span data-stu-id="f8213-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="f8213-119">50 GB lagringsgrense per postboks og ubegrenset Exchange Online-arkivering</span><span class="sxs-lookup"><span data-stu-id="f8213-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="f8213-120">100 GB lagringsgrense per postboks og ubegrenset Exchange Online-arkivering</span><span class="sxs-lookup"><span data-stu-id="f8213-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="f8213-121">Lag</span><span class="sxs-lookup"><span data-stu-id="f8213-121">Teams</span></span>    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="f8213-124">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="f8213-124">OneDrive for Business</span></span>    | <span data-ttu-id="f8213-125">1 TB lagringsgrense per bruker</span><span class="sxs-lookup"><span data-stu-id="f8213-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="f8213-126">Ubegrenset</span><span class="sxs-lookup"><span data-stu-id="f8213-126">Unlimited</span></span> | 
| <span data-ttu-id="f8213-127">Yammer, SharePoint Online, Planlegger, Strøm</span><span class="sxs-lookup"><span data-stu-id="f8213-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="f8213-130">AnsatteHub</span><span class="sxs-lookup"><span data-stu-id="f8213-130">StaffHub</span></span>    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="f8213-133">Kundeansvarlig for Outlook, MileIQ</span><span class="sxs-lookup"><span data-stu-id="f8213-133">Outlook Customer Manager, MileIQ</span></span>    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="f8213-135">**Beskyttelse mot trusler**</span><span class="sxs-lookup"><span data-stu-id="f8213-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="f8213-136">Office 365 Avansert trusselbeskyttelse (ATP)-plan 1</span><span class="sxs-lookup"><span data-stu-id="f8213-136">Office 365 Advanced Threat Protection (ATP) Plan 1</span></span> | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="f8213-138">Ikke inkludert, men kan legges til på</span><span class="sxs-lookup"><span data-stu-id="f8213-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="f8213-139">**Identitetsadministrasjon**</span><span class="sxs-lookup"><span data-stu-id="f8213-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="f8213-140">Selvbetjent tilbakestilling av passord for hybride Azure Active Directory-kontoer (Azure AD), Azure multifaktorautentisering (MFA), Betinget tilgang, passordskriving for lokale identiteter</span><span class="sxs-lookup"><span data-stu-id="f8213-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| <span data-ttu-id="f8213-142">**Administrasjon av enheter og apper**</span><span class="sxs-lookup"><span data-stu-id="f8213-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="f8213-143">Microsoft Intune, Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="f8213-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="f8213-145">Aktivering av delt datamaskin</span><span class="sxs-lookup"><span data-stu-id="f8213-145">Shared computer activation</span></span>|     ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Office 365 E3](../media/check-mark.png)| 
| <span data-ttu-id="f8213-148">Oppgrader rettigheter til Windows 10 Pro fra Win 7/8.1 Pro-lisenser</span><span class="sxs-lookup"><span data-stu-id="f8213-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    || 
| <span data-ttu-id="f8213-150">**Beskyttelse av informasjon**</span><span class="sxs-lookup"><span data-stu-id="f8213-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="f8213-151">Forebygging av tap av data i Office 365</span><span class="sxs-lookup"><span data-stu-id="f8213-151">Office 365 Data Loss Prevention</span></span>|    ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)|![Følger med Office 365 E3](../media/check-mark.png)|
|<span data-ttu-id="f8213-154">Azure Information Protection Plan 1, Bitlocker-håndhevelse</span><span class="sxs-lookup"><span data-stu-id="f8213-154">Azure Information Protection Plan 1, Bitlocker enforcement</span></span>|![Følger med Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="f8213-156">Azure Information Protection Plan 1, Følsomhetsetiketter</span><span class="sxs-lookup"><span data-stu-id="f8213-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Følger med Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="f8213-158">**Klienttilgangslisens (CAL-rettigheter)**</span><span class="sxs-lookup"><span data-stu-id="f8213-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="f8213-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="f8213-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Følger med Office 365 E3](../media/check-mark.png)|

<span data-ttu-id="f8213-161"><sup>1</sup> Microsoft 365 Business Premium-versjonen av Office-appene inkluderer ikke volumaktivering via gruppepolicy, apptelemetri, oppdateringskontroller, regnearksammenligning og forespørsel eller forretningsintelligens.</span><span class="sxs-lookup"><span data-stu-id="f8213-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="f8213-162">Migrasjon</span><span class="sxs-lookup"><span data-stu-id="f8213-162">Migration</span></span>

<span data-ttu-id="f8213-163">Hvis du vil overføre abonnementet, kan du se [Endre planer manuelt](../commerce/subscriptions/change-plans-manually.md) for instruksjoner hvis du vil flytte bare noen få personer til Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="f8213-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="f8213-164">Du kan også [oppgradere alle automatisk](../commerce/subscriptions/upgrade-to-different-plan.md), eller arbeide med en partner for å flytte E3-abonnementet og lisensene til et Microsoft 365 Business Premium-abonnement.</span><span class="sxs-lookup"><span data-stu-id="f8213-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="f8213-165">Avsnittene nedenfor beskriver endringene du må gjøre, om noen, og hva du kan gjøre etter overføringen.</span><span class="sxs-lookup"><span data-stu-id="f8213-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="f8213-166">Konfigurasjon og data for Office 365 E3-abonnement</span><span class="sxs-lookup"><span data-stu-id="f8213-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="f8213-167">Du trenger ikke å gjøre endringer i gjeldende abonnement eller data før du overfører, som inkluderer:</span><span class="sxs-lookup"><span data-stu-id="f8213-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="f8213-168">Abonnementskonfigurasjon, for eksempel DNS-poster og domenenavn.</span><span class="sxs-lookup"><span data-stu-id="f8213-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="f8213-169">Bruker- og gruppekontoer og godkjenningsinnstillinger, for eksempel godkjenning med flere faktorer eller policyer for betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="f8213-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="f8213-170">Produktivitetstjenestekonfigurasjoner og deres data, for eksempel Teams, Exchange Online-postbokser, SharePoint Online-områder, OneDrive for Business-mapper og OneNote-notatblokker.</span><span class="sxs-lookup"><span data-stu-id="f8213-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="f8213-171">Office-programmer skaleres automatisk.</span><span class="sxs-lookup"><span data-stu-id="f8213-171">Office applications will scale automatically.</span></span> <span data-ttu-id="f8213-172">Moderne lisensiering for Office 365 kontrollerer brukerens lisenstilordning hver 72.</span><span class="sxs-lookup"><span data-stu-id="f8213-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="f8213-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="f8213-173">Windows 10</span></span>

<span data-ttu-id="f8213-174">Hvis Windows ikke allerede er på Windows Pro Creator-oppdateringen, [kan du oppgradere dem til Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="f8213-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="f8213-175">Konfigurere policyer for å beskytte brukerenheter og filer</span><span class="sxs-lookup"><span data-stu-id="f8213-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="f8213-176">Hvis du konfigurerer Office 365 MDM-policyer og -enheter, vises disse enhetene på **Enheter-siden** i administrasjonssenteret for Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f8213-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="f8213-177">Alle policyer du konfigurerer, vises i listen over klassiske policyer i [Intune-portalen](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span><span class="sxs-lookup"><span data-stu-id="f8213-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="f8213-178">Når du har tilordnet lisenser til Microsoft 365 Business Premium, kan du begynne å beskytte brukernes enheter og filer.</span><span class="sxs-lookup"><span data-stu-id="f8213-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="f8213-179">Hvis du oppgraderte alle i organisasjonen til Microsoft 365 Business Premium, ser du installasjonsveiviseren på Hjem-siden, og kan følge [trinnene Konfigurer Microsoft 365 Business Premium i installasjonsveiviseren](set-up.md) for å beskytte filer og mobile enheter.</span><span class="sxs-lookup"><span data-stu-id="f8213-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="f8213-180">Du kan også fullføre disse trinnene på Enheter-siden:</span><span class="sxs-lookup"><span data-stu-id="f8213-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="f8213-181">Gå til **Devices** \> **Enhetspolicyer**i navigasjonsenheten til venstre.</span><span class="sxs-lookup"><span data-stu-id="f8213-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="f8213-182">Velg **Legg til**på Siden **Enhetspolicyer.**</span><span class="sxs-lookup"><span data-stu-id="f8213-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="f8213-183">I ruten **Legg til policy** gir du policyen et navn, og deretter velger du en **policytype** fra rullegardinlisten.</span><span class="sxs-lookup"><span data-stu-id="f8213-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="f8213-184">Du kan konfigurere programpolicyer for å beskytte filer på Android- og iPhone-enheter, i tillegg til Windows 10, og du kan konfigurere enhetskonfigurasjonspolicyer for bedriftseide Windows 10-enheter.</span><span class="sxs-lookup"><span data-stu-id="f8213-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="f8213-185">Se følgende koblinger for mer informasjon:</span><span class="sxs-lookup"><span data-stu-id="f8213-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="f8213-186">Angi innstillinger for appbeskyttelse på Android- eller iOS-enheter</span><span class="sxs-lookup"><span data-stu-id="f8213-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="f8213-187">Angi innstillinger for appbeskyttelse for Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="f8213-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="f8213-188">Angi innstillinger for enhetsbeskyttelse for Windows 10-PCer</span><span class="sxs-lookup"><span data-stu-id="f8213-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="f8213-189">Når du har konfigurert policyer, kan du og de ansatte konfigurere enheter:</span><span class="sxs-lookup"><span data-stu-id="f8213-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="f8213-190">Se [Konfigurere Windows-enheter for Microsoft 365 Business Premium-brukere](set-up-windows-devices.md) for trinn for Windows-enheter.</span><span class="sxs-lookup"><span data-stu-id="f8213-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="f8213-191">Se [Konfigurere mobile enheter for Microsoft 365 Business Premium-brukere](set-up-mobile-devices.md) for trinn for Android-telefoner og iPhoner.</span><span class="sxs-lookup"><span data-stu-id="f8213-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 

### <a name="threat-protection"></a><span data-ttu-id="f8213-192">Beskyttelse mot trusler</span><span class="sxs-lookup"><span data-stu-id="f8213-192">Threat protection</span></span>

<span data-ttu-id="f8213-193">Når du har overført til Microsoft 365 Business Premium, har du Office 365 ATP.</span><span class="sxs-lookup"><span data-stu-id="f8213-193">After migrating to Microsoft 365 Business Premium, you have Office 365 ATP.</span></span> <span data-ttu-id="f8213-194">Se [Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for en oversikt.</span><span class="sxs-lookup"><span data-stu-id="f8213-194">See [Office 365 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for an overview.</span></span> <span data-ttu-id="f8213-195">Hvis du vil konfigurere, kan du se [konfigurere ATP-sikre koblinger](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [konfigurere ATP-sikre vedlegg](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)og konfigurere [ATP-anti-phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span><span class="sxs-lookup"><span data-stu-id="f8213-195">To set up, see [set up ATP safe links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up ATP safe attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up ATP anti-phishing](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="f8213-196">Følsomhetsetiketter</span><span class="sxs-lookup"><span data-stu-id="f8213-196">Sensitivity labels</span></span>

<span data-ttu-id="f8213-197">Hvis du vil begynne å bruke følsomhetsetiketter, kan du se [Oversikt over følsomhetsetiketter](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) og [opprette og administrere følsomhetsetiketter](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span><span class="sxs-lookup"><span data-stu-id="f8213-197">To start using sensitivity labels, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>
