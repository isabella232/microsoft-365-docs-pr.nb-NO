---
title: Konfigurere Microsoft 365 Business Premium
f1.keywords:
- NOCSH
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
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Oppdag installasjonstrinnene for Microsoft 365 Business Premium, inkludert å legge til et domene og brukere, konfigurere sikkerhetspolicyer og mer.
ms.openlocfilehash: efa7934ece0dfeac3c4b20daa37da6f1160901e7
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081899"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="827b8-103">Konfigurere Microsoft 365 Business Premium i installasjonsveiviseren</span><span class="sxs-lookup"><span data-stu-id="827b8-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="827b8-104">Se denne videoen for å få en oversikt over Microsoft 365 Business Premium-oppsett.</span><span class="sxs-lookup"><span data-stu-id="827b8-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

<span data-ttu-id="827b8-105">Hvis du synes at denne videoen er nyttig, kan du se den [fullstendige opplæringsserien for små bedrifter og de som er nybegynnere i Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="827b8-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="827b8-106">Legge til domene- og bruker- og konfigureringspolicyer</span><span class="sxs-lookup"><span data-stu-id="827b8-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="827b8-107">Når du kjøper Microsoft 365 Business Premium, kan du bruke et domene du eier, eller kjøpe et under [registreringen](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="827b8-107">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="827b8-108">Hvis du kjøpte et nytt domene da du registrerte deg, er domenet konfigurert, og du kan flytte til [Legg til brukere og tilordne lisenser](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="827b8-108">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="827b8-109">Legg til domenet for å tilpasse påloggingen</span><span class="sxs-lookup"><span data-stu-id="827b8-109">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="827b8-110">Logg på [administrasjonssenteret for Microsoft 365](https://admin.microsoft.com) ved hjelp av den globale administratorlegitimasjonen.</span><span class="sxs-lookup"><span data-stu-id="827b8-110">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="827b8-111">Velg **Gå til oppsett** for å starte veiviseren.</span><span class="sxs-lookup"><span data-stu-id="827b8-111">Choose **Go to setup** to start the wizard.</span></span>

    ![Velg Gå til oppsett.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="827b8-113">På siden **Installer Office-apper** kan du installere appene på din egen datamaskin.</span><span class="sxs-lookup"><span data-stu-id="827b8-113">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="827b8-114">Skriv inn domenenavnet du vil bruke (for eksempel contoso.com) i trinnet Legg til **domene.**</span><span class="sxs-lookup"><span data-stu-id="827b8-114">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="827b8-115">Hvis du kjøpte et domene under registreringen, vil du ikke se **Legg til et domenetrinn** her.</span><span class="sxs-lookup"><span data-stu-id="827b8-115">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="827b8-116">Gå til [Legg til brukere](#add-users-and-assign-licenses) i stedet.</span><span class="sxs-lookup"><span data-stu-id="827b8-116">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Skjermbilde av påmeldingssiden For å tilpasse påloggingssiden.](../media/adddomain.png)

    
4. <span data-ttu-id="827b8-118">Følg trinnene i veiviseren for å [opprette DNS-poster hos en DNS-vertsleverandør for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) som bekrefter at du eier domenet.</span><span class="sxs-lookup"><span data-stu-id="827b8-118">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="827b8-119">Hvis du kjenner domeneverten din, kan du også se [vertsspesifikke instruksjoner](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="827b8-119">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="827b8-120">Hvis vertsleverandøren er GoDaddy eller en annen vert aktivert med [domenetilkobling,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)er prosessen enkel, og du blir automatisk bedt om å logge på og la Microsoft godkjenne på dine vegne.</span><span class="sxs-lookup"><span data-stu-id="827b8-120">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Velg Autoriser på GoDaddy Confirm Access-siden.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="827b8-122">Legge til brukere og tilordne lisenser</span><span class="sxs-lookup"><span data-stu-id="827b8-122">Add users and assign licenses</span></span>

<span data-ttu-id="827b8-123">Du kan legge til brukere i veiviseren, men du kan også [legge til brukere senere](add-users-m365b.md) i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="827b8-123">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="827b8-124">I tillegg, hvis du har en lokal domenekontroller, kan du legge til brukere med [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="827b8-124">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="827b8-125">Legge til brukere i veiviseren</span><span class="sxs-lookup"><span data-stu-id="827b8-125">Add users in the wizard</span></span>

<span data-ttu-id="827b8-126">Alle brukere du legger til i veiviseren, tilordnes automatisk en Microsoft 365 Business Premium-lisens.</span><span class="sxs-lookup"><span data-stu-id="827b8-126">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Skjermbilde av siden Legg til nye brukere i veiviseren](../media/addnewuserspage.png)

1. <span data-ttu-id="827b8-128">Hvis Microsoft 365 Business Premium-abonnementet har eksisterende brukere (for eksempel hvis du brukte Azure AD Connect), får du muligheten til å tilordne lisenser til dem nå.</span><span class="sxs-lookup"><span data-stu-id="827b8-128">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="827b8-129">Gå videre og legg til lisenser for dem også.</span><span class="sxs-lookup"><span data-stu-id="827b8-129">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="827b8-130">Når du har lagt til brukerne, får du også et alternativ for å dele legitimasjon med de nye brukerne du har lagt til.</span><span class="sxs-lookup"><span data-stu-id="827b8-130">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="827b8-131">Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.</span><span class="sxs-lookup"><span data-stu-id="827b8-131">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="827b8-132">Koble til domenet ditt</span><span class="sxs-lookup"><span data-stu-id="827b8-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="827b8-133">Hvis du valgte å bruke .onmicrosoft-domenet, eller brukte Azure AD Connect til å konfigurere brukere, vil du ikke se dette trinnet.</span><span class="sxs-lookup"><span data-stu-id="827b8-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="827b8-134">Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.</span><span class="sxs-lookup"><span data-stu-id="827b8-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="827b8-135">Oppsettsveiviseren oppdager vanligvis registratoren og gir deg en kobling til trinnvise instruksjoner for hvordan du oppdaterer NS-postene på nettstedet til registratoren.</span><span class="sxs-lookup"><span data-stu-id="827b8-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="827b8-136">Hvis den ikke gjør det, [endrer du navneservere for å konfigurere Microsoft 365 med en domeneregistrator](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span><span class="sxs-lookup"><span data-stu-id="827b8-136">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span></span> 

    - <span data-ttu-id="827b8-137">Hvis du har eksisterende DNS-poster, for eksempel et eksisterende webområde, men DNS-verten er aktivert for [domenetilkobling](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), velger du **Legg til poster for meg**.</span><span class="sxs-lookup"><span data-stu-id="827b8-137">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="827b8-138">Godta alle **standardinnstillingene på** siden Velg elektroniske tjenester, og velg **Neste**, og velg **Autoriser** på DNS-vertens side.</span><span class="sxs-lookup"><span data-stu-id="827b8-138">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="827b8-139">Hvis du har eksisterende DNS-poster med andre DNS-verter (ikke aktivert for domenetilkobling), bør du administrere dine egne DNS-poster for å sikre at de eksisterende tjenestene forblir tilkoblet.</span><span class="sxs-lookup"><span data-stu-id="827b8-139">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="827b8-140">Se [grunnleggende domene for](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="827b8-140">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Aktivere poster-siden.](../media/activaterecords.png)

2. <span data-ttu-id="827b8-142">Følg trinnene i veiviseren og e-post og andre tjenester vil bli satt opp for deg.</span><span class="sxs-lookup"><span data-stu-id="827b8-142">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="827b8-143">Beskytt organisasjonen</span><span class="sxs-lookup"><span data-stu-id="827b8-143">Protect your organization</span></span> 

<span data-ttu-id="827b8-144">Policyene du definerer i veiviseren, brukes automatisk på en [sikkerhetsgruppe](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) kalt *Alle brukere*.</span><span class="sxs-lookup"><span data-stu-id="827b8-144">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="827b8-145">Du kan også opprette flere grupper du vil tilordne policyer til i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="827b8-145">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="827b8-146">På **øk beskyttelse mot avanserte cybertrusler**anbefales det at du godtar standardinnstillingene for å la [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) skanne filer og koblinger i Office-apper.</span><span class="sxs-lookup"><span data-stu-id="827b8-146">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Skjermbilde av Øk beskyttelsessiden.](../media/increasetreatprotection.png)


2. <span data-ttu-id="827b8-148">På siden **Forhindre lekkasjer av sensitive data** godtar du standardinnstillingene for å aktivere Office 365 Data Loss Prevention (DLP) for å spore sensitive data i Office-apper og forhindre utilsiktet deling av disse utenfor organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="827b8-148">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="827b8-149">La administrasjon av mobilapper være på siden **Beskytt data i Office for mobil,** utvid innstillingene og se gjennom dem, og velg deretter **Opprett policy for administrasjon av mobilapper**.</span><span class="sxs-lookup"><span data-stu-id="827b8-149">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Skjermbilde av Beskytt data på Office for mobil.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="827b8-151">Sikre Pc-er med Windows 10</span><span class="sxs-lookup"><span data-stu-id="827b8-151">Secure Windows 10 PCs</span></span>

<span data-ttu-id="827b8-152">Velg **Oppsett** i venstre navigasjonsrute, og velg deretter **Sikre Windows 10-datamaskinene**under **Pålogging og sikkerhet**.</span><span class="sxs-lookup"><span data-stu-id="827b8-152">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="827b8-153">Velg **Vis** for å komme i gang.</span><span class="sxs-lookup"><span data-stu-id="827b8-153">Choose **View** to get started.</span></span> <span data-ttu-id="827b8-154">Se [sikre Windows 10-datamaskinene for](secure-win-10-pcs.md) fullstendige instruksjoner.</span><span class="sxs-lookup"><span data-stu-id="827b8-154">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="827b8-155">Distribuere Office 365-klientapper</span><span class="sxs-lookup"><span data-stu-id="827b8-155">Deploy Office 365 client apps</span></span>

<span data-ttu-id="827b8-156">Hvis du velger å installere Office-apper automatisk under installasjonen, installeres appene på Windows 10-enhetene når brukerne har logget på Azure AD fra Windows-enhetene sine, ved hjelp av arbeidslegitimasjonen.</span><span class="sxs-lookup"><span data-stu-id="827b8-156">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="827b8-157">Hvis du vil installere Office på mobile iOS- eller Android-enheter, kan du se [Konfigurere mobile enheter for Microsoft 365 Business Premium-brukere](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="827b8-157">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="827b8-158">Du kan også installere Office individuelt.</span><span class="sxs-lookup"><span data-stu-id="827b8-158">You can also install Office individually.</span></span> <span data-ttu-id="827b8-159">Se [installere Office på en PC eller Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instruksjoner.</span><span class="sxs-lookup"><span data-stu-id="827b8-159">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="827b8-160">Se også</span><span class="sxs-lookup"><span data-stu-id="827b8-160">See also</span></span>

[<span data-ttu-id="827b8-161">Opplæringsvideoer for Microsoft 365 for bedrifter</span><span class="sxs-lookup"><span data-stu-id="827b8-161">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
