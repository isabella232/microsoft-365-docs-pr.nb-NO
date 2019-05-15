---
title: Konfigurere Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
ms.openlocfilehash: 42a35810531b6abd5b22e5fdbce2c0cfea57b8d7
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074594"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="b6590-103">Definere Microsoft 365 Business i installasjonsveiviseren for</span><span class="sxs-lookup"><span data-stu-id="b6590-103">Set up Microsoft 365 Business in the setup wizard</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="b6590-104">Legge til domenet, brukere, og konfigurere policyer</span><span class="sxs-lookup"><span data-stu-id="b6590-104">Add your domain, users, and set up policies</span></span>

![Banner som peker til https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="b6590-106">Når du kjøper Microsoft 365 Business, har du muligheten til å bruke et domene du eier, eller kjøpe en i løpet av [registreringen](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="b6590-106">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="b6590-107">Hvis du har kjøpt et nytt domene når du registrerte deg, domenet er alle satt opp, og du kan flytte for å [legge til brukere og tilordne lisenser](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="b6590-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="b6590-108">Legge til domenet for å tilpasse pålogging</span><span class="sxs-lookup"><span data-stu-id="b6590-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="b6590-109">Logg på [administrasjonssenteret for Microsoft 365](https://admin.microsoft.com) ved hjelp av global admin-rettigheter.</span><span class="sxs-lookup"><span data-stu-id="b6590-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="b6590-110">Velg **Legg til et domene** eller **legge til brukere** for å starte veiviseren.</span><span class="sxs-lookup"><span data-stu-id="b6590-110">Choose **Add a domain** or **Add users** to start the wizard.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="b6590-111">Hvis du har kjøpt et domene under registreringen, vil du ikke se **legge til et domene** trinn her.</span><span class="sxs-lookup"><span data-stu-id="b6590-111">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="b6590-112">Gå til [Legg til brukere](#add-users-and-assign-licenses) i stedet.</span><span class="sxs-lookup"><span data-stu-id="b6590-112">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Velg Legg til et domene.](media/addadomainadmincenter.png)
    
3. <span data-ttu-id="b6590-114">I veiviseren angir du navnet på domenet du vil bruke (for eksempel contoso.com).</span><span class="sxs-lookup"><span data-stu-id="b6590-114">In the wizard, enter the domain name you want to use (like contoso.com).</span></span>


    ![Skjermbilde av Tilpass på siden.](media/personalizesignin.png)

    
4. <span data-ttu-id="b6590-116">Følg trinnene i veiviseren til å [opprette DNS-poster på alle DNS-vertsleverandøren for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , som bekrefter at du eier domenet.</span><span class="sxs-lookup"><span data-stu-id="b6590-116">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="b6590-117">Hvis du kjenner ditt domene host, se også [vert for spesifikke instruksjoner](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="b6590-117">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="b6590-118">Hvis din vertsleverandøren er GoDaddy, prosessen er enkelt, og du blir automatisk bedt om å logge på og la Microsoft godkjenne på dine vegne:</span><span class="sxs-lookup"><span data-stu-id="b6590-118">If your hosting provider is GoDaddy, the process is easy and you will be automatically asked to sign in and let Microsoft authenticate on your behalf:</span></span>

    ![Velg Godkjenn på GoDaddy bekrefte tilgang-siden.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="b6590-120">Legge til brukere og tilordne lisenser</span><span class="sxs-lookup"><span data-stu-id="b6590-120">Add users and assign licenses</span></span>

<span data-ttu-id="b6590-121">Du kan legge til brukere i veiviseren, men du kan også [legge til senere brukere](add-users-m365b.md) i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="b6590-121">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="b6590-122">Hvis du har en lokal domenekontroller, kan du i tillegg legge til brukere med [Azure AD-tilkobling](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="b6590-122">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="b6590-123">Legge til brukere i veiviseren</span><span class="sxs-lookup"><span data-stu-id="b6590-123">Add users in the wizard</span></span>

<span data-ttu-id="b6590-124">Eventuelle brukere du legger til i veiviseren Hent automatisk tilordnet en lisens for Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="b6590-124">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Skjermbilde av siden Legg til nye brukere i veiviseren](media/addnewuserspage.png)

1. <span data-ttu-id="b6590-126">Hvis abonnementet på Microsoft 365 Business har eksisterende brukere (for eksempel, hvis du brukte Azure AD-tilkobling), får du et alternativ for å tilordne lisenser til dem nå.</span><span class="sxs-lookup"><span data-stu-id="b6590-126">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you get an option to assign licenses to them now.</span></span> <span data-ttu-id="b6590-127">Gå videre og legg til lisenser for dem også.</span><span class="sxs-lookup"><span data-stu-id="b6590-127">Go ahead and add licenses to them as well.</span></span>

3. <span data-ttu-id="b6590-128">Når du har lagt til brukerne, får du også muligheten til å dele legitimasjon med de nye brukerne du har lagt til.</span><span class="sxs-lookup"><span data-stu-id="b6590-128">After you have added the users, you will also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="b6590-129">Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.</span><span class="sxs-lookup"><span data-stu-id="b6590-129">You can choose to print them out, email them, or download them.</span></span>

4. <span data-ttu-id="b6590-130">Hopp over overføring av e-postmeldinger, og velg **Neste** på **Overfør e-postmeldinger**-siden.</span><span class="sxs-lookup"><span data-stu-id="b6590-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 

    <span data-ttu-id="b6590-131">Hvis du flytter fra en annen leverandør av e-post og vil kopiere dataene senere, kan du [Overfør e-post og kontakter til Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="b6590-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>


### <a name="connect-your-domain"></a><span data-ttu-id="b6590-132">Koble til domenet ditt</span><span class="sxs-lookup"><span data-stu-id="b6590-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="b6590-133">Hvis du velger å bruke .onmicrosoft-domene, eller brukt Azure AD-tilkobling til å definere brukere, vil du ikke se dette trinnet.</span><span class="sxs-lookup"><span data-stu-id="b6590-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="b6590-134">Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.</span><span class="sxs-lookup"><span data-stu-id="b6590-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="b6590-135">Oppsettsveiviseren oppdager vanligvis registratoren og gir deg en kobling til trinnvise instruksjoner for hvordan du oppdaterer NS-postene på nettstedet til registratoren.</span><span class="sxs-lookup"><span data-stu-id="b6590-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="b6590-136">Hvis ikke, [Endre nameservers for å konfigurere Office 365 med en hvilken som helst domeneregistrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="b6590-136">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="b6590-137">Hvis du har eksisterende DNS-poster, for eksempel et eksisterende webområde, vil du håndtere dine egne DNS-poster for å kontrollere eksisterende tjenester forbli tilkoblet.</span><span class="sxs-lookup"><span data-stu-id="b6590-137">If you have existing DNS records, for example an existing web site, you will want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="b6590-138">Se [Grunnleggende om domenet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="b6590-138">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Koble ditt domene-siden med jeg skal behandle mine egne DNS-poster.](media/connectyourdomainpage.png)

2. <span data-ttu-id="b6590-140">Følg trinnene i veiviseren, og e-post og andre tjenester vil bli satt opp for deg.</span><span class="sxs-lookup"><span data-stu-id="b6590-140">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="set-up-security-policies-and-device-configurations"></a><span data-ttu-id="b6590-141">Konfigurere sikkerhetspolicyer og enheten konfigurasjoner</span><span class="sxs-lookup"><span data-stu-id="b6590-141">Set up security policies and device configurations</span></span> 

<span data-ttu-id="b6590-142">Policyer som er definert i veiviseren brukes automatisk på en [sikkerhetsgruppe](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) kalt *Alle brukere*.</span><span class="sxs-lookup"><span data-stu-id="b6590-142">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="b6590-143">Du kan også opprette flere grupper du tilordner policyer til i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="b6590-143">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="b6590-144">Du **beskytte filene arbeid på mobile enheter** alternativet er **Beskytt arbeidsfiler når enhetene mistes eller stjeles** valgt som standard.</span><span class="sxs-lookup"><span data-stu-id="b6590-144">On the **Protect your work files on mobile devices** the option **Protect work files when devices are lost or stolen** is selected by default.</span></span> <span data-ttu-id="b6590-145">Du har et alternativ for å aktivere **styre hvordan brukere får tilgang til Office-filer på mobile enheter**, og dette anbefales.</span><span class="sxs-lookup"><span data-stu-id="b6590-145">You have an option to turn on **Manage how users access Office files on mobile devices**, and this is recommended.</span></span>

    ![Skjermbilde av beskytte arbeidsfiler på mobile enheter-siden.](media/protectworkfilesondevices.png)

     - <span data-ttu-id="b6590-147">Utvid **Beskytt arbeidsfiler når enhetene mistes eller blir stjålet** for å vise [standardverdier](protect-work-files-on-lost-or-stolen-device.md):</span><span class="sxs-lookup"><span data-stu-id="b6590-147">Expand **Protect work files when devices are lost or stolen** to display the [default values](protect-work-files-on-lost-or-stolen-device.md):</span></span>

        ![Skjermbilde av standardverdier for å beskytte filer på tapt enheter.](media/protectworkfilesondevicesdefault.png)

    - <span data-ttu-id="b6590-149">Velg **Behandle hvordan brukere får tilgang til Office-filer på mobile enheter** , og utvid den for å vise [standardverdier](manage-user-access-on-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="b6590-149">Select **Manage how users access Office files on mobile devices** and expand it to display the [default values](manage-user-access-on-mobile-devices.md).</span></span> <span data-ttu-id="b6590-150">Vi anbefaler at du godta standardverdiene under opprette programpolicyer for Android, iOS og 10 for Windows-installasjonen som gjelder for alle brukere.</span><span class="sxs-lookup"><span data-stu-id="b6590-150">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="b6590-151">Du kan opprette flere policyer når konfigurasjonen er fullført.</span><span class="sxs-lookup"><span data-stu-id="b6590-151">You can create more policies after setup completes.</span></span>

        ![Skjermbilde av beskyttelsesinnstillingene for Office-filer på mobile.](media/useraccessonmobile.png)

2. <span data-ttu-id="b6590-153">Det siste trinnet på beskytte data og enheter, kan du definere policyer for å sikre Windows 10 enheter.</span><span class="sxs-lookup"><span data-stu-id="b6590-153">The last step on protect data and devices allows you to set up policies to secure Windows 10 devices.</span></span> <span data-ttu-id="b6590-154">Disse innstillingene brukes automatisk når en bruker Windows 10 kobler seg til organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="b6590-154">These settings are applied automatically when a user's Windows 10 connects to your organization.</span></span> <span data-ttu-id="b6590-155">Du kan utvide **sikre Windows 10 enheter** for å vise og endre [standardverdiene](secure-windows-10-devices.md).</span><span class="sxs-lookup"><span data-stu-id="b6590-155">You can expand **Secure Windows 10 devices** to see and modify the [default values](secure-windows-10-devices.md).</span></span>
3. <span data-ttu-id="b6590-156">Du kan også velge å [automatisk installere Office](install-office-on-windows-10-during-setup.md) på Windows 10 enheter.</span><span class="sxs-lookup"><span data-stu-id="b6590-156">You can also choose to [automatically install Office](install-office-on-windows-10-during-setup.md) on Windows 10 devices.</span></span>

    ![Skjermbilde av satt Windows 10 konfigurasjonssiden for enheten.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="b6590-158">Distribuere Office 365-klientprogrammer</span><span class="sxs-lookup"><span data-stu-id="b6590-158">Deploy Office 365 client apps</span></span>

<span data-ttu-id="b6590-159">Hvis du velger å installere Office-programmer i automatisk under settet opp, installerer apps på Windows 10-enheter når brukerne har logget på Azure AD fra deres Windows-enheter med legitimasjonen arbeid.</span><span class="sxs-lookup"><span data-stu-id="b6590-159">If you chose to automatically install Office apps in during the set up, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices with their work credentials.</span></span>
<span data-ttu-id="b6590-160">Hvis du vil installere Office på mobile iOS eller Android enheter, kan du se [definere mobile enheter for forretningsbrukere som Microsoft 365](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="b6590-160">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="b6590-161">Du kan også installere Office individuelt.</span><span class="sxs-lookup"><span data-stu-id="b6590-161">You can also install Office individually.</span></span> <span data-ttu-id="b6590-162">Se [installere Office på en PC eller Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for å få instruksjoner.</span><span class="sxs-lookup"><span data-stu-id="b6590-162">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for instructions.</span></span>
