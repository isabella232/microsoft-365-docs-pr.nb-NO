---
title: Konfigurere Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Lær hvordan du konfigurerer Microsoft 365 Business.
ms.openlocfilehash: e635b828609fc47cd8b92bb179a25bcc43cb0a1a
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660853"
---
# <a name="set-up-microsoft-365-business"></a><span data-ttu-id="39511-103">Konfigurere Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="39511-103">Set up Microsoft 365 Business</span></span>

<span data-ttu-id="39511-104">Før du begynner, kan du se [Få Microsoft 365 Business](get-microsoft-365-business.md) for registrering detaljene.</span><span class="sxs-lookup"><span data-stu-id="39511-104">Before you get started, see [Get Microsoft 365 Business](get-microsoft-365-business.md) for sign-up details.</span></span>

<span data-ttu-id="39511-105">Se en [kort video om hvordan du konfigurerer Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) ved hjelp av Sett opp veiviseren, og når du ikke har en lokale Active Directory</span><span class="sxs-lookup"><span data-stu-id="39511-105">Watch a [short video on how to set up Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) by using the set up wizard, and when you don't have an on-premises Active Directory</span></span>
  

## <a name="overview"></a><span data-ttu-id="39511-106">Oversikt</span><span class="sxs-lookup"><span data-stu-id="39511-106">Overview</span></span>

<span data-ttu-id="39511-107">Det meste av den er satt opp trinnene kan gjøres i installasjonsveiviseren, men de andre alternativene er også oppført.</span><span class="sxs-lookup"><span data-stu-id="39511-107">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>

