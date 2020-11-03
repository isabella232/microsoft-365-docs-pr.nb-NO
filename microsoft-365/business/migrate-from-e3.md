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
# <a name="migrating-from-office-365-e3-to-microsoft-365-business-premium"></a><span data-ttu-id="3dc20-103">Overføre fra Office 365 E3 til Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="3dc20-103">Migrating from Office 365 E3 to Microsoft 365 Business Premium</span></span> 

<span data-ttu-id="3dc20-104">Microsoft 365 Business Premium har alt du trenger for å bruke små bedrifter til å kombinere de beste Sky BAS ert produktivitets appene med enkel enhets administrasjon og sikkerhet.</span><span class="sxs-lookup"><span data-stu-id="3dc20-104">Microsoft 365 Business Premium has everything you need for your small business, combining the best-in-class cloud-based productivity apps with simple device management and security.</span></span> <span data-ttu-id="3dc20-105">Hvis du for øyeblikket har et Office 365-E3-abonnement, men ikke har mer enn 300 med arbeidere, kan du vurdere å bytte til Microsoft 365 Business Premium for å få nye sikkerhets funksjoner.</span><span class="sxs-lookup"><span data-stu-id="3dc20-105">If you currently have an Office 365 E3 subscription, but don't have more than 300 employees, consider switching to Microsoft 365 Business Premium for added security features.</span></span>

<span data-ttu-id="3dc20-106">Det er enkelt å overføre: først bytter du lisenser, og alle dataene og bruker opplysningene i det gjeldende abonnementet beholdes.</span><span class="sxs-lookup"><span data-stu-id="3dc20-106">Migrating is easy: First you switch licenses and all your data and user information in your current subscription is maintained.</span></span> <span data-ttu-id="3dc20-107">Etter overføringen må du konfigurere funksjonene som er lagt til i Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="3dc20-107">After the migration, you'll need to set up the features that are added in Microsoft 365 Business Premium.</span></span>

## <a name="differences-between-office-365-e3-and-microsoft-365-business-premium"></a><span data-ttu-id="3dc20-108">Forskjeller mellom Office 365 E3 og Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="3dc20-108">Differences between Office 365 E3 and Microsoft 365 Business Premium</span></span>

<span data-ttu-id="3dc20-109">Denne tabellen viser forskjellene mellom Microsoft 365 Business Premium og Office 365 E3.</span><span class="sxs-lookup"><span data-stu-id="3dc20-109">This table shows the differences between Microsoft 365 Business Premium and Office 365 E3.</span></span>

