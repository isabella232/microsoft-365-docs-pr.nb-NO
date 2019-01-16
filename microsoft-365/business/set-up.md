---
title: Konfigurere Microsoft 365 Business ved hjelp av veiviseren for konfigurasjon
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
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Lær hvordan du konfigurerer Microsoft 365 Business ved å fylle ut fire trinn.
ms.openlocfilehash: f57239b884bd2e186c0bc01973130a10fa4cfe84
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982196"
---
# <a name="set-up-microsoft-365-business-by-using-the-setup-wizard"></a><span data-ttu-id="80860-103">Konfigurere Microsoft 365 Business ved hjelp av veiviseren for konfigurasjon</span><span class="sxs-lookup"><span data-stu-id="80860-103">Set up Microsoft 365 Business by using the setup wizard</span></span>

<span data-ttu-id="80860-104">Fullfør trinn 1-4 nedenfor.</span><span class="sxs-lookup"><span data-stu-id="80860-104">Complete steps 1-4 below.</span></span>
  
### <a name="set-up-microsoft-365-business"></a><span data-ttu-id="80860-105">Konfigurere Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="80860-105">Set up Microsoft 365 Business</span></span>

<span data-ttu-id="80860-106">Se en video om hvordan du konfigurerer Microsoft 365 Business når du ikke har en lokale Active Directory:</span><span class="sxs-lookup"><span data-stu-id="80860-106">Watch a video on how to set up Microsoft 365 Business when you don't have an on-premises Active Directory:</span></span>
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/0705c337-f3e8-4d28-bb6c-530cd28e99f2?autoplay=false]
  
<span data-ttu-id="80860-p101">Fremgangsmåten for oppsett inneholder informasjon for oppsett som inkluderer lokale Active Directory. Hvis du vil fortsette å få tilgang til domenetilknyttede enheter, Les følgende artikler for to forskjellige måter for å aktivere som, og Fullfør trinnene før du kjører veiviseren for installasjon:</span><span class="sxs-lookup"><span data-stu-id="80860-p101">The set-up steps include information for setups that include local Active Directory. If you want to continue to access domain-joined devices, read the following articles for two different way of enabling that, and complete the steps before you run the Setup wizard:</span></span>
  
- [<span data-ttu-id="80860-109">Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="80860-109">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>](manage-windows-devices.md)
    
    <span data-ttu-id="80860-110">– Dette er den anbefalte måten.</span><span class="sxs-lookup"><span data-stu-id="80860-110">-This is the recommended way.</span></span>
    
- [<span data-ttu-id="80860-111">Access lokale ressurser fra en Azure AD-koblet enheten i Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="80860-111">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>](access-resources.md)
    
### <a name="step-1-personalize-sign-in"></a><span data-ttu-id="80860-112">Trinn 1: Tilpasse pålogging</span><span class="sxs-lookup"><span data-stu-id="80860-112">Step 1: Personalize sign-in</span></span>

