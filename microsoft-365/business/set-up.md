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
description: Oppdag konfigurasjonstrinnene for Microsoft 365 Business Premium, inkludert å legge til et domene og brukere, konfigurere sikkerhetspolicyer og mer.
ms.openlocfilehash: e7ebe179c67077dc71ae4873b0711d0e810c701a
ms.sourcegitcommit: 1b30ac6e05906c8a014b1fed33fc71e1821f6ad2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2021
ms.locfileid: "50044734"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a><span data-ttu-id="f054d-103">Konfigurere Microsoft 365 Business Premium i konfigurasjonsveiviseren</span><span class="sxs-lookup"><span data-stu-id="f054d-103">Set up Microsoft 365 Business Premium in the setup wizard</span></span>

<span data-ttu-id="f054d-104">Se denne videoen for å få en oversikt over konfigurasjon av Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="f054d-104">Watch this video for an overview of Microsoft 365 Business Premium setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a><span data-ttu-id="f054d-105">Legge til domenet ditt, brukere og konfigurere policyer</span><span class="sxs-lookup"><span data-stu-id="f054d-105">Add your domain, users, and set up policies</span></span>

<span data-ttu-id="f054d-106">Når du kjøper Microsoft 365 Business Premium, kan du bruke et domene du eier, eller kjøpe et under [registreringen.](sign-up.md)</span><span class="sxs-lookup"><span data-stu-id="f054d-106">When you purchase Microsoft 365 Business Premium, you have the option of using a domain you own, or buying one during the [sign-up](sign-up.md).</span></span>