| <span data-ttu-id="3dc20-110">Funksjon</span><span class="sxs-lookup"><span data-stu-id="3dc20-110">Feature</span></span>    | <span data-ttu-id="3dc20-111">Støtte i Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="3dc20-111">Support in Microsoft 365 Business Premium</span></span>    | <span data-ttu-id="3dc20-112">Støtte i Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="3dc20-112">Support in Office 365 E3</span></span> | 
|:-------|:-----|:-----|
| <span data-ttu-id="3dc20-113">**Lokalt**</span><span class="sxs-lookup"><span data-stu-id="3dc20-113">**On-premises**</span></span>        | | | 
| <span data-ttu-id="3dc20-114">Office-apper<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="3dc20-114">Office apps<sup>1</sup></span></span>    | <span data-ttu-id="3dc20-115">Microsoft 365-apper for bedrifter</span><span class="sxs-lookup"><span data-stu-id="3dc20-115">Microsoft 365 Apps for business</span></span>    | <span data-ttu-id="3dc20-116">Microsoft 365-apper for enterprise</span><span class="sxs-lookup"><span data-stu-id="3dc20-116">Microsoft 365 Apps for enterprise</span></span> | 
| <span data-ttu-id="3dc20-117">**Produktivitets programmer for skyen**</span><span class="sxs-lookup"><span data-stu-id="3dc20-117">**Cloud productivity apps**</span></span>        | | | 
| <span data-ttu-id="3dc20-118">Exchange Online og Outlook</span><span class="sxs-lookup"><span data-stu-id="3dc20-118">Exchange Online and Outlook</span></span>    | <span data-ttu-id="3dc20-119">lagrings grensen på 50 GB per post boks og ubegrenset Exchange Online-arkivering</span><span class="sxs-lookup"><span data-stu-id="3dc20-119">50 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span>    | <span data-ttu-id="3dc20-120">lagrings grensen på 100 GB per post boks og ubegrenset Exchange Online-arkivering</span><span class="sxs-lookup"><span data-stu-id="3dc20-120">100 GB storage limit per mailbox and unlimited Exchange Online Archiving</span></span> | 
| <span data-ttu-id="3dc20-121">Team</span><span class="sxs-lookup"><span data-stu-id="3dc20-121">Teams</span></span>    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="3dc20-124">OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="3dc20-124">OneDrive for Business</span></span>    | <span data-ttu-id="3dc20-125">1 TB lagrings grense per bruker</span><span class="sxs-lookup"><span data-stu-id="3dc20-125">1 TB storage limit per user</span></span>    | <span data-ttu-id="3dc20-126">Uendelige</span><span class="sxs-lookup"><span data-stu-id="3dc20-126">Unlimited</span></span> | 
| <span data-ttu-id="3dc20-127">Yammer, SharePoint Online, Planner, dataflyt</span><span class="sxs-lookup"><span data-stu-id="3dc20-127">Yammer, SharePoint Online, Planner, Stream</span></span>    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="3dc20-130">StaffHub</span><span class="sxs-lookup"><span data-stu-id="3dc20-130">StaffHub</span></span>    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png) | 
| <span data-ttu-id="3dc20-133">Outlook Customer Manager, MileIQ</span><span class="sxs-lookup"><span data-stu-id="3dc20-133">Outlook Customer Manager, MileIQ</span></span>    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| <span data-ttu-id="3dc20-135">**Trussel beskyttelse**</span><span class="sxs-lookup"><span data-stu-id="3dc20-135">**Threat Protection**</span></span>        | | | 
| <span data-ttu-id="3dc20-136">Defender for Office 365 plan 1</span><span class="sxs-lookup"><span data-stu-id="3dc20-136">Defender for Office 365 Plan 1</span></span> | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | <span data-ttu-id="3dc20-138">Ikke inkludert, men kan legges til på</span><span class="sxs-lookup"><span data-stu-id="3dc20-138">Not included, but can be added on</span></span> | 
| <span data-ttu-id="3dc20-139">**Identitets behandling**</span><span class="sxs-lookup"><span data-stu-id="3dc20-139">**Identity management**</span></span>        | | | 
| <span data-ttu-id="3dc20-140">Selv betjent tilbakestilling av passord for hybride Azure Active Directory-kontoer (Azure AD), Azure multi-Factor Authentication (MFA), betinget tilgang, passord bakgrunn for lokale identiteter</span><span class="sxs-lookup"><span data-stu-id="3dc20-140">Self-service password reset for hybrid Azure Active Directory (Azure AD) accounts, Azure multi-factor authentication (MFA), Conditional Access, password writeback for on-premises identities</span></span>|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    |  | 
| <span data-ttu-id="3dc20-142">**Enhets-og app-behandling**</span><span class="sxs-lookup"><span data-stu-id="3dc20-142">**Device and app management**</span></span>        | | |
| <span data-ttu-id="3dc20-143">Microsoft Intune, Windows autopilot</span><span class="sxs-lookup"><span data-stu-id="3dc20-143">Microsoft Intune, Windows AutoPilot</span></span>|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    |  |
| <span data-ttu-id="3dc20-145">Aktivering av delt data maskin</span><span class="sxs-lookup"><span data-stu-id="3dc20-145">Shared computer activation</span></span>|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Office 365 E3](../media/check-mark.png)| 
| <span data-ttu-id="3dc20-148">Oppgraderings rettigheter til Windows 10 Pro fra Win 7/8.1 Pro-lisenser</span><span class="sxs-lookup"><span data-stu-id="3dc20-148">Upgrade rights to Windows 10 Pro from Win 7/8.1 Pro licenses</span></span>|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    || 
| <span data-ttu-id="3dc20-150">**Informasjons beskyttelse**</span><span class="sxs-lookup"><span data-stu-id="3dc20-150">**Information protection**</span></span>        | | |
|<span data-ttu-id="3dc20-151">Office 365 datatap-hindring</span><span class="sxs-lookup"><span data-stu-id="3dc20-151">Office 365 Data Loss Prevention</span></span>|    ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)|![Inkludert i Office 365 E3](../media/check-mark.png)|
|<span data-ttu-id="3dc20-154">Azure Information Protection Plan 1, BitLocker-håndhevelse</span><span class="sxs-lookup"><span data-stu-id="3dc20-154">Azure Information Protection Plan 1, Bitlocker enforcement</span></span>|![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="3dc20-156">Azure Information Protection Plan 1, følsomhet-etiketter</span><span class="sxs-lookup"><span data-stu-id="3dc20-156">Azure Information Protection Plan 1, Sensitivity labels</span></span>|![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)||
|<span data-ttu-id="3dc20-158">**Klient adgangs lisens (CAL-rettigheter)**</span><span class="sxs-lookup"><span data-stu-id="3dc20-158">**Client Access License (CAL rights)**</span></span>|||
|<span data-ttu-id="3dc20-159">Enterprise CAL-programserie (Exchange, SharePoint, Skype)</span><span class="sxs-lookup"><span data-stu-id="3dc20-159">Enterprise CAL Suite (Exchange, SharePoint, Skype)</span></span>||![Inkludert i Office 365 E3](../media/check-mark.png)|

<span data-ttu-id="3dc20-161"><sup>1</sup> Microsoft 365 Business Premium-versjonen av Office-appene omfatter ikke volum aktivering via gruppe policy, telemetribehandling for apper, oppdaterings kontroller, regne ark sammenligning og forespørsel eller forretnings intelligens.</span><span class="sxs-lookup"><span data-stu-id="3dc20-161"><sup>1</sup> The Microsoft 365 Business Premium version of the Office apps doesn't include volume activation through Group Policy, app telemetry, update controls, spreadsheet compare and inquire, or business Intelligence.</span></span>

## <a name="migration"></a><span data-ttu-id="3dc20-162">Medlemsserver</span><span class="sxs-lookup"><span data-stu-id="3dc20-162">Migration</span></span>

<span data-ttu-id="3dc20-163">Hvis du vil overføre abonnementet, kan du se [endre planer manuelt](../commerce/subscriptions/change-plans-manually.md) hvis du vil flytte bare noen få personer til Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="3dc20-163">To migrate your subscription, see [Change plans manually](../commerce/subscriptions/change-plans-manually.md) for instructions if you want to move just a few people to Microsoft 365 Business Premium.</span></span> <span data-ttu-id="3dc20-164">Du kan også [oppgradere alle automatisk](../commerce/subscriptions/upgrade-to-different-plan.md), eller arbeide med en partner for å flytte E3-abonnementet og-lisensene til et Microsoft 365 Business Premium-abonnement.</span><span class="sxs-lookup"><span data-stu-id="3dc20-164">You can also [upgrade everyone automatically](../commerce/subscriptions/upgrade-to-different-plan.md), or work with a partner to move your E3 subscription and licenses to a Microsoft 365 Business Premium subscription.</span></span>
<span data-ttu-id="3dc20-165">De følgende avsnittene beskriver endringene du trenger for å gjøre, og hva du kan gjøre etter overføringen.</span><span class="sxs-lookup"><span data-stu-id="3dc20-165">The following sections describe the changes you need to make, if any, and what you can do after the migration.</span></span>

### <a name="office-365-e3-subscription-configuration-and-data"></a><span data-ttu-id="3dc20-166">Konfigurasjon og data for E3-abonnement for Office 365</span><span class="sxs-lookup"><span data-stu-id="3dc20-166">Office 365 E3 subscription configuration and data</span></span>
<span data-ttu-id="3dc20-167">Du trenger ikke å gjøre endringer i gjeldende abonnement eller data før du overfører, som omfatter følgende:</span><span class="sxs-lookup"><span data-stu-id="3dc20-167">You don't need to do any changes to your current subscription or data before migrating, which includes:</span></span>

- <span data-ttu-id="3dc20-168">Abonnements konfigurasjon, for eksempel DNS-poster og domene navn.</span><span class="sxs-lookup"><span data-stu-id="3dc20-168">Subscription configuration, such as DNS records and domain names.</span></span>
- <span data-ttu-id="3dc20-169">Bruker-og gruppe kontoer og godkjennings innstillinger, for eksempel godkjenning for flere faktorer eller policyer for betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="3dc20-169">User and group accounts and authentication settings, such as multi factor authentication or conditional access policies.</span></span>
- <span data-ttu-id="3dc20-170">Produktivitets tjeneste konfigurasjoner og tilhørende data, for eksempel team, Exchange Online-postbokser, SharePoint Online-nettsteder, OneDrive for Business-mapper og OneNote-notatblokker.</span><span class="sxs-lookup"><span data-stu-id="3dc20-170">Productivity service configurations and their data, such as Teams, Exchange Online mailboxes, SharePoint Online sites, OneDrive for Business folders, and OneNote notebooks.</span></span>
- <span data-ttu-id="3dc20-171">Office-programmer skalerer automatisk.</span><span class="sxs-lookup"><span data-stu-id="3dc20-171">Office applications will scale automatically.</span></span> <span data-ttu-id="3dc20-172">Office 365 moderne lisensiering vil kontrollere brukerens lisens tilordning hver 72 timer, og vil konvertere Office-programmer til versjonen som Sams varer med bruker abonnementet.</span><span class="sxs-lookup"><span data-stu-id="3dc20-172">Office 365 modern licensing will check the user’s license assignment every 72 hours and will convert Office applications to the version that matches the user subscription.</span></span>

### <a name="windows-10"></a><span data-ttu-id="3dc20-173">Windows 10</span><span class="sxs-lookup"><span data-stu-id="3dc20-173">Windows 10</span></span>

<span data-ttu-id="3dc20-174">Hvis Windows ikke allerede er på Windows Pro Creator-oppdateringen, [oppgraderer du dem til Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="3dc20-174">If your Windows aren't already on Windows Pro Creator update, [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>

### <a name="set-up-policies-to-protect-user-devices-and-files"></a><span data-ttu-id="3dc20-175">Konfigurere policyer for å beskytte bruker enheter og filer</span><span class="sxs-lookup"><span data-stu-id="3dc20-175">Set up policies to protect user devices and files</span></span>

> [!NOTE]
> <span data-ttu-id="3dc20-176">Hvis du konfigurerer Office 365 MDM-policyer og-enheter, vil disse enhetene være oppført på **enheter** -siden i administrasjons senteret for Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3dc20-176">If you set up Office 365 MDM policies and devices, those devices will be listed on the **Devices** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="3dc20-177">Policyer du konfigurerer, vises i listen over klassiske policyer i [Intune-portalen](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span><span class="sxs-lookup"><span data-stu-id="3dc20-177">Any policies you set up will show up in the list of classic policies in the [Intune portal](https://portal.azure.com/#blade/Microsoft_Intune_DeviceSettings/ExtensionLandingBlade/overview).</span></span>

<span data-ttu-id="3dc20-178">Når du har tilordnet lisenser til Microsoft 365 Business Premium, kan du begynne å beskytte brukernes enheter og filer.</span><span class="sxs-lookup"><span data-stu-id="3dc20-178">After you have assigned licenses to Microsoft 365 Business Premium, you can start protecting the users' devices and files.</span></span>

<span data-ttu-id="3dc20-179">Hvis du har oppgradert alle i organisasjonen til Microsoft 365 Business Premium, ser du konfigurasjons vei viseren på Starts IDen, og du kan følge [konfigureringen av Microsoft 365 Business Premium i vei viseren for konfigurasjon av installasjons programmet](set-up.md) for å beskytte filer og mobile enheter.</span><span class="sxs-lookup"><span data-stu-id="3dc20-179">If you upgraded everyone in your organization to Microsoft 365 Business Premium, you'll see the setup wizard on the Home page, and can follow the [Set up Microsoft 365 Business Premium in the setup wizard](set-up.md) steps to protect files and mobile devices.</span></span>

<span data-ttu-id="3dc20-180">Du kan også fullføre disse trinnene på enheter-siden:</span><span class="sxs-lookup"><span data-stu-id="3dc20-180">You can also complete these steps on the Devices page:</span></span>
  
1. <span data-ttu-id="3dc20-181">Gå til **enhets** policyer i den venstre ruten i administrasjons senteret \> **Policies**.</span><span class="sxs-lookup"><span data-stu-id="3dc20-181">In the admin center, in the left nav, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="3dc20-182">Velg **Legg til** på siden **enhets policyer** .</span><span class="sxs-lookup"><span data-stu-id="3dc20-182">On the **Device policies** page, choose **Add**.</span></span>
    
3. <span data-ttu-id="3dc20-183">I **Legg til policy** -ruten gir du policyen et navn, og deretter velger du en **policy type** fra rulle gardin listen.</span><span class="sxs-lookup"><span data-stu-id="3dc20-183">In the **Add policy** pane give the policy a name, and then choose a **Policy type** from the drop-down.</span></span> 
    
     <span data-ttu-id="3dc20-184">Du kan konfigurere program policyer for å beskytte filer på Android-og iPhone-enheter, i tillegg til Windows 10, og du kan konfigurere policyer for enhets konfigurasjon for firmaet som eier Windows 10-enheter.</span><span class="sxs-lookup"><span data-stu-id="3dc20-184">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="3dc20-185">Se følgende koblinger for mer informasjon:</span><span class="sxs-lookup"><span data-stu-id="3dc20-185">See the following links for details:</span></span>
    
  - [<span data-ttu-id="3dc20-186">Angi innstillinger for appbeskyttelse på Android- eller iOS-enheter</span><span class="sxs-lookup"><span data-stu-id="3dc20-186">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="3dc20-187">Angi innstillinger for appbeskyttelse for Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="3dc20-187">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="3dc20-188">Angi innstillinger for enhets beskyttelse for Windows 10-PC-er</span><span class="sxs-lookup"><span data-stu-id="3dc20-188">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  
4. <span data-ttu-id="3dc20-189">Når du har konfigurert policyer, kan du og de ansatte konfigurere enheter:</span><span class="sxs-lookup"><span data-stu-id="3dc20-189">Once you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="3dc20-190">Se [konfigurere Windows-enheter for Microsoft 365 Business Premium-brukere](set-up-windows-devices.md) for trinn for Windows-enheter.</span><span class="sxs-lookup"><span data-stu-id="3dc20-190">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="3dc20-191">Se [konfigurere mobile enheter for Microsoft 365 Business Premium-brukere](set-up-mobile-devices.md) for trinn for Android-telefoner og-iPhone.</span><span class="sxs-lookup"><span data-stu-id="3dc20-191">See [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
  
### <a name="mailbox-size"></a><span data-ttu-id="3dc20-192">Post boks størrelse</span><span class="sxs-lookup"><span data-stu-id="3dc20-192">Mailbox Size</span></span>

<span data-ttu-id="3dc20-193">Microsoft 365 Business Premium har en lagrings grense på 50 GB fordi den bruker Exchange Online plan 1.</span><span class="sxs-lookup"><span data-stu-id="3dc20-193">Microsoft 365 Business Premium has a 50 GB storage limit as it uses Exchange Online Plan 1.</span></span> <span data-ttu-id="3dc20-194">Når du overfører til Microsoft 365 Business Premium, anbefales det at du tilordner denne brukeren en Exchange Online-plan 2 og fjerner Exchange Online-planen 1 som det ikke er mulig å tilordne begge, hvis noen av brukerne overskrider 50 GB.</span><span class="sxs-lookup"><span data-stu-id="3dc20-194">While migrating to Microsoft 365 Business Premium, if any of your users exceed 50 GB of mailbox storage, it is recommended that you assign this user an Exchange Online Plan 2 and remove the Exchange Online Plan 1 as it's not feasible to assign both.</span></span>


### <a name="threat-protection"></a><span data-ttu-id="3dc20-195">Trussel beskyttelse</span><span class="sxs-lookup"><span data-stu-id="3dc20-195">Threat protection</span></span>

<span data-ttu-id="3dc20-196">Når du har overført til Microsoft 365 Business Premium, har du Defender for Office 365.</span><span class="sxs-lookup"><span data-stu-id="3dc20-196">After migrating to Microsoft 365 Business Premium, you have Defender for Office 365.</span></span> <span data-ttu-id="3dc20-197">Se [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for en oversikt.</span><span class="sxs-lookup"><span data-stu-id="3dc20-197">See [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) for an overview.</span></span> <span data-ttu-id="3dc20-198">Hvis du vil konfigurere, kan du se [konfigurere sikre koblinger](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [konfigurere sikre vedlegg](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)og [konfigurere anti-phishing i Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span><span class="sxs-lookup"><span data-stu-id="3dc20-198">To set up, see [set up Safe Links](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa), [set up Safe Attachments](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5), and [set up Anti-phishing in Defender for Office 365](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c).</span></span>

### <a name="sensitivity-labels"></a><span data-ttu-id="3dc20-199">Følsomhetsetiketter</span><span class="sxs-lookup"><span data-stu-id="3dc20-199">Sensitivity labels</span></span>

<span data-ttu-id="3dc20-200">Hvis du vil begynne å bruke følsomhet etiketter, kan du se [Oversikt over følsomhet](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) og [opprette og behandle](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video om følsomhet-etiketter.</span><span class="sxs-lookup"><span data-stu-id="3dc20-200">To start using sensitivity labels, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels) and [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>