1. <span data-ttu-id="80860-p102">Logg på [Microsoft 365 Business](https://portal.microsoft.com) ved hjelp av legitimasjonen for global administrator. Velg **Administrasjon**-flisen for å gå til administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="80860-p102">Sign in to [Microsoft 365 Business](https://portal.microsoft.com) by using your global admin credentials. Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="80860-115">Velg **Start konfigurasjon** (det kan hende du ser **Fortsett konfigurasjon** i stedet, avhengig av status) i administrasjonssenteret for å starte veiviseren.</span><span class="sxs-lookup"><span data-stu-id="80860-115">Choose **Start setup** (depending on your state you may see **Continue setup** instead) in the admin center to start the wizard.</span></span> 
    
3. <span data-ttu-id="80860-116">Skriv inn domenenavnet du vil bruke (for eksempel contoso.com).</span><span class="sxs-lookup"><span data-stu-id="80860-116">Enter the domain name you want to use (like contoso.com).</span></span>
    
    <span data-ttu-id="80860-p103">Gå videre og Skriv inn domenet ditt selv om du har bekreftet det ved hjelp av Azure AD-tilkobling, for eksempel. De følgende to trinnene gjelder ikke for deg hvis du brukte Azure AD-tilkobling for å bekrefte domenet.</span><span class="sxs-lookup"><span data-stu-id="80860-p103">Go ahead and enter your domain even if you have verified it while using Azure AD Connect, for example. The following two steps do not apply to you if you used Azure AD Connect to verify your domain.</span></span>
    
4. <span data-ttu-id="80860-119">Følg trinnene i veiviseren til å [opprette DNS-poster på alle DNS-vertsleverandøren for Office 365](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) , som bekrefter at du eier domenet.</span><span class="sxs-lookup"><span data-stu-id="80860-119">Follow the steps in the wizard to [Create DNS records at any DNS hosting provider for Office 365](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) that verifies you own the domain.</span></span> 
    
    <span data-ttu-id="80860-p104">Du kan vise et eksempel video av [Video: installasjonsprogrammet for Office 365 i administrasjonssenteret nye](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8). Vær oppmerksom på at denne videoen ikke inneholder data protection trinnene i Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="80860-p104">You can view an example video of [Video: Setup Office 365 in the new Admin Center](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8). Note that this video does not include the data protection steps of Microsoft 365 Business.</span></span>
    
    ![Screenshot of the Business Cloud Suite setup wizard.](media/3c4fd40c-2de1-4a87-8ee0-78d3928c7bb7.png)
  
### <a name="step-2-add-users-and-assign-licenses"></a><span data-ttu-id="80860-123">Trinn 2: Legge til brukere og tilordne lisenser</span><span class="sxs-lookup"><span data-stu-id="80860-123">Step 2: Add users and assign licenses</span></span>

1. <span data-ttu-id="80860-124">Du kan legge til brukere her, eller du kan [legge til brukere senere](add-users-m365b.md) i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="80860-124">You can add users here, or you can [add users later](add-users-m365b.md) in the admin center.</span></span> 
    
    <span data-ttu-id="80860-125">Alle brukerne du legger til, får automatisk tildelt en Microsoft 365 Business-lisens.</span><span class="sxs-lookup"><span data-stu-id="80860-125">Any users you add get automatically assigned a Microsoft 365 Business license.</span></span>
    
2. <span data-ttu-id="80860-p105">Hvis ditt Microsoft 365 Business-abonnement har eksisterende brukere (for eksempel hvis du brukte Azure AD Connect), får du muligheten til å tildele lisenser til dem nå. Gå videre og legg til lisenser for dem også.</span><span class="sxs-lookup"><span data-stu-id="80860-p105">If your Microsoft 365 Business subscription has existing users (for example, if you used Azure AD Connect) , you will get an option to assign licenses to them now. Go ahead and add licenses to them as well.</span></span>
    
3. <span data-ttu-id="80860-p106">Du får også en mulighet til å dele legitimasjon med de nye brukerne du har lagt til. Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.</span><span class="sxs-lookup"><span data-stu-id="80860-p106">You will also get an option to share credentials with the new users you added. You can choose to print them out, email them, or download them.</span></span>
    
4. <span data-ttu-id="80860-130">Hopp over overføring av e-postmeldinger, og velg **Neste** på **Overfør e-postmeldinger**-siden.</span><span class="sxs-lookup"><span data-stu-id="80860-130">Skip migrating email messages and choose **Next** on **Migrate email messages** page.</span></span> 
    
    <span data-ttu-id="80860-131">Hvis du flytter fra en annen leverandør av e-post og vil kopiere dataene senere, kan du [Overfør e-post og kontakter til Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span><span class="sxs-lookup"><span data-stu-id="80860-131">If you are moving from another email provider and want to copy your data later, you can [Migrate email and contacts to Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).</span></span>
    
    ![Screenshot of two new users added in the setup wizard](media/8f729967-5c65-4ceb-b737-18119db40564.png)
  
### <a name="step-3-connect-your-domain"></a><span data-ttu-id="80860-133">Trinn 3: Koble til domenet</span><span class="sxs-lookup"><span data-stu-id="80860-133">Step 3: Connect your domain</span></span>

> [!NOTE]
> <span data-ttu-id="80860-134">Hvis du velger å bruke .onmicrosoft-domene, eller brukt Azure AD-tilkobling, vil du ikke se dette trinnet.</span><span class="sxs-lookup"><span data-stu-id="80860-134">If you chose to use the .onmicrosoft domain, or used Azure AD Connect, you will not see this step.</span></span> 
  
<span data-ttu-id="80860-135">Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.</span><span class="sxs-lookup"><span data-stu-id="80860-135">To set up services, you have to update some records at your DNS host or domain registrar.</span></span>
  
1. <span data-ttu-id="80860-p107">Installasjonsveiviseren vanligvis oppdager registraren og gir deg en kobling til trinnvise instruksjoner for å oppdatere NS-postene på webområdet registrar. Hvis ikke, [Endre nameservers for å konfigurere Office 365 med en hvilken som helst domeneregistrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span><span class="sxs-lookup"><span data-stu-id="80860-p107">The setup wizard typically detects your registrar and gives you a link to step-by-step instructions for updating your NS records at the registrar website. If it doesn't, [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).</span></span>
    
2. <span data-ttu-id="80860-138">E-post og andre tjenester vil bli opprettet for deg</span><span class="sxs-lookup"><span data-stu-id="80860-138">Email and other services will be set up for you</span></span>
    
### <a name="step-4-manage-devices-and-work-files"></a><span data-ttu-id="80860-139">Trinn 4: Håndtere enheter og arbeide filer</span><span class="sxs-lookup"><span data-stu-id="80860-139">Step 4: Manage devices and work files</span></span>

1. <span data-ttu-id="80860-p108">Siden Angi **styre hvordan brukere får tilgang til Office-filer på mobile enheter** innstillinger og **Beskytt arbeidsfiler når enhetene mistes eller blir stjålet** **på**, på **Beskytt arbeidsfiler på mobile enheter** . Du kan også få tilgang til hver underordnet innstilling ved å klikke pilene ved siden av hver innstilling.</span><span class="sxs-lookup"><span data-stu-id="80860-p108">On the **Protect work files on your mobile devices** page set both **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** settings to **On**. You can also access each sub-setting by clicking the chevrons next to each setting.</span></span>
  
  <span data-ttu-id="80860-142">Alle de lisensierte brukere arbeidsfiler blir nå beskyttet på iOS og Android enheter, så snart de [installerer Office-programmer](set-up-mobile-devices.md) (og godkjenne legitimasjonen Microsoft 365 Business).</span><span class="sxs-lookup"><span data-stu-id="80860-142">All of your licensed users' work files are now protected on iOS and Android devices, as soon as they [install Office apps](set-up-mobile-devices.md) (and authenticate with their Microsoft 365 Business credentials).</span></span> 
  
  ![Screenshot of protect work files on your mobile devices page](media/3139a9aa-6228-4e74-8166-c6a886d7319f.PNG)
  
2. <span data-ttu-id="80860-144">På siden **Angi Windows-10 enhetskonfigurasjon** sette innstillingen for **Sikker Windows 10 enheter** **på**.</span><span class="sxs-lookup"><span data-stu-id="80860-144">On the **Set Windows 10 device configuration** page, set **Secure Windows 10 Devices** setting to **On**.</span></span>
  
   <span data-ttu-id="80860-145">Du kan også få tilgang til hver underordnet innstilling ved å klikke vinkeltegnet ved siden av den.</span><span class="sxs-lookup"><span data-stu-id="80860-145">You can also access each sub-setting by clicking the chevron next to it.</span></span>
  
3. <span data-ttu-id="80860-p109">Sett innstillingen for å **Installere Office på Windows 10 enheter** til **Ja** hvis alle brukerne har 10 for Windows-datamaskiner, og ingen eksisterende Office installeres, eller klikk for å kjøre Office-installasjoner. Hvis dette ikke er tilfelle, setter du dette alternativet til **Nei**. Du kan [automatisk installere Office](auto-install-or-uninstall-office.md) senere fra administrasjonssenteret når du har klargjort på brukernes datamaskiner. For instruksjoner, kan du se [forberede installasjon av Office-klienten](prepare-for-office-client-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="80860-p109">Set the **Install Office on Windows 10 Devices** setting to **Yes** if all of your users have Windows 10 computers, and either no existing Office installs, or click-to-run Office installs. If this is not the case, set this option to **No**. You can [automatically install Office](auto-install-or-uninstall-office.md) later from the admin center after you have prepared the user computers. For instructions, see [prepare for Office client installation](prepare-for-office-client-deployment.md).</span></span>
  
    <span data-ttu-id="80860-150">Den lisensierte brukere arbeidsfiler på Windows 10 enheter blir vist så snart de [bli med sine Windows 10-enhet](set-up-windows-devices.md) til et Microsoft 365 Business Azure AD-domene eller [installere Windows 10 på en ny datamaskin](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) mens du samtidig å bli med i Microsoft-365 Business Azure AD-domene.</span><span class="sxs-lookup"><span data-stu-id="80860-150">The licensed users' work files on Windows 10 devices will be projected as soon as they [join their Windows 10 device](set-up-windows-devices.md) to a Microsoft 365 Business Azure AD domain or [install Windows 10 on a new computer](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) while simultaneously joining the Microsoft 365 Business Azure AD domain.</span></span> 
  
4. <span data-ttu-id="80860-151">Klikk **Neste** , og du er ferdig med installasjonen.</span><span class="sxs-lookup"><span data-stu-id="80860-151">Click **Next** and you are done with setup.</span></span> 
  
    <span data-ttu-id="80860-152">La oss tilbakemelding på dette trinnet for å hjelpe oss å forbedre opplevelsen.</span><span class="sxs-lookup"><span data-stu-id="80860-152">Please leave us feedback at this step to help us improve the experience.</span></span>
  
    ![Screenshot of Prepare Windows 10 devices page](media/bff701c1-48a3-44f4-aa95-9d959d57c85b.PNG)
  
## <a name="additional-security-settings"></a><span data-ttu-id="80860-154">Flere sikkerhetsinnstillinger</span><span class="sxs-lookup"><span data-stu-id="80860-154">Additional security settings</span></span>

<span data-ttu-id="80860-155">I tillegg til sikkerhet og overholdelse innstillingen i installasjonsveiviseren, kan du også angi følgende tilleggsinnstillinger:</span><span class="sxs-lookup"><span data-stu-id="80860-155">In addition to the security and compliance setting in the setup wizard, you can also set up the following additional settings:</span></span>
  
- <span data-ttu-id="80860-p110">Angi beskyttelse mot usikre vedlegg. **Avansert Threat Protection** (ATP) identifiserer skadelig innhold og blokkerer leveringen av usikre vedlegg, bidrar til å beskytte deg mot phishing-forsøk og ransomware infeksjoner. Hvis du vil aktivere beskyttelse for vedlegg, kan du se [definere policyer for Office 365 ATP trygt vedlegg](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).</span><span class="sxs-lookup"><span data-stu-id="80860-p110">Set up protection against unsafe attachments. **Advanced Threat Protection** (ATP) identifies malicious content and then blocks delivery of unsafe attachments, helping protect you against phishing schemes and ransomware infections. To activate attachment protection, see [Set up Office 365 ATP Safe Attachments policies](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).</span></span>
    
- <span data-ttu-id="80860-p111">Beskytte miljøet når brukere klikker skadelig koblinger. ATP undersøker koblinger i e-post når en bruker klikker dem.. Hvis en kobling er usikre, er brukeren varsles om ikke å gå til webområdet eller informert om at webområdet er blokkert. Dette bidrar til å beskytte deg mot phishing-forsøk. [Definer policyer for Office 365 ATP-klarerte koblinger](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) eller [definere policyer for Office 365 ATP-klarerte koblinger](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).</span><span class="sxs-lookup"><span data-stu-id="80860-p111">Protect your environment when users click malicious links. ATP examines links in email at the time a user clicks them. If a link is unsafe, the user is warned not to visit the site or informed that the site has been blocked. This helps protect against phishing schemes. [Set up Office 365 ATP Safe Links policies](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) or [Set up Office 365 ATP Safe Links policies](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).</span></span>
    
- <span data-ttu-id="80860-p112">Du kan beholde alle postboks-innhold, inkludert Slettede elementer ved å plassere hele postboksen for en bruker i **rettstvist holder**. For instruksjoner, se</span><span class="sxs-lookup"><span data-stu-id="80860-p112">You can preserve all mailbox content including deleted items by putting a user's entire mailbox on **litigation hold**. For instructions, see</span></span> 
- <span data-ttu-id="80860-166">[Definer tilbakeholdelse av e-post med Exchange Online-arkivering](security-features.md#set-up-email-retention-with-exchange-online-archiving).</span><span class="sxs-lookup"><span data-stu-id="80860-166">[Set up email retention with Exchange Online Archiving](security-features.md#set-up-email-retention-with-exchange-online-archiving).</span></span>
    
- <span data-ttu-id="80860-p113">Definer tilpassede **policyer for dokumentoppbevaring**, for eksempel å bevare i en bestemt tidsperiode eller slette innholdet permanent på slutten av Oppbevaringstiden. Du kan aktivere egendefinerte oppbevaringspolicyer i verdipapirer og overholdelse center, går du til **styring av Data** \> **oppbevaring**, og følg deretter instruksjonene i veiviseren. Hvis du vil ha mer informasjon, se [Oversikt over policyer for dokumentoppbevaring](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="80860-p113">Set up customized **retention policies**, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period. You can enable customized retention policies in the Securities and compliance center, go to **Data governance** \> **Retention**, and then follow the steps in the wizard. To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>
    
## <a name="next-steps"></a><span data-ttu-id="80860-170">Neste trinn</span><span class="sxs-lookup"><span data-stu-id="80860-170">Next steps</span></span>

<span data-ttu-id="80860-171">For brukere som har sine lisenser, er neste trinn å konfigurere enheter.</span><span class="sxs-lookup"><span data-stu-id="80860-171">For the users that have their licenses, the next step is to set up devices.</span></span><br/> <span data-ttu-id="80860-172">Se [konfigurere Windows-enheter for forretningsbrukere som Microsoft 365](set-up-windows-devices.md) og [definere mobile enheter for forretningsbrukere som Microsoft 365](set-up-mobile-devices.md).</span><span class="sxs-lookup"><span data-stu-id="80860-172">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) and [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md).</span></span> <br/><span data-ttu-id="80860-173">Se [Behandle Microsoft 365 Business](manage.md) for koblinger til emner om hvordan du angir beskyttelse enheten og app-policyer, og hvordan du kan fjerne data fra Brukerenheter.</span><span class="sxs-lookup"><span data-stu-id="80860-173">See [Manage Microsoft 365 Business](manage.md) for links to topics on how to set device and app protection polices, and how to remove data from user devices.</span></span> 
  