- <span data-ttu-id="f054d-107">Hvis du kjøpte et nytt domene da du registrerte deg, er domenet konfigurert, og du kan flytte til Legg til brukere og [tilordne lisenser.](#add-users-and-assign-licenses)</span><span class="sxs-lookup"><span data-stu-id="f054d-107">If you purchased a new domain when you signed up, your domain is all set up and you can move to [Add users and assign licenses](#add-users-and-assign-licenses).</span></span>

### <a name="add-your-domain-to-personalize-sign-in"></a><span data-ttu-id="f054d-108">Legge til domenet for å tilpasse pålogging</span><span class="sxs-lookup"><span data-stu-id="f054d-108">Add your domain to personalize sign-in</span></span>

1. <span data-ttu-id="f054d-109">Logg på [administrasjonssenteret for Microsoft 365](https://admin.microsoft.com) ved hjelp av legitimasjonen for global administrator.</span><span class="sxs-lookup"><span data-stu-id="f054d-109">Sign in to [Microsoft 365 admin center](https://admin.microsoft.com) by using your global admin credentials.</span></span> 

2. <span data-ttu-id="f054d-110">Velg **Gå til konfigurasjon for** å starte veiviseren.</span><span class="sxs-lookup"><span data-stu-id="f054d-110">Choose **Go to setup** to start the wizard.</span></span>

    ![Velg Gå til konfigurasjon.](../media/gotosetupinadmincenter.png)

3. <span data-ttu-id="f054d-112">På siden **Installer Office-apper** kan du også installere appene på din egen datamaskin.</span><span class="sxs-lookup"><span data-stu-id="f054d-112">On the **Install your Office apps** page, you can optionally install the apps on your own computer.</span></span>
    
4. <span data-ttu-id="f054d-113">I **trinnet Legg til** domene skriver du inn domenenavnet du vil bruke (for contoso.com).</span><span class="sxs-lookup"><span data-stu-id="f054d-113">In the **Add domain** step, enter the domain name you want to use (like contoso.com).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="f054d-114">Hvis du kjøpte et domene under registreringen, ser du ikke Legg til **et domene-trinn** her.</span><span class="sxs-lookup"><span data-stu-id="f054d-114">If you purchased a domain during the sign-up, you will not see **Add a domain** step here.</span></span> <span data-ttu-id="f054d-115">Gå til [Legg til brukere i](#add-users-and-assign-licenses) stedet.</span><span class="sxs-lookup"><span data-stu-id="f054d-115">Go to [Add users](#add-users-and-assign-licenses) instead.</span></span>

    ![Skjermbilde av siden Tilpass påloggingen.](../media/adddomain.png)

    
4. <span data-ttu-id="f054d-117">Følg fremgangsmåten i veiviseren for å [opprette DNS-poster hos en DNS-vert for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) som bekrefter at du eier domenet.</span><span class="sxs-lookup"><span data-stu-id="f054d-117">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) that verifies you own the domain.</span></span> <span data-ttu-id="f054d-118">Hvis du kjenner domeneverten, kan du også se [vertens spesifikke instruksjoner.](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)</span><span class="sxs-lookup"><span data-stu-id="f054d-118">If you know your domain host, see also the [host specific instructions](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).</span></span>

    <span data-ttu-id="f054d-119">Hvis vertsleverandøren er GoDaddy eller [](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)en annen vert som er aktivert med domenekryssing, er prosessen enkel, og du blir automatisk bedt om å logge på og la Microsoft godkjenne på dine vegne.</span><span class="sxs-lookup"><span data-stu-id="f054d-119">If your hosting provider is GoDaddy or another host enabled with [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), the process is easy and you'll be automatically asked to sign in and let Microsoft authenticate on your behalf.</span></span>

    ![Velg Godkjenn på GoDaddys bekreft tilgang-side.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a><span data-ttu-id="f054d-121">Legge til brukere og tilordne lisenser</span><span class="sxs-lookup"><span data-stu-id="f054d-121">Add users and assign licenses</span></span>

<span data-ttu-id="f054d-122">Du kan legge til brukere i veiviseren, men du kan også [legge til brukere senere](add-users-m365b.md) i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="f054d-122">You can add users in the wizard, but you can also [add users later](add-users-m365b.md) in the admin center.</span></span> <span data-ttu-id="f054d-123">Hvis du har en lokal domenekontroller, kan du i tillegg legge til brukere [med Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="f054d-123">Additionally, if you have a local domain controller, you can add users with [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

#### <a name="add-users-in-the-wizard"></a><span data-ttu-id="f054d-124">Legge til brukere i veiviseren</span><span class="sxs-lookup"><span data-stu-id="f054d-124">Add users in the wizard</span></span>

<span data-ttu-id="f054d-125">Alle brukere du legger til i veiviseren, tilordnes automatisk en Lisens for Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="f054d-125">Any users you add in the wizard get automatically assigned a Microsoft 365 Business Premium license.</span></span>

![Skjermbilde av siden Legg til nye brukere i veiviseren](../media/addnewuserspage.png)

1. <span data-ttu-id="f054d-127">Hvis Microsoft 365 Business Premium-abonnementet har eksisterende brukere (for eksempel hvis du brukte Azure AD Connect), får du et alternativ for å tilordne lisenser til dem nå.</span><span class="sxs-lookup"><span data-stu-id="f054d-127">If your Microsoft 365 Business Premium subscription has existing users (for example, if you used Azure AD Connect), you get an option to assign licenses to them now.</span></span> <span data-ttu-id="f054d-128">Gå videre og legg til lisenser for dem også.</span><span class="sxs-lookup"><span data-stu-id="f054d-128">Go ahead and add licenses to them as well.</span></span>

2. <span data-ttu-id="f054d-129">Når du har lagt til brukerne, får du også et alternativ for å dele legitimasjon med de nye brukerne du har lagt til.</span><span class="sxs-lookup"><span data-stu-id="f054d-129">After you've added the users, you'll also get an option to share credentials with the new users you added.</span></span> <span data-ttu-id="f054d-130">Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.</span><span class="sxs-lookup"><span data-stu-id="f054d-130">You can choose to print them out, email them, or download them.</span></span>

### <a name="connect-your-domain"></a><span data-ttu-id="f054d-131">Koble til domenet ditt</span><span class="sxs-lookup"><span data-stu-id="f054d-131">Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="f054d-132">Hvis du valgte å bruke .onmicrosoft-domenet, eller brukte Azure AD Connect til å konfigurere brukere, vil du ikke se dette trinnet.</span><span class="sxs-lookup"><span data-stu-id="f054d-132">If you chose to use the .onmicrosoft domain, or used Azure AD Connect to set up users, you will not see this step.</span></span>
  
<span data-ttu-id="f054d-133">Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.</span><span class="sxs-lookup"><span data-stu-id="f054d-133">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="f054d-134">Oppsettsveiviseren oppdager vanligvis registratoren og gir deg en kobling til trinnvise instruksjoner for hvordan du oppdaterer NS-postene på nettstedet til registratoren.</span><span class="sxs-lookup"><span data-stu-id="f054d-134">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website.</span></span> <span data-ttu-id="f054d-135">Hvis den ikke gjør det, [endrer du navneservere for å konfigurere Microsoft 365 med en hvilken som helst domeneregistrator.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="f054d-135">If it doesn't, [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar).</span></span> 

    - <span data-ttu-id="f054d-136">Hvis du har eksisterende DNS-poster, for eksempel et eksisterende nettsted, men DNS-verten er aktivert for [domene](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)connect, velger du Legg **til poster for meg.**</span><span class="sxs-lookup"><span data-stu-id="f054d-136">If you have existing DNS records, for example an existing web site, but your DNS host is enabled for [domain connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), choose **Add records for me**.</span></span> <span data-ttu-id="f054d-137">Godta alle **standardinnstillingene på** siden Velg nettjenester, og velg  **Neste,** og velg Autoriser på siden til DNS-verten.</span><span class="sxs-lookup"><span data-stu-id="f054d-137">On the **Choose your online services** page, accept all the defaults, and choose **Next**, and choose **Authorize** on your DNS host's page.</span></span>
    - <span data-ttu-id="f054d-138">Hvis du har eksisterende DNS-poster med andre DNS-verter (ikke aktivert for domenekoblet), må du administrere dine egne DNS-poster for å sikre at de eksisterende tjenestene forblir tilkoblet.</span><span class="sxs-lookup"><span data-stu-id="f054d-138">If you have existing DNS records with other DNS hosts (not enabled for domain connect), you'll want to manage your own DNS records to make sure the existing services stay connected.</span></span> <span data-ttu-id="f054d-139">Se [grunnleggende funksjoner](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for domenet hvis du vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="f054d-139">See [domain basics](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for more info.</span></span>

        ![Siden Aktiver poster.](../media/activaterecords.png)

2. <span data-ttu-id="f054d-141">Følg trinnene i veiviseren, og e-post og andre tjenester vil bli konfigurert for deg.</span><span class="sxs-lookup"><span data-stu-id="f054d-141">Follow the steps in the wizard and email and other services will be set up for you.</span></span>

### <a name="protect-your-organization"></a><span data-ttu-id="f054d-142">Beskytte organisasjonen</span><span class="sxs-lookup"><span data-stu-id="f054d-142">Protect your organization</span></span> 

<span data-ttu-id="f054d-143">Policyene du konfigurerte i veiviseren, brukes automatisk på en [sikkerhetsgruppe](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) kalt *Alle brukere.*</span><span class="sxs-lookup"><span data-stu-id="f054d-143">The policies you set up in the wizard are applied automatically to a [Security group](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) called *All Users*.</span></span> <span data-ttu-id="f054d-144">Du kan også opprette flere grupper for å tilordne policyer til i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="f054d-144">You can also create additional groups to assign policies to in the admin center.</span></span>

1. <span data-ttu-id="f054d-145">På Øk beskyttelse fra avanserte **datatrusler** anbefales det at du godtar standardverdiene for å la [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) skanne filer og koblinger i Office-apper.</span><span class="sxs-lookup"><span data-stu-id="f054d-145">On the **Increase protection from advanced cyber threats**, it is recommended that you accept the defaults to let [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) scan files and links in Office apps.</span></span>

    ![Skjermbilde av Øk beskyttelse-siden.](../media/increasetreatprotection.png)


2. <span data-ttu-id="f054d-147">Godta standardinnstillingen for å slå på Office 365 Data Loss Prevention (DLP) for å spore sensitive data i Office-apper og forhindre utilsiktet deling av disse utenfor organisasjonen, på siden Forhindre lekkasje av sensitive **data.**</span><span class="sxs-lookup"><span data-stu-id="f054d-147">On the **Prevent leaks of sensitive data** page, accept the defaults to turn on Office 365 Data Loss Prevention (DLP) to track sensitive data in Office apps and prevent the accidental sharing of these outside your organization.</span></span>

3. <span data-ttu-id="f054d-148">La administrasjon av mobilapper være på, utvid innstillingene og se gjennom dem, og velg deretter Opprett policy for administrasjon av **mobilapper** på siden Beskytt data i **Office for** mobil.</span><span class="sxs-lookup"><span data-stu-id="f054d-148">On the **Protect data in Office for mobile** page, leave mobile app management on, expand the settings and review them, and then select **Create mobile app management policy**.</span></span>

    ![Skjermbilde av siden Beskytt data i Office for mobil.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a><span data-ttu-id="f054d-150">Sikre PC-er med Windows 10</span><span class="sxs-lookup"><span data-stu-id="f054d-150">Secure Windows 10 PCs</span></span>

<span data-ttu-id="f054d-151">Velg Konfigurer til  venstre, og velg deretter Sikre **Windows 10-datamaskinene** under Pålogging og sikkerhet. </span><span class="sxs-lookup"><span data-stu-id="f054d-151">On the left nav, select **Setup** and then, under **Sign-in and security**, choose **Secure your Windows 10 computers**.</span></span> <span data-ttu-id="f054d-152">Velg **Vis for** å komme i gang.</span><span class="sxs-lookup"><span data-stu-id="f054d-152">Choose **View** to get started.</span></span> <span data-ttu-id="f054d-153">Se [sikre Windows 10-datamaskiner](secure-win-10-pcs.md) for fullstendige instruksjoner.</span><span class="sxs-lookup"><span data-stu-id="f054d-153">See [secure your Windows 10 computers](secure-win-10-pcs.md) for complete instructions.</span></span>

## <a name="deploy-office-365-client-apps"></a><span data-ttu-id="f054d-154">Distribuere Office 365-klientapper</span><span class="sxs-lookup"><span data-stu-id="f054d-154">Deploy Office 365 client apps</span></span>

<span data-ttu-id="f054d-155">Hvis du velger å installere Office-apper automatisk under installasjonen, installeres appene på Windows 10-enhetene når brukerne har logget på Azure AD fra Windows-enhetene sine ved hjelp av jobblegitimasjonen.</span><span class="sxs-lookup"><span data-stu-id="f054d-155">If you chose to automatically install Office apps during setup, the apps will install on the Windows 10 devices once the users have signed in to Azure AD from their Windows devices, using their work credentials.</span></span>

<span data-ttu-id="f054d-156">Hvis du vil installere Office på mobile iOS- eller Android-enheter, kan du se Konfigurere mobile enheter for Brukere av [Microsoft 365 Business Premium.](set-up-mobile-devices.md)</span><span class="sxs-lookup"><span data-stu-id="f054d-156">To install Office on mobile iOS or Android devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md).</span></span>

<span data-ttu-id="f054d-157">Du kan også installere Office enkeltvis.</span><span class="sxs-lookup"><span data-stu-id="f054d-157">You can also install Office individually.</span></span> <span data-ttu-id="f054d-158">Se [installere Office på en PC eller Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instruksjoner.</span><span class="sxs-lookup"><span data-stu-id="f054d-158">See [install Office on a PC or Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instructions.</span></span>

## <a name="see-also"></a><span data-ttu-id="f054d-159">Se også</span><span class="sxs-lookup"><span data-stu-id="f054d-159">See also</span></span>

[<span data-ttu-id="f054d-160">Opplæringsvideoer for Microsoft 365 for bedrifter</span><span class="sxs-lookup"><span data-stu-id="f054d-160">Microsoft 365 for business training videos</span></span>](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