1. <span data-ttu-id="39511-108">[Legg til domenet ditt](#add-your-domain-to-personalize-sign-in) (Hvis du kjøpte domenet ditt ved å [registrere deg](sign-up.md), dette trinnet er allerede har gjort.)</span><span class="sxs-lookup"><span data-stu-id="39511-108">[Add your domain](#add-your-domain-to-personalize-sign-in) (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>
2. <span data-ttu-id="39511-109">Legg til brukere.</span><span class="sxs-lookup"><span data-stu-id="39511-109">Add users.</span></span> <span data-ttu-id="39511-110">Du kan gjøre dette på en av tre måter:</span><span class="sxs-lookup"><span data-stu-id="39511-110">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="39511-111">I [installasjonsveiviseren](#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="39511-111">In the [setup wizard](#add-users-in-the-wizard).</span></span>
    - <span data-ttu-id="39511-112">Bruk katalogsynkronisering for å [legge til brukere ved hjelp av Azure AD-tilkobling](#add-users-by-using-azure-ad-connect) Hvis du har en lokale Active directory.</span><span class="sxs-lookup"><span data-stu-id="39511-112">Use directory synchronization to [add users by using Azure AD Connect](#add-users-by-using-azure-ad-connect) if you have an on-premises Active directory.</span></span>
    - <span data-ttu-id="39511-113">Du kan også [legge til senere brukere](add-users-m365b.md) i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="39511-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
3. <span data-ttu-id="39511-114">Definere retningslinjer for sikkerhet og konfigurere enheter.</span><span class="sxs-lookup"><span data-stu-id="39511-114">Set up security policies and configure devices.</span></span> <span data-ttu-id="39511-115">Du kan gjøre dette på en av tre måter:</span><span class="sxs-lookup"><span data-stu-id="39511-115">You can do this in any of the three ways:</span></span>
    - <span data-ttu-id="39511-116">I [installasjonsveiviseren](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="39511-116">In the [setup wizard](#set-up-policies-in-the-wizard).</span></span>  
    - <span data-ttu-id="39511-117">[Administrasjonssenteret](#modify-or-add-policies-in-the-admin-center).</span><span class="sxs-lookup"><span data-stu-id="39511-117">In the [admin center](#modify-or-add-policies-in-the-admin-center).</span></span>
    - <span data-ttu-id="39511-118">[Intune administrasjonssenteret](https://docs.microsoft.com/intune/what-is-device-management).</span><span class="sxs-lookup"><span data-stu-id="39511-118">In the [Intune admin center](https://docs.microsoft.com/intune/what-is-device-management).</span></span>
4. <span data-ttu-id="39511-119">Definer og administrer Windows 10 enheter.</span><span class="sxs-lookup"><span data-stu-id="39511-119">Set up and manage Windows 10 devices.</span></span>

    <span data-ttu-id="39511-120">Når du slår sammen en enhet for WIndows 10 Azure AD, får alle policyene brukes på den.</span><span class="sxs-lookup"><span data-stu-id="39511-120">When you join a WIndows 10 device to Azure AD, all the policies get applied to it.</span></span>
    - <span data-ttu-id="39511-121">Sette opp Windows 10 enheten konfigurasjoner i [installasjonsveiviseren](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="39511-121">Set up Windows 10 device configurations in the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="39511-122">Bli med i en [ny enhet for Windows 10](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="39511-122">Join a [new Windows 10 device](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) to Azure AD.</span></span>
    - <span data-ttu-id="39511-123">Koble en [eksisterende Windows-10-enhet](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="39511-123">Join an [existing Windows 10 device](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) to Azure AD.</span></span>
1. <span data-ttu-id="39511-124">Installer Office 365 Business.</span><span class="sxs-lookup"><span data-stu-id="39511-124">Install Office 365 Business.</span></span>
    - <span data-ttu-id="39511-125">Du kan installere Office automatisk i Windows-enheter ved hjelp av [installasjonsveiviseren](#set-up-policies-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="39511-125">You can automatically install Office in the Windows devices by using the [setup wizard](#set-up-policies-in-the-wizard).</span></span>
    - <span data-ttu-id="39511-126">Automatisk [installerer Office](auto-install-or-uninstall-office.md) fra administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="39511-126">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
    - <span data-ttu-id="39511-127">La brukere [installere Office-programmer](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows og enheter.</span><span class="sxs-lookup"><span data-stu-id="39511-127">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
1. <span data-ttu-id="39511-128">Angi ekstra sikkerhet.</span><span class="sxs-lookup"><span data-stu-id="39511-128">Set up additional security.</span></span>
    - <span data-ttu-id="39511-129">Veiviseren legger til policyer for å sikre dine enheter, men du kan også dra nytte av [ytterligere](#additional-security-settings) sikkerhetsfunksjoner til bidrar til å sikre dine data, kontoer og e-post.</span><span class="sxs-lookup"><span data-stu-id="39511-129">The setup wizard adds policies to secure your devices, but you can also take advantage of [additional security](#additional-security-settings) capabilities to helps secure your data, accounts, and emails.</span></span> 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="39511-130">Legge til domenet, brukere og definere policyer</span><span class="sxs-lookup"><span data-stu-id="39511-130">Add your domain, users and set up policies</span></span>

![Banner som peker til https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="39511-132">Når du kjøper Microsoft 365 Business, har du muligheten til å bruke et domene du eier, eller kjøpe en i løpet av [registreringen](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="39511-132">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="39511-133">Hvis du har kjøpt et nytt domene når du registrerte deg, domenet er alle satt opp, og du kan flytte for å [legge til brukere og tilordne lisenser](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="39511-133">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="39511-134">Legge til domenet for å tilpasse pålogging</span><span class="sxs-lookup"><span data-stu-id="39511-134">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="39511-135">Logg på [administrasjonssenteret for Microsoft 365](https://admin.microsoft.com) ved hjelp av global admin-rettigheter.</span><span class="sxs-lookup"><span data-stu-id="39511-135">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="39511-136">Velg **Legg til et domene** for å starte veiviseren.</span><span class="sxs-lookup"><span data-stu-id="39511-136">Choose **Add a domain** to start the wizard.</span></span>

    ![Velg Legg til et domene.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="39511-138">I veiviseren angir du navnet på domenet du vil bruke (for eksempel contoso.com).</span><span class="sxs-lookup"><span data-stu-id="39511-138">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Skjermbilde av Tilpass på siden.](media/personalizesignin.png)

    
4. <span data-ttu-id="39511-140">Følg trinnene i veiviseren til å [opprette DNS-poster på alle DNS-vertsleverandøren for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , som bekrefter at du eier domenet.</span><span class="sxs-lookup"><span data-stu-id="39511-140">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="39511-141">Hvis du kjenner ditt domene host, se også [vert for spesifikke instruksjoner](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="39511-141">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="39511-142">Hvis din vertsleverandøren er GoDaddy, prosessen er enkelt, og du blir automatisk bedt om å logge på og la Microsoft godkjenne på dine vegne:</span><span class="sxs-lookup"><span data-stu-id="39511-142">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![Velg Godkjenn på GoDaddy bekrefte tilgang-siden.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="39511-144">Legge til brukere og tilordne lisenser</span><span class="sxs-lookup"><span data-stu-id="39511-144">Add users and assign licenses</span></span>

<span data-ttu-id="39511-145">Du kan legge til brukere i veiviseren, men du kan også [legge til senere brukere](add-users-m365b.md) i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="39511-145">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="39511-146">Hvis du har en lokal domenekontroller, kan du i tillegg legge til brukere med [Azure AD-tilkobling](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="39511-146">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="39511-147">Legge til brukere i veiviseren</span><span class="sxs-lookup"><span data-stu-id="39511-147">Add users in the wizard</span></span>

<span data-ttu-id="39511-148">Eventuelle brukere du legger til i veiviseren Hent automatisk tilordnet en lisens for Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="39511-148">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>
<span data-ttu-id="39511-149">Hvis du har en lokal domenekontroller, og bruker Active Directory, kan du se [hvordan ddd brukere ved hjelp av Azure AD-tilkobling](#add-users-by-using-azure-ad-connect).</span><span class="sxs-lookup"><span data-stu-id="39511-149">If you have a local domain controller, and are using Active Directory, see [how to ddd users by using Azure AD Connect](#add-users-by-using-azure-ad-connect).</span></span>

![Skjermbilde av siden Legg til nye brukere i veiviseren](media/addnewuserspage.png)

1. <span data-ttu-id="39511-p106">Hvis ditt Microsoft 365 Business-abonnement har eksisterende brukere (for eksempel hvis du brukte Azure AD Connect), får du muligheten til å tildele lisenser til dem nå. Gå videre og legg til lisenser for dem også.</span><span class="sxs-lookup"><span data-stu-id="39511-p106">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you will get an option to assign licenses to them now. Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="39511-153">Når du har lagt til brukerne, får du også muligheten til å dele legitimasjon med de nye brukerne du har lagt til.</span><span class="sxs-lookup"><span data-stu-id="39511-153">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="39511-154">Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.</span><span class="sxs-lookup"><span data-stu-id="39511-154">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="39511-155">Hopp over overføring av e-postmeldinger, og velg **Neste** på **Overfør e-postmeldinger**-siden.</span><span class="sxs-lookup"><span data-stu-id="39511-155">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="39511-156">Hvis du flytter fra en annen leverandør av e-post og vil kopiere dataene senere, kan du [Overfør e-post og kontakter til Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="39511-156">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>

#### <a name="add-users-by-using-azure-ad-connect"></a><span data-ttu-id="39511-157">Legge til brukere ved hjelp av Azure AD-tilkobling</span><span class="sxs-lookup"><span data-stu-id="39511-157">Add users by using Azure AD Connect</span></span>

 <span data-ttu-id="39511-158">Hvis du har en lokal domenekontroller med Active Directory, synkroniserer du brukerne med Microsoft 365 Business ved hjelp av [Azure AD-tilkobling](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="39511-158">If you have a local domain controller with Active Directory, you synchronize your users with Microsoft 365 Business by using [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span> <span data-ttu-id="39511-159">Fullfør dette før du starter veiviseren.</span><span class="sxs-lookup"><span data-stu-id="39511-159">Complete this before you start the setup wizard.</span></span> <span data-ttu-id="39511-160">Du kan laste den ned i administrasjonssenteret:</span><span class="sxs-lookup"><span data-stu-id="39511-160">You can download it in the admin center:</span></span>

- <span data-ttu-id="39511-161">Gå til **brukere** \> **aktive brukere**, velg ellipser øverst på siden, og velg deretter **katalogsynkronisering** for å laste ned Azure AD-tilkobling.</span><span class="sxs-lookup"><span data-stu-id="39511-161">Go to **Users** \> **Active users**, select the ellipses on the top of the page and then select **Directory synchronization** to download Azure AD Connect.</span></span>

    ![Velg ellipser > Directory snchronization på aktive brukere-siden.](media/setupdirsync.png)

    > [!IMPORTANT]
    > <span data-ttu-id="39511-163">Hvis du oppretter brukere på denne måten, vil du fortsatt har til å tilordne lisenser til dem i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="39511-163">If you create users this way, you will still have to assign licenses to them in the admin center.</span></span>

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a><span data-ttu-id="39511-164">Fortsette å få tilgang til domenetilknyttede programmer og enheter</span><span class="sxs-lookup"><span data-stu-id="39511-164">Continue to access domain-joined apps and devices</span></span>

<span data-ttu-id="39511-165">Hvis du vil fortsette å få tilgang til domenetilknyttede programmer og enheter, kan du lese følgende artikler for to forskjellige måter for å aktivere som:</span><span class="sxs-lookup"><span data-stu-id="39511-165">If you want to continue to access domain-joined apps and devices, read the following articles for two different way of enabling that:</span></span>
  
- [<span data-ttu-id="39511-166">Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="39511-166">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>](manage-windows-devices.md)
    - <span data-ttu-id="39511-167">Dette er den anbefalte måten.</span><span class="sxs-lookup"><span data-stu-id="39511-167">This is the recommended way.</span></span>

- [<span data-ttu-id="39511-168">Access lokale ressurser fra en Azure AD-koblet enheten i Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="39511-168">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>](access-resources.md)

### <a name="connect-your-domain"></a><span data-ttu-id="39511-169">Koble til domenet ditt</span><span class="sxs-lookup"><span data-stu-id="39511-169">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="39511-170">Hvis du velger å bruke .onmicrosoft-domene, eller brukt Azure AD-tilkobling til å definere brukere, vil du ikke se dette trinnet.</span><span class="sxs-lookup"><span data-stu-id="39511-170">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="39511-171">Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.</span><span class="sxs-lookup"><span data-stu-id="39511-171">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="39511-172">Oppsettsveiviseren oppdager vanligvis registratoren og gir deg en kobling til trinnvise instruksjoner for hvordan du oppdaterer NS-postene på nettstedet til registratoren.</span><span class="sxs-lookup"><span data-stu-id="39511-172">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="39511-173">Hvis ikke, [Endre nameservers for å konfigurere Office 365 med en hvilken som helst domeneregistrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="39511-173">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="39511-174">Hvis du har eksisterende DNS-poster, for eksempel et eksisterende webområde, vil du håndtere dine egne DNS-poster for å kontrollere eksisterende tjenester forbli tilkoblet.</span><span class="sxs-lookup"><span data-stu-id="39511-174">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="39511-175">Se [Grunnleggende om domenet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="39511-175">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Koble ditt domene-siden med jeg skal behandle mine egne DNS-poster.](media/connectyourdomainpage.png)

2. <span data-ttu-id="39511-177">Følg trinnene i veiviseren, og e-post og andre tjenester vil bli satt opp for deg.</span><span class="sxs-lookup"><span data-stu-id="39511-177">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="39511-178">Konfigurere sikkerhetspolicyer og enheten konfigurasjoner</span><span class="sxs-lookup"><span data-stu-id="39511-178">Set up security policies and device configurations</span></span> 

<span data-ttu-id="39511-179">Disse policyene gjelder for hver bruker du gi en lisens til, eller til en gruppe brukere hvis du vil tilordne forskjellige policyer til et sett med brukere.</span><span class="sxs-lookup"><span data-stu-id="39511-179">These policies apply to every user you give a license to, or to a group of users if you decide to assign different policies to a set of users.</span></span>

#### <a name="set-up-policies-in-the-wizard"></a><span data-ttu-id="39511-180">Definer policyer i veiviseren</span><span class="sxs-lookup"><span data-stu-id="39511-180">Set up policies in the wizard</span></span>

<span data-ttu-id="39511-181">Policyer som er definert i veiviseren brukes automatisk på en [sikkerhetsgruppe](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) kalt *Alle brukere*.</span><span class="sxs-lookup"><span data-stu-id="39511-181">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span>

1. <span data-ttu-id="39511-182">Du **beskytte filene arbeid på mobile enheter** alternativet er **Beskytt arbeidsfiler når enhetene mistes eller stjeles** valgt som standard.</span><span class="sxs-lookup"><span data-stu-id="39511-182">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="39511-183">Du har et alternativ for å aktivere **styre hvordan brukere får tilgang til Office-filer på mobile enheter**, og dette anbefales.</span><span class="sxs-lookup"><span data-stu-id="39511-183">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Skjermbilde av beskytte arbeidsfiler på mobile enheter-siden.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="39511-185">Hvis du utvider **Beskytt arbeidsfiler når enhetene mistes eller blir stjålet**, [standardverdier](protect-work-files-on-lost-or-stolen-device.md) , er forhåndsvalgt:</span><span class="sxs-lookup"><span data-stu-id="39511-185">If you expand **Protect work files when devices are lost or stolen**, the [default values](protect-work-files-on-lost-or-stolen-device.md) are pre-selected:</span></span>

        ![Skjermbilde av standardverdier for å beskytte filer på tapt enheter.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="39511-187">Hvis du velger å **Behandle hvordan brukere får tilgang til Office-filer på mobile enheter** og utvide den, vises [standardverdiene](manage-user-access-on-mobile-devices.md) .</span><span class="sxs-lookup"><span data-stu-id="39511-187">If you select **Manage how users access Office files on mobile devices** and expand it, the [default values](manage-user-access-on-mobile-devices.md) are shown.</span></span> <span data-ttu-id="39511-188">Vi anbefaler at du godtar standardverdiene under konfigurasjonen for å opprette programpolicyer for Android, iOS og Windows 10 som gjelder for alle brukere.</span><span class="sxs-lookup"><span data-stu-id="39511-188">We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="39511-189">Du kan opprette flere policyer når konfigurasjonen er fullført.</span><span class="sxs-lookup"><span data-stu-id="39511-189">You can create more policies after setup completes.</span></span>

        ![Skjermbilde av beskyttelsesinnstillingene for Office-filer på mobile.](media/useraccessonmobile.png)

2. <span data-ttu-id="39511-191">Det siste trinnet på beskytte data og enheter, kan du definere policyer for å sikre Windows 10 enheter.</span><span class="sxs-lookup"><span data-stu-id="39511-191">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="39511-192">Disse innstillingene brukes automatisk når en bruker Windows 10 kobler seg til organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="39511-192">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="39511-193">Du kan utvide **sikre Windows 10 enheter** for å vise og endre [standardverdiene](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="39511-193">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="39511-194">Du kan også velge å [automatisk installere Office](install-office-on-windows-10-during-setup.md) på Windows 10 enheter.</span><span class="sxs-lookup"><span data-stu-id="39511-194">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Skjermbilde av satt Windows 10 konfigurasjonssiden for enheten.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a><span data-ttu-id="39511-196">Endre eller legge til policyer i administrasjonssenteret</span><span class="sxs-lookup"><span data-stu-id="39511-196">Modify or add policies in the admin center</span></span>

<span data-ttu-id="39511-197">Se [Behandle Microsoft 365 Business](manage.md) for koblinger til emner om hvordan du kan vise og endre beskyttelse enheten og app-policyer, og hvordan du kan fjerne data fra, eller tilbakestille Brukerenheter.</span><span class="sxs-lookup"><span data-stu-id="39511-197">See [manage Microsoft 365 Business](manage.md) for links to topics on how to view and modify device and app protection polices, and how to remove data from, or reset user devices.</span></span>

## <a name="deploy-and-manage-windows-10"></a><span data-ttu-id="39511-198">Distribuere og administrere Windows 10</span><span class="sxs-lookup"><span data-stu-id="39511-198">Deploy and manage Windows 10</span></span>
<span data-ttu-id="39511-199">Se [konfigurere Windows-enheter for Microsoft 365 Business brukere](set-up-windows-devices.md) koble til Azure AD, enten under installasjonen for nye datamaskiner, eller ved å endre e-postadressen for eksisterende datamaskiner manuelt.</span><span class="sxs-lookup"><span data-stu-id="39511-199">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) to manually connect to Azure AD, either during setup for new computers, or by changing sign-in profile for existing computers.</span></span> 

### <a name="use-autopilot-to-set-up-new-devices"></a><span data-ttu-id="39511-200">Bruk Autopilot til å definere nye enheter</span><span class="sxs-lookup"><span data-stu-id="39511-200">Use Autopilot to set up new devices</span></span>

<span data-ttu-id="39511-201">Du kan bruke [Windows Autopilot](add-autopilot-devices-and-profile.md) å automatisk forhåndskonfigurere **nye** Windows 10 enheter for en bruker, men det kan være enklere å få en [partner](https://www.microsoft.com/solution-providers/search) som kan gjøre dette for deg.</span><span class="sxs-lookup"><span data-stu-id="39511-201">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="39511-202">Du kan også gå til [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) og be om en sky teknologi ekspert definere nye enheter du kjøpe for deg.</span><span class="sxs-lookup"><span data-stu-id="39511-202">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

### <a name="access-on-premises-resources"></a><span data-ttu-id="39511-203">Få tilgang til lokale ressurser</span><span class="sxs-lookup"><span data-stu-id="39511-203">Access on-premises resources</span></span>

<span data-ttu-id="39511-204">Hvis organisasjonen bruker Windows Server Active Directory på lokaler, kan du definere Microsoft 365 Business til å beskytte Windows 10 enheter, samtidig som du har tilgang til lokale ressurser som krever lokal godkjenning.</span><span class="sxs-lookup"><span data-stu-id="39511-204">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="39511-205">Følg trinnene i [aktivere domenetilknyttede Windows 10 enheter som skal administreres av Microsoft 365 Business](manage-windows-devices.md) å sette opp dette.</span><span class="sxs-lookup"><span data-stu-id="39511-205">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="39511-206">Dette er den foretrukne metoden og enheter i denne tilstanden kalles Hybrid Azure AD koblet enheter.</span><span class="sxs-lookup"><span data-stu-id="39511-206">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

<span data-ttu-id="39511-207">Hvis firmaet har en lokal Active Directory, som inneholder noen lokale ressurser (for eksempel delte filer og skrivere), kan du gi din Azure AD-koblet enheter tilgang til disse ressursene ved å følge fremgangsmåten her: [Access lokale ressurser fra en Azure AD-koblet enheten i Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="39511-207">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="39511-208">Distribuere Office 365-klientprogrammer</span><span class="sxs-lookup"><span data-stu-id="39511-208">Deploy Office 365 client apps</span></span>

<span data-ttu-id="39511-209">Hvis du velger å installere Office-programmer i automatisk under settet opp, installerer apps på Windows 10-enheter når brukerne har logget på Azure AD fra deres Windows-enheter med legitimasjonen arbeid.</span><span class="sxs-lookup"><span data-stu-id="39511-209">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="39511-210">Hvis du vil installere Office på mobile iOS eller Android enheter, kan du se [definere mobile enheter for forretningsbrukere som Microsoft 365](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="39511-210">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="39511-211">Du kan også installere Office individuelt.</span><span class="sxs-lookup"><span data-stu-id="39511-211">You can also install Office individually.</span></span> <span data-ttu-id="39511-212">Se [installere Office på en PC eller Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for å få instruksjoner.</span><span class="sxs-lookup"><span data-stu-id="39511-212">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for instructions.</span></span>

## <a name="additional-security-settings"></a><span data-ttu-id="39511-213">Flere sikkerhetsinnstillinger</span><span class="sxs-lookup"><span data-stu-id="39511-213">Additional security settings</span></span>

<span data-ttu-id="39511-214">I tillegg til sikkerhet og overholdelse innstillingen i installasjonsveiviseren, kan du også angi følgende tilleggsinnstillinger:</span><span class="sxs-lookup"><span data-stu-id="39511-214">In addition to the security and compliance setting in the setup wizard, you can also set up the following additional settings:</span></span>
  
- <span data-ttu-id="39511-215">**Beskyttelse mot skadelig programvare for e-post**</span><span class="sxs-lookup"><span data-stu-id="39511-215">**Email malware protection**</span></span>
- <span data-ttu-id="39511-216">**Avanserte Threat Protection (ATP) trygt vedlegg**</span><span class="sxs-lookup"><span data-stu-id="39511-216">**Advanced Threat Protection (ATP) Safe Attachments**</span></span>
- <span data-ttu-id="39511-217">**ATP-klarerte koblinger**</span><span class="sxs-lookup"><span data-stu-id="39511-217">**ATP Safe Links**</span></span>
- <span data-ttu-id="39511-218">**PASSENDE anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="39511-218">**APT anti-phishing**</span></span>
- <span data-ttu-id="39511-219">**Exchange Online Archiving**</span><span class="sxs-lookup"><span data-stu-id="39511-219">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="39511-220">**Data tap forebygging (DLP)**</span><span class="sxs-lookup"><span data-stu-id="39511-220">**Data loss prevention (DLP)**</span></span>
- <span data-ttu-id="39511-221">**Azure informasjonsbeskyttelse** (Planlegge 1)</span><span class="sxs-lookup"><span data-stu-id="39511-221">**Azure Information Protection** (Plan 1)</span></span>
- <span data-ttu-id="39511-222">**Intune portal tilgjengelighet**</span><span class="sxs-lookup"><span data-stu-id="39511-222">**Intune portal availability**</span></span>

<span data-ttu-id="39511-223">Å komme i gang, kan du se [konfigurere avanserte sikkerhetspolicyer](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="39511-223">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

<span data-ttu-id="39511-224">Se også [topp 10 måter å sikre bedriften din Microsoft-365](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for et veikart for gode fremgangsmåter for sikkerhet.</span><span class="sxs-lookup"><span data-stu-id="39511-224">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>