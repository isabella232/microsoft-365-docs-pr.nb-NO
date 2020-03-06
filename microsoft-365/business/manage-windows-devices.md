---
title: Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business
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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Lær hvordan du aktiverer Microsoft 365 for å beskytte lokale Active-Directory-tilknyttede Windows 10-enheter med bare noen få trinn.
ms.openlocfilehash: 8d7caefa1ddcadf684fdb5b712601b1bdd4fb5bd
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/06/2020
ms.locfileid: "42550251"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="18629-103">Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="18629-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="18629-104">Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business til å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgang til lokale ressurser som krever lokal godkjenning.</span><span class="sxs-lookup"><span data-stu-id="18629-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="18629-105">Hvis du vil konfigurere denne beskyttelsen, kan du implementere **hybrid Azure AD-tilknyttede enheter**.</span><span class="sxs-lookup"><span data-stu-id="18629-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="18629-106">Disse enhetene er koblet til både den lokale Active Directory og Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="18629-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="18629-107">Denne videoen beskriver fremgangsmåten for hvordan du konfigurerer dette for det vanligste scenariet, som også er beskrevet i trinnene som følger.</span><span class="sxs-lookup"><span data-stu-id="18629-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="18629-108">1. Klargjør for katalogsynkronisering</span><span class="sxs-lookup"><span data-stu-id="18629-108">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="18629-109">Før du synkroniserer brukere og datamaskiner fra det lokale Active Directory-domenet, kan du se [Klargjøre for katalogsynkronisering til Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="18629-109">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="18629-110">Spesielt:</span><span class="sxs-lookup"><span data-stu-id="18629-110">In particular:</span></span>

   - <span data-ttu-id="18629-111">Kontroller at det ikke finnes noen duplikater i katalogen for følgende attributter: **e-post,** **proxy-adresser**og **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="18629-111">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="18629-112">Disse verdiene må være unike, og eventuelle duplikater må fjernes.</span><span class="sxs-lookup"><span data-stu-id="18629-112">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="18629-113">Vi anbefaler at du konfigurerer attributtet **userPrincipalName** (UPN) for hver lokale brukerkonto slik at det samsvarer med den primære e-postadressen som tilsvarer den lisensierte Microsoft 365-brukeren.</span><span class="sxs-lookup"><span data-stu-id="18629-113">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="18629-114">For eksempel: *mary.shelley@contoso.com* i stedet for *mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="18629-114">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="18629-115">Hvis Active Directory-domenet slutter i et ikke-rutbart suffiks som *lokale* eller *LAN*, i stedet for et internett-rutbart suffiks, for eksempel *.com* eller *.org*, justerer du UPN-suffikset for de lokale brukerkontoene først som beskrevet i [Klargjøre et ikke-rutbart domene for katalogsynkronisering](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="18629-115">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="18629-116">2. Installere og konfigurere Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="18629-116">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="18629-117">Hvis du vil synkronisere brukere, grupper og kontakter fra den lokale Active Directory til Azure Active Directory, installerer du Azure Active Directory Connect og konfigurerer katalogsynkronisering.</span><span class="sxs-lookup"><span data-stu-id="18629-117">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> <span data-ttu-id="18629-118">Se [Konfigurere katalogsynkronisering for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) for å lære mer.</span><span class="sxs-lookup"><span data-stu-id="18629-118">See [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) to learn more.</span></span>

> [!NOTE]
> <span data-ttu-id="18629-119">Trinnene er nøyaktig de samme for Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="18629-119">The steps are exactly the same for Microsoft 365 Business.</span></span> 

<span data-ttu-id="18629-120">Når du konfigurerer alternativene for Azure AD Connect, anbefaler vi at du aktiverer **passordsynkronisering,** **sømløs enkel pålogging**og funksjonen for **passordwriteback,** som også støttes i Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="18629-120">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 Business.</span></span>

> [!NOTE]
> <span data-ttu-id="18629-121">Det er noen ekstra trinn for passordwriteback utover avmerkingsboksen i Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="18629-121">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="18629-122">Hvis du vil ha mer informasjon, kan du se [Slik gjør du det: Konfigurere passordwriteback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="18629-122">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

## <a name="3-configure-hybrid-azure-ad-join"></a><span data-ttu-id="18629-123">3. Konfigurere Hybrid Azure AD-sammenføyning</span><span class="sxs-lookup"><span data-stu-id="18629-123">3. Configure Hybrid Azure AD Join</span></span>

<span data-ttu-id="18629-124">Før du aktiverer Windows 10-enheter til å være Hybrid Azure AD joined, må du kontrollere at du oppfyller følgende forutsetninger:</span><span class="sxs-lookup"><span data-stu-id="18629-124">Before you enable Windows 10 devices to be Hybrid Azure AD joined, make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="18629-125">Du kjører den nyeste versjonen av Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="18629-125">You're running the latest version of Azure AD Connect.</span></span>

   - <span data-ttu-id="18629-126">Azure AD-tilkobling har synkronisert alle datamaskinobjektene for enhetene du vil være hybrid Azure AD sammenføyd.</span><span class="sxs-lookup"><span data-stu-id="18629-126">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="18629-127">Hvis datamaskinobjektene tilhører bestemte organisasjonsenheter (OU), må du kontrollere at disse oUene også er angitt for synkronisering i Azure AD-tilkobling.</span><span class="sxs-lookup"><span data-stu-id="18629-127">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>

<span data-ttu-id="18629-128">Hvis du vil registrere eksisterende domenetilknyttede Windows 10-enheter som Hybrid Azure AD ble med, følger du fremgangsmåten i [opplæringen: Konfigurere hybrid Azure Active Directory-sammenføyning for administrerte domener](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span><span class="sxs-lookup"><span data-stu-id="18629-128">To register existing domain-joined Windows 10 devices as Hybrid Azure AD joined, follow the steps in the [Tutorial: Configure hybrid Azure Active Directory join for managed domains](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="18629-129">Denne hybrid-aktiverer eksisterende lokale Active Directory sammenføyde Windows 10-datamaskiner og gjør dem skyklare.</span><span class="sxs-lookup"><span data-stu-id="18629-129">This hybrid-enables your existing on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a><span data-ttu-id="18629-130">4. Aktivere automatisk registrering for Windows 10</span><span class="sxs-lookup"><span data-stu-id="18629-130">4. Enable automatic enrollment for Windows 10</span></span>

 <span data-ttu-id="18629-131">Hvis du vil registrere Windows 10-enheter for administrasjon av mobilenheter automatisk i Intune, kan du se [Registrere en Windows 10-enhet automatisk ved hjelp av gruppepolicy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span><span class="sxs-lookup"><span data-stu-id="18629-131">To automatically enroll Windows 10 devices for mobile device management in Intune, see [Enroll a Windows 10 device automatically using Group Policy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span></span> <span data-ttu-id="18629-132">Du kan angi gruppepolicyen på et lokalt datamaskinnivå, eller for masseoperasjoner kan du bruke gruppepolicyadministrasjonskonsollen og ADMX-malene til å opprette denne gruppepolicyinnstillingen på domenekontrolleren.</span><span class="sxs-lookup"><span data-stu-id="18629-132">You can set the Group Policy at a local computer level, or for bulk operations, you can use the Group Policy Management Console and ADMX templates to create this Group Policy setting on your Domain Controller.</span></span>

## <a name="5-configure-seamless-single-sign-on"></a><span data-ttu-id="18629-133">5. Konfigurer sømløs enkel pålogging</span><span class="sxs-lookup"><span data-stu-id="18629-133">5. Configure Seamless Single Sign-On</span></span>

  <span data-ttu-id="18629-134">Sømløs SSO logger automatisk brukere inn i sine Microsoft 365-skyressurser når de bruker bedriftsdatamaskiner.</span><span class="sxs-lookup"><span data-stu-id="18629-134">Seamless SSO automatically signs users into their Microsoft 365 cloud resources when they use corporate computers.</span></span> <span data-ttu-id="18629-135">Bare distribuer ett av de to gruppepolicyalternativene som er beskrevet i [Azure Active Directory Seamless Single Sign-On: Hurtigstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span><span class="sxs-lookup"><span data-stu-id="18629-135">Simply deploy one of the two Group Policy options described in [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span></span> <span data-ttu-id="18629-136">Alternativet **Gruppepolicy** tillater ikke brukere å endre innstillingene sine, mens alternativet **Innstillinger for gruppepolicy** angir verdiene, men lar dem også være brukerkonfigurerbare.</span><span class="sxs-lookup"><span data-stu-id="18629-136">The **Group Policy** option doesn't allow users to change their settings, while the **Group Policy Preference** option sets the values but also leaves them user-configurable.</span></span>

## <a name="6-set-up-windows-hello-for-business"></a><span data-ttu-id="18629-137">6. Konfigurere Windows Hello for Business</span><span class="sxs-lookup"><span data-stu-id="18629-137">6. Set up Windows Hello for Business</span></span>

 <span data-ttu-id="18629-138">Windows Hello for Business erstatter passord med sterk tofaktorautentisering (2FA) for å logge på en lokal datamaskin.</span><span class="sxs-lookup"><span data-stu-id="18629-138">Windows Hello for Business replaces passwords with strong two-factor authentication (2FA) for signing into a local computer.</span></span> <span data-ttu-id="18629-139">En faktor er et asymmetrisk nøkkelpar, og den andre er en PIN-kode eller annen lokal bevegelse, for eksempel fingeravtrykk eller ansiktsgjenkjenning hvis enheten støtter den.</span><span class="sxs-lookup"><span data-stu-id="18629-139">One factor is an asymmetric key pair, and the other is a PIN or other local gesture such as fingerprint or facial recognition if your device supports it.</span></span> <span data-ttu-id="18629-140">Vi anbefaler at du erstatter passord med 2FA og Windows Hello for Business der det er mulig.</span><span class="sxs-lookup"><span data-stu-id="18629-140">We recommend that you replace passwords with 2FA and Windows Hello for Business where possible.</span></span>

<span data-ttu-id="18629-141">Hvis du vil konfigurere Hybrid Windows Hello for Bedrifter, kan du se [gjennom Hybrid Key trust Windows Hello for Business Forutsetninger](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span><span class="sxs-lookup"><span data-stu-id="18629-141">To configure Hybrid Windows Hello for Business, review the [Hybrid Key trust Windows Hello for Business Prerequisites](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span></span> <span data-ttu-id="18629-142">Følg deretter instruksjonene i [Konfigurer hybrid Windows Hello for Business nøkkel klareringsinnstillinger](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings).</span><span class="sxs-lookup"><span data-stu-id="18629-142">Then follow the instructions in [Configure Hybrid Windows Hello for Business key trust settings](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings).</span></span> 
