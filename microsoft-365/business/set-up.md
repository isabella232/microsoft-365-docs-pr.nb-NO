---
title: Konfigurere Microsoft 365 Business
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Oppdag konfigurasjonstrinnene for Microsoft 365 Business, inkludert å legge til et domene og brukere, konfigurere sikkerhetspolicyer og mer.
ms.openlocfilehash: 4535a32b579b91b6c2bb0e64ec95904be6c08fce
ms.sourcegitcommit: 6c8edbc54b193e964cf93aec48c51cb79231f1d9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2020
ms.locfileid: "42543943"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a><span data-ttu-id="58a45-103">Konfigurere Microsoft 365 Business i installasjonsveiviseren</span><span class="sxs-lookup"><span data-stu-id="58a45-103">Set up Microsoft 365 Business in the setup wizard</span></span>

<span data-ttu-id="58a45-104">Se denne videoen for å få en oversikt over installasjonsprogrammet for Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="58a45-104">Watch this video for an overview of Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

<span data-ttu-id="58a45-105">Hvis du synes at denne videoen er nyttig, kan du se den [fullstendige opplæringsserien for små bedrifter og de som er nybegynnere i Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="58a45-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="58a45-106">Legge til domene, brukere og konfigurere policyer</span><span class="sxs-lookup"><span data-stu-id="58a45-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="58a45-107">[![Etikett for å gi deg beskjed om at administrasjonssenteret endres. Du finner mer informasjon på aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="58a45-107">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="58a45-108">Når du kjøper Microsoft 365 Business, har du muligheten til å bruke et domene du eier, eller kjøpe et under [registreringen](sign-up.md).</span><span class="sxs-lookup"><span data-stu-id="58a45-108">When you purchase Microsoft 365 Business, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="58a45-109">Hvis du kjøpte et nytt domene da du registrerte deg, er domenet konfigurert, og du kan flytte til [Legg til brukere og tilordne lisenser](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="58a45-109">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="58a45-110">Legge til domenet ditt for å tilpasse påloggingen</span><span class="sxs-lookup"><span data-stu-id="58a45-110">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="58a45-111">Logg på [administrasjonssenteret for Microsoft 365](https://admin.microsoft.com) ved hjelp av den globale administratorlegitimasjonen.</span><span class="sxs-lookup"><span data-stu-id="58a45-111">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="58a45-112">Velg **Gå til oppsett** for å starte veiviseren.</span><span class="sxs-lookup"><span data-stu-id="58a45-112">Choose **Go to setup** to start the wizard.</span></span>

    ![Velg Gå til oppsett.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="58a45-114">På siden **Installer Office-apper** kan du eventuelt installere appene på din egen datamaskin.</span><span class="sxs-lookup"><span data-stu-id="58a45-114">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="58a45-115">Skriv inn domenenavnet du vil bruke (for eksempel contoso.com) i trinnet Legg til **domene.**</span><span class="sxs-lookup"><span data-stu-id="58a45-115">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="58a45-116">Hvis du kjøpte et domene under registreringen, ser du ikke **Legge til et domenetrinn** her.</span><span class="sxs-lookup"><span data-stu-id="58a45-116">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="58a45-117">Gå til [Legg til brukere](#add-users-and-assign-licenses) i stedet.</span><span class="sxs-lookup"><span data-stu-id="58a45-117">Go to [Add users ](#add-users-and-assign-licenses) instead.</span></span>

    ![Skjermbilde av siden Tilpass påloggingssiden.](../media/adddomain.png)

    
4. <span data-ttu-id="58a45-119">Følg trinnene i veiviseren for å [opprette DNS-poster hos en DNS-vertsleverandør for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) som bekrefter at du eier domenet.</span><span class="sxs-lookup"><span data-stu-id="58a45-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="58a45-120">Hvis du kjenner domeneverten, kan du se også [vertsspesifikke instruksjoner](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span><span class="sxs-lookup"><span data-stu-id="58a45-120">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="58a45-121">Hvis vertsleverandøren din er GoDaddy eller en annen vert aktivert med [domenetilkobling,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)er prosessen enkel, og du blir automatisk bedt om å logge på og la Microsoft godkjenne på dine vegne.</span><span class="sxs-lookup"><span data-stu-id="58a45-121">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Velg Godkjenn på Siden Bekreft tilgang til GoDaddy Bekrefter tilgang.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="58a45-123">Legge til brukere og tilordne lisenser</span><span class="sxs-lookup"><span data-stu-id="58a45-123">Add users and assign licenses</span></span>

<span data-ttu-id="58a45-124">Du kan legge til brukere i veiviseren, men du kan også [legge til brukere senere](add-users-m365b.md) i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="58a45-124">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="58a45-125">I tillegg, hvis du har en lokal domenekontroller, kan du legge til brukere med [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="58a45-125">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="58a45-126">Legge til brukere i veiviseren</span><span class="sxs-lookup"><span data-stu-id="58a45-126">Add users in the wizard</span></span>

<span data-ttu-id="58a45-127">Alle brukere du legger til i veiviseren, tilordnes automatisk en Microsoft 365 Business-lisens.</span><span class="sxs-lookup"><span data-stu-id="58a45-127">Any users you add in the wizard get automatically assigned a Microsoft 365 Business license.</span></span>

![Skjermbilde av siden Legg til nye brukere i veiviseren](../media/addnewuserspage.png)

1. <span data-ttu-id="58a45-129">Hvis Microsoft 365 Business-abonnementet har eksisterende brukere (for eksempel hvis du brukte Azure AD Connect), får du et alternativ for å tilordne lisenser til dem nå.</span><span class="sxs-lookup"><span data-stu-id="58a45-129">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="58a45-130">Gå videre og legg til lisenser for dem også.</span><span class="sxs-lookup"><span data-stu-id="58a45-130">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="58a45-131">Når du har lagt til brukerne, får du også et alternativ for å dele legitimasjon med de nye brukerne du har lagt til.</span><span class="sxs-lookup"><span data-stu-id="58a45-131">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="58a45-132">Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.</span><span class="sxs-lookup"><span data-stu-id="58a45-132">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="58a45-133">Koble til domenet ditt</span><span class="sxs-lookup"><span data-stu-id="58a45-133">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="58a45-134">Hvis du valgte å bruke .onmicrosoft-domenet eller brukt Azure AD Connect til å konfigurere brukere, vil du ikke se dette trinnet.</span><span class="sxs-lookup"><span data-stu-id="58a45-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="58a45-135">Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.</span><span class="sxs-lookup"><span data-stu-id="58a45-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="58a45-136">Oppsettsveiviseren oppdager vanligvis registratoren og gir deg en kobling til trinnvise instruksjoner for hvordan du oppdaterer NS-postene på nettstedet til registratoren.</span><span class="sxs-lookup"><span data-stu-id="58a45-136">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="58a45-137">Hvis det ikke gjør det, [kan du endre navneservere til å konfigurere Office 365 med en domeneregistrator](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="58a45-137">If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span> 

    - <span data-ttu-id="58a45-138">Hvis du har eksisterende DNS-poster, for eksempel et eksisterende webområde, men DNS-verten er aktivert for [domenetilkobling,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)velger du **Legg til poster for meg**.</span><span class="sxs-lookup"><span data-stu-id="58a45-138">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="58a45-139">Godta alle standardene på siden **Velg elektroniske tjenester,** og velg **Neste**, og velg **Godkjenn** på DNS-vertens side.</span><span class="sxs-lookup"><span data-stu-id="58a45-139">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="58a45-140">Hvis du har eksisterende DNS-poster med andre DNS-verter (ikke aktivert for domenetilkobling), vil du administrere dine egne DNS-poster for å sikre at de eksisterende tjenestene forblir tilkoblet.</span><span class="sxs-lookup"><span data-stu-id="58a45-140">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="58a45-141">Se [grunnleggende om domene](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="58a45-141">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Aktivere poster-siden.](../media/activaterecords.png)

2. <span data-ttu-id="58a45-143">Følg trinnene i veiviseren, og e-post og andre tjenester vil bli konfigurert for deg.</span><span class="sxs-lookup"><span data-stu-id="58a45-143">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="58a45-144">Beskytt organisasjonen</span><span class="sxs-lookup"><span data-stu-id="58a45-144">Protect your organization</span></span> 

<span data-ttu-id="58a45-145">Policyene du konfigurerte i veiviseren, brukes automatisk på en [sikkerhetsgruppe](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) kalt *Alle brukere*.</span><span class="sxs-lookup"><span data-stu-id="58a45-145">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="58a45-146">Du kan også opprette flere grupper for å tilordne policyer til i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="58a45-146">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="58a45-147">På **Øk beskyttelsen mot avanserte cybertrusler**anbefales det at du godtar standardinnstillingene for å la [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) skanne filer og koblinger i Office-apper.</span><span class="sxs-lookup"><span data-stu-id="58a45-147">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Skjermbilde av Siden Øk beskyttelse.](../media/increasetreatprotection.png)


2. <span data-ttu-id="58a45-149">På siden **Forhindre lekkasjer av sensitive data** godtar du standardinnstillingene for å aktivere Office 365 Data Loss Prevention (DLP) for å spore sensitive data i Office-apper og forhindre utilsiktet deling av disse utenfor organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="58a45-149">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="58a45-150">På siden **Beskytt data i Office for mobil** lar du administrasjon av mobilapper være på, utvide innstillingene og se gjennom dem, og velg deretter Opprett policy for administrasjon av **mobilapper**.</span><span class="sxs-lookup"><span data-stu-id="58a45-150">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Skjermbilde av Beskytt data på Office for mobilside.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="58a45-152">Sikre Windows 10-PCer</span><span class="sxs-lookup"><span data-stu-id="58a45-152">Secure Windows 10 PCs</span></span>

<span data-ttu-id="58a45-153">Velg **Oppsett** til venstre, og velg deretter **Sikre Windows 10-datamaskiner**under **Sing-in og sikkerhet**.</span><span class="sxs-lookup"><span data-stu-id="58a45-153">On the left nav, select **Setup** and then, under **Sing-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="58a45-154">Velg **Vis** for å komme i gang.</span><span class="sxs-lookup"><span data-stu-id="58a45-154">Choose **View** to get started.</span></span> <span data-ttu-id="58a45-155">Se [sikre Windows 10-datamaskinene](secure-win-10-pcs.md) for fullstendige instruksjoner.</span><span class="sxs-lookup"><span data-stu-id="58a45-155">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="58a45-156">Distribuere Office 365-klientapper</span><span class="sxs-lookup"><span data-stu-id="58a45-156">Deploy Office 365 client apps</span></span>

<span data-ttu-id="58a45-157">Hvis du velger å installere Office-apper automatisk under installasjonen, installeres appene på Windows 10-enhetene når brukerne har logget på Azure AD fra Windows-enhetene sine, ved hjelp av arbeidslegitimasjonen.</span><span class="sxs-lookup"><span data-stu-id="58a45-157">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="58a45-158">Hvis du vil installere Office på mobile iOS- eller Android-enheter, kan du se [Konfigurere mobile enheter for Microsoft 365 Business-brukere](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="58a45-158">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="58a45-159">Du kan også installere Office individuelt.</span><span class="sxs-lookup"><span data-stu-id="58a45-159">You can also install Office individually.</span></span> <span data-ttu-id="58a45-160">Se [installere Office på en PC eller Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instruksjoner.</span><span class="sxs-lookup"><span data-stu-id="58a45-160">See [install Office on a PC or Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="58a45-161">Se også</span><span class="sxs-lookup"><span data-stu-id="58a45-161">See also</span></span>

[<span data-ttu-id="58a45-162">Opplæringsvideoer for Microsoft 365-bedrifter</span><span class="sxs-lookup"><span data-stu-id="58a45-162">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
