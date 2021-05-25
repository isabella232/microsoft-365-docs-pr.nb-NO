---
title: Konfigurere Microsoft 365 Business Premium
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
description: Oppdag konfigurasjonstrinnene for Microsoft 365 Business Premium, inkludert å legge til et domene og brukere, konfigurere sikkerhetspolicyer og mer.
ms.openlocfilehash: 3e15f16db2a233d2e11d444600398102b075932d
ms.sourcegitcommit: 686f192e1a650ec805fe8e908b46ca51771ed41f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/24/2021
ms.locfileid: "52624393"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="8126c-103">Konfigurere Microsoft 365 Business Premium i konfigurasjonsveiviseren</span><span class="sxs-lookup"><span data-stu-id="8126c-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

## <a name="watch-overview-of-microsoft-365-setup"></a><span data-ttu-id="8126c-104">Se: Oversikt over Microsoft 365 oppsett</span><span class="sxs-lookup"><span data-stu-id="8126c-104">Watch: Overview of Microsoft 365 setup</span></span>

<span data-ttu-id="8126c-105">Se denne videoen for en oversikt over Microsoft 365 Business Premium oppsett.</span><span class="sxs-lookup"><span data-stu-id="8126c-105">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="8126c-106">Legge til domenet, brukerne og konfigurere policyer</span><span class="sxs-lookup"><span data-stu-id="8126c-106">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="8126c-107">Når du kjøper Microsoft 365 Business Premium, har du muligheten til å bruke et domene du eier, eller kjøpe et under [registreringen.](sign-up.md)</span><span class="sxs-lookup"><span data-stu-id="8126c-107">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="8126c-108">Hvis du kjøpte et nytt domene da du registrerte deg, er domenet konfigurert, og du kan flytte til Legg til brukere [og tilordne lisenser](#add-users-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="8126c-108">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="8126c-109">Legge til domenet for å tilpasse påloggingen</span><span class="sxs-lookup"><span data-stu-id="8126c-109">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="8126c-110">Logg på Microsoft 365 [ved](https://admin.microsoft.com) hjelp av den globale administratorlegitimasjonen.</span><span class="sxs-lookup"><span data-stu-id="8126c-110">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="8126c-111">Velg **Gå til konfigurasjon for** å starte veiviseren.</span><span class="sxs-lookup"><span data-stu-id="8126c-111">Choose **Go to setup** to start the wizard.</span></span>

    ![Velg Gå til konfigurasjon.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="8126c-113">På siden **Installer Office apper** kan du eventuelt installere appene på din egen datamaskin.</span><span class="sxs-lookup"><span data-stu-id="8126c-113">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="8126c-114">Skriv inn **domenenavnet** du vil bruke (for eksempel contoso.com) i trinnet Legg til domene.</span><span class="sxs-lookup"><span data-stu-id="8126c-114">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="8126c-115">Hvis du kjøpte et domene under registreringen, vil du ikke se Legge **til et domenetrinn** her.</span><span class="sxs-lookup"><span data-stu-id="8126c-115">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="8126c-116">Gå til [Legg til brukere i](#add-users-and-assign-licenses) stedet.</span><span class="sxs-lookup"><span data-stu-id="8126c-116">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Skjermbilde av siden Tilpass påloggingen.](../media/adddomain.png)

    
4. <span data-ttu-id="8126c-118">Følg trinnene i veiviseren for å opprette DNS-poster hos en [DNS-vertsleverandør for](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) Microsoft 365 som bekrefter at du eier domenet.</span><span class="sxs-lookup"><span data-stu-id="8126c-118">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="8126c-119">Hvis du kjenner domeneverten, kan du se også de [vertsspesifikke instruksjonene.](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)</span><span class="sxs-lookup"><span data-stu-id="8126c-119">If you know your domain host, see also the [host specific instructions](/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="8126c-120">Hvis vertsleverandøren din er GoDaddy [](/office365/admin/get-help-with-domains/domain-connect)eller en annen vert aktivert med domenetilkryssing, er prosessen enkel, og du blir automatisk bedt om å logge på og la Microsoft godkjenne på dine vegne.</span><span class="sxs-lookup"><span data-stu-id="8126c-120">If your hosting provider is GoDaddy or another host enabled with [domain connect](/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Velg Godkjenn på Siden Bekreft tilgang for GoDaddy.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="8126c-122">Legge til brukere og tilordne lisenser</span><span class="sxs-lookup"><span data-stu-id="8126c-122">Add users and assign licenses</span></span>

<span data-ttu-id="8126c-123">Du kan legge til brukere i veiviseren, men du kan også [legge til brukere senere](../admin/add-users/add-users.md) i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="8126c-123">You can add users in the wizard, but you can also [add users later](../admin/add-users/add-users.md) in the admin center.</span></span> <span data-ttu-id="8126c-124">Hvis du har en lokal domenekontroller, kan du i tillegg legge til brukere med [Azure AD Koble til.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="8126c-124">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="8126c-125">Legge til brukere i veiviseren</span><span class="sxs-lookup"><span data-stu-id="8126c-125">Add users in the wizard</span></span>

<span data-ttu-id="8126c-126">Alle brukere du legger til i veiviseren, får automatisk tilordnet en Microsoft 365 Business Premium lisens.</span><span class="sxs-lookup"><span data-stu-id="8126c-126">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Skjermbilde av siden Legg til nye brukere i veiviseren](../media/addnewuserspage.png)

1. <span data-ttu-id="8126c-128">Hvis abonnementet Microsoft 365 Business Premium eksisterende brukere (for eksempel hvis du brukte Azure AD Koble til), får du et alternativ for å tilordne lisenser til dem nå.</span><span class="sxs-lookup"><span data-stu-id="8126c-128">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="8126c-129">Gå videre og legg til lisenser for dem også.</span><span class="sxs-lookup"><span data-stu-id="8126c-129">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="8126c-130">Når du har lagt til brukerne, får du også et alternativ for å dele legitimasjon med de nye brukerne du har lagt til.</span><span class="sxs-lookup"><span data-stu-id="8126c-130">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="8126c-131">Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.</span><span class="sxs-lookup"><span data-stu-id="8126c-131">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="8126c-132">Koble til domenet ditt</span><span class="sxs-lookup"><span data-stu-id="8126c-132">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="8126c-133">Hvis du valgte å bruke .onmicrosoft-domenet eller brukte Azure AD Koble til å konfigurere brukere, vil du ikke se dette trinnet.</span><span class="sxs-lookup"><span data-stu-id="8126c-133">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="8126c-134">Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.</span><span class="sxs-lookup"><span data-stu-id="8126c-134">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="8126c-135">Oppsettsveiviseren oppdager vanligvis registratoren og gir deg en kobling til trinnvise instruksjoner for hvordan du oppdaterer NS-postene på nettstedet til registratoren.</span><span class="sxs-lookup"><span data-stu-id="8126c-135">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="8126c-136">Hvis den ikke gjør det, [endrer du navneservere for å Microsoft 365 med en hvilken som helst domeneregistrator.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md)</span><span class="sxs-lookup"><span data-stu-id="8126c-136">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md).</span></span> 

    - <span data-ttu-id="8126c-137">Hvis du har eksisterende DNS-poster, for eksempel et eksisterende nettsted, men DNS-verten er aktivert for [domene-tilkobling,](/office365/admin/get-help-with-domains/domain-connect)velger du Legg til **poster for meg**.</span><span class="sxs-lookup"><span data-stu-id="8126c-137">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="8126c-138">Godta alle **standardene** på siden Velg **nettbaserte** tjenester, og velg **Neste**, og velg Godkjenn på dns-vertens side.</span><span class="sxs-lookup"><span data-stu-id="8126c-138">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="8126c-139">Hvis du har eksisterende DNS-poster med andre DNS-verter (ikke aktivert for domenekoblet), bør du administrere dine egne DNS-poster for å sikre at de eksisterende tjenestene forblir tilkoblet.</span><span class="sxs-lookup"><span data-stu-id="8126c-139">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="8126c-140">Se [grunnleggende om domener](/office365/admin/get-help-with-domains/dns-basics) hvis du vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="8126c-140">See [domain basics](/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Aktiver poster-siden.](../media/activaterecords.png)

2. <span data-ttu-id="8126c-142">Følg trinnene i veiviseren, og e-post og andre tjenester vil bli konfigurert for deg.</span><span class="sxs-lookup"><span data-stu-id="8126c-142">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="8126c-143">Beskytt organisasjonen</span><span class="sxs-lookup"><span data-stu-id="8126c-143">Protect your organization</span></span> 

<span data-ttu-id="8126c-144">Policyene du konfigurerer i veiviseren, brukes automatisk på en [sikkerhetsgruppe](/office365/admin/create-groups/compare-groups#security-groups) kalt *Alle brukere*.</span><span class="sxs-lookup"><span data-stu-id="8126c-144">The policies you set up in the wizard are applied automatically to a [Security group](/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="8126c-145">Du kan også opprette flere grupper som du kan tilordne policyer til i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="8126c-145">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="8126c-146">På Øk beskyttelse mot avanserte **cybertrusler** anbefales det at du godtar standardinnstillingene for å la Office 365 [Advance Threat Protection](../security/office-365-security/defender-for-office-365.md) skanne filer og koblinger i Office apper.</span><span class="sxs-lookup"><span data-stu-id="8126c-146">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](../security/office-365-security/defender-for-office-365.md) scan files and links in Office apps.</span></span>

    ![Skjermbilde av Siden Øk beskyttelse.](../media/increasetreatprotection.png)


2. <span data-ttu-id="8126c-148">På siden Forhindre **lekkasjer** av sensitive data godtar du standardinnstillingene for å aktivere Office 365 Data loss Prevention (DLP) for å spore sensitive data i Office-apper og hindre utilsiktet deling av disse utenfor organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="8126c-148">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="8126c-149">På siden **Beskytt data i Office for** mobil lar du administrasjon av mobilapper være på, utvider innstillingene og ser gjennom dem, og velger deretter Opprett policy for administrasjon av **mobilapper**.</span><span class="sxs-lookup"><span data-stu-id="8126c-149">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Skjermbilde av Beskytt data i Office for mobilsiden.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="8126c-151">Sikre Windows 10 PC-er</span><span class="sxs-lookup"><span data-stu-id="8126c-151">Secure Windows 10 PCs</span></span>

<span data-ttu-id="8126c-152">Velg Oppsett til  venstre, og **velg** deretter Sikre datamaskinene Windows 10 dine under Pålogging **og sikkerhet**.</span><span class="sxs-lookup"><span data-stu-id="8126c-152">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="8126c-153">Velg **Vis for** å komme i gang.</span><span class="sxs-lookup"><span data-stu-id="8126c-153">Choose **View** to get started.</span></span> <span data-ttu-id="8126c-154">Se [sikre datamaskinene Windows 10 for](secure-win-10-pcs.md) fullstendige instruksjoner.</span><span class="sxs-lookup"><span data-stu-id="8126c-154">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="8126c-155">Distribuere Office 365 klientapper</span><span class="sxs-lookup"><span data-stu-id="8126c-155">Deploy Office 365 client apps</span></span>

<span data-ttu-id="8126c-156">Hvis du velger å installere Office-apper automatisk under installasjonen, installeres appene på Windows 10-enhetene når brukerne har logget på Azure AD fra Windows-enhetene sine ved hjelp av jobblegitimasjonen.</span><span class="sxs-lookup"><span data-stu-id="8126c-156">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="8126c-157">Hvis du vil Office på mobile iOS- eller [Android-enheter,](set-up-mobile-devices.md)kan du se Konfigurere mobile enheter for Microsoft 365 Business Premium brukere .</span><span class="sxs-lookup"><span data-stu-id="8126c-157">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="8126c-158">Du kan også installere Office enkeltvis.</span><span class="sxs-lookup"><span data-stu-id="8126c-158">You can also install Office individually.</span></span> <span data-ttu-id="8126c-159">Se [Installere Office på en PC eller Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instruksjoner.</span><span class="sxs-lookup"><span data-stu-id="8126c-159">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="related-content"></a><span data-ttu-id="8126c-160">Beslektet innhold</span><span class="sxs-lookup"><span data-stu-id="8126c-160">Related content</span></span>

<span data-ttu-id="8126c-161">[Microsoft 365 opplæringsvideoer for bedrifter](../business-video/index.yml) (koblingsside)</span><span class="sxs-lookup"><span data-stu-id="8126c-161">[Microsoft 365 for business training videos](../business-video/index.yml) (link page)</span></span>
