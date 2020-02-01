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
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Lær hvordan du aktiverer Microsoft 365 for å beskytte lokale Active Directory-tilknyttede Windows 10-enheter.
ms.openlocfilehash: 170703c7367f9c0e9cb4c10edbd81cb214aa1d3e
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593805"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="3d969-103">Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="3d969-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="3d969-104">Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business til å beskytte Windows 10-enheter, samtidig som du opprettholder tilgangtil lokale ressurser som krever lokal godkjenning.</span><span class="sxs-lookup"><span data-stu-id="3d969-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="3d969-105">Hvis du vil konfigurere denne beskyttelsen, kan du implementere **Hybrid Azure AD-sammenkoblede enheter**.</span><span class="sxs-lookup"><span data-stu-id="3d969-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="3d969-106">Disse enhetene er koblet til både den lokale Active Directory og Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3d969-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="3d969-107">Denne videoen beskriver fremgangsmåten for hvordan du konfigurerer dette for det vanligste scenariet, som også er beskrevet i trinnene som følger.</span><span class="sxs-lookup"><span data-stu-id="3d969-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="3d969-108">1. Klargjør for katalogsynkronisering</span><span class="sxs-lookup"><span data-stu-id="3d969-108">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="3d969-109">Før du synkroniserer brukere og datamaskiner fra det lokale Active Directory-domenet, kan du se [Klargjøre for katalogsynkronisering til Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="3d969-109">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="3d969-110">Spesielt:</span><span class="sxs-lookup"><span data-stu-id="3d969-110">In particular:</span></span>

   - <span data-ttu-id="3d969-111">Kontroller at det ikke finnes noen duplikater i katalogen for følgende attributter: **e-post**, **proxyAddresses**og **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="3d969-111">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="3d969-112">Disse verdiene må være unike, og eventuelle duplikater må fjernes.</span><span class="sxs-lookup"><span data-stu-id="3d969-112">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="3d969-113">Vi anbefaler at du konfigurerer **attributtet userPrincipalName** (UPN) for hver lokale brukerkonto slik at den samsvarer med den primære e-postadressen som tilsvarer den lisensierte Microsoft 365-brukeren.</span><span class="sxs-lookup"><span data-stu-id="3d969-113">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="3d969-114">For eksempel: *mary.shelley@contoso.com* i stedet for *mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="3d969-114">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="3d969-115">Hvis Active Directory-domenet slutter i et ikke-rutbart suffiks som *.local* eller *.lan*, i stedet for et internet routable suffiks som *.com* eller *.org*, justerer DU UPN-suffikset for de lokale brukerkontoene først som beskrevet i [Klargjøre et ikke-routable-domene for katalogsynkronisering](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="3d969-115">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="3d969-116">2. Installer og konfigurer Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="3d969-116">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="3d969-117">Hvis du vil synkronisere brukere, grupper og kontakter fra den lokale Active Directory til Azure Active Directory, installerer du Azure Active Directory Connect og konfigurerer katalogsynkronisering.</span><span class="sxs-lookup"><span data-stu-id="3d969-117">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> <span data-ttu-id="3d969-118">Se [Konfigurere katalogsynkronisering for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) for å finne ut mer.</span><span class="sxs-lookup"><span data-stu-id="3d969-118">See [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) to learn more.</span></span>

> [!NOTE]
> <span data-ttu-id="3d969-119">Trinnene er nøyaktig de samme for Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="3d969-119">The steps are exactly the same for Microsoft 365 Business.</span></span> 

<span data-ttu-id="3d969-120">Når du konfigurerer alternativene for Azure AD Connect, anbefaler vi at du aktiverer **synkronisering av passord**, sømløs enkel **pålogging**og funksjonen for **passordskriving,** som også støttes i Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="3d969-120">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 Business.</span></span>

> [!NOTE]
> <span data-ttu-id="3d969-121">Det er noen flere trinn for passordwriteback utover avmerkingsboksen i Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="3d969-121">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="3d969-122">Hvis du vil ha mer informasjon, kan du se [Slik konfigurerer du passordwriteback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="3d969-122">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

## <a name="3-configure-hybrid-azure-ad-join"></a><span data-ttu-id="3d969-123">3. Konfigurer Hybrid Azure AD Join</span><span class="sxs-lookup"><span data-stu-id="3d969-123">3. Configure Hybrid Azure AD Join</span></span>

<span data-ttu-id="3d969-124">Før du aktiverer Windows 10-enheter som Hybrid Azure AD, må du kontrollere at du oppfyller følgende forutsetninger:</span><span class="sxs-lookup"><span data-stu-id="3d969-124">Before you enable Windows 10 devices to be Hybrid Azure AD joined, make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="3d969-125">Du kjører den nyeste versjonen av Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="3d969-125">You're running the latest version of Azure AD Connect.</span></span>

   - <span data-ttu-id="3d969-126">Azure AD connect har synkronisert alle datamaskinobjektene til enhetene du vil være hybrid Azure AD sluttet.</span><span class="sxs-lookup"><span data-stu-id="3d969-126">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="3d969-127">Hvis datamaskinobjektene tilhører bestemte organisasjonsenheter (OU), må du kontrollere at disse oUene også er angitt for synkronisering i Azure AD-tilkobling.</span><span class="sxs-lookup"><span data-stu-id="3d969-127">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>

<span data-ttu-id="3d969-128">Hvis du vil registrere eksisterende domenetilknyttede Windows 10-enheter som Hybrid Azure AD ble koblet til, følger du fremgangsmåten i [opplæringen: Konfigurere hybrid Azure Active Directory-sammenføyning for administrerte domener](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span><span class="sxs-lookup"><span data-stu-id="3d969-128">To register existing domain-joined Windows 10 devices as Hybrid Azure AD joined, follow the steps in the [Tutorial: Configure hybrid Azure Active Directory join for managed domains](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="3d969-129">Denne hybrid-aktiverer eksisterende lokale Active Directory sluttet Windows 10 datamaskiner og gjøre dem skyklar.</span><span class="sxs-lookup"><span data-stu-id="3d969-129">This hybrid-enables your existing on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a><span data-ttu-id="3d969-130">4. Aktiver automatisk registrering for Windows 10</span><span class="sxs-lookup"><span data-stu-id="3d969-130">4. Enable automatic enrollment for Windows 10</span></span>

 <span data-ttu-id="3d969-131">Hvis du vil registrere Windows 10-enheter automatisk for administrasjon av mobilenheter i Intune, kan du se [Registrere en Windows 10-enhet automatisk ved hjelp av gruppepolicy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span><span class="sxs-lookup"><span data-stu-id="3d969-131">To automatically enroll Windows 10 devices for mobile device management in Intune, see [Enroll a Windows 10 device automatically using Group Policy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy).</span></span> <span data-ttu-id="3d969-132">Du kan angi gruppepolicyen på lokalt datamaskinnivå, eller for masseoperasjoner, du kan bruke maler for gruppepolicybehandling og ADMX til å opprette denne gruppepolicyinnstillingen på domenekontrolleren.</span><span class="sxs-lookup"><span data-stu-id="3d969-132">You can set the Group Policy at a local computer level, or for bulk operations, you can use the Group Policy Management Console and ADMX templates to create this Group Policy setting on your Domain Controller.</span></span>

## <a name="5-configure-seamless-single-sign-on"></a><span data-ttu-id="3d969-133">5. Konfigurer sømløs enkel pålogging</span><span class="sxs-lookup"><span data-stu-id="3d969-133">5. Configure Seamless Single Sign-On</span></span>

  <span data-ttu-id="3d969-134">Sømløs SSO signerer automatisk brukere i Microsoft 365-skyressursene når de bruker firmadatamaskiner.</span><span class="sxs-lookup"><span data-stu-id="3d969-134">Seamless SSO automatically signs users into their Microsoft 365 cloud resources when they use corporate computers.</span></span> <span data-ttu-id="3d969-135">Bare distribuer ett av de to gruppepolicyalternativene som er beskrevet i [Azure Active Directory Seamless Single Sign-On: Hurtigstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span><span class="sxs-lookup"><span data-stu-id="3d969-135">Simply deploy one of the two Group Policy options described in [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature).</span></span> <span data-ttu-id="3d969-136">**Alternativet Gruppepolicy** tillater ikke brukere å endre innstillingene sine, mens alternativet **Gruppepolicyinnstilling** angir verdiene, men lar dem også konfigureres.</span><span class="sxs-lookup"><span data-stu-id="3d969-136">The **Group Policy** option doesn't allow users to change their settings, while the **Group Policy Preference** option sets the values but also leaves them user-configurable.</span></span>

## <a name="6-set-up-windows-hello-for-business"></a><span data-ttu-id="3d969-137">6. Konfigurere Windows Hello for Bedrifter</span><span class="sxs-lookup"><span data-stu-id="3d969-137">6. Set up Windows Hello for Business</span></span>

 <span data-ttu-id="3d969-138">Windows Hello for Business erstatter passord med sterk tofaktorautentisering (2FA) for å logge på en lokal datamaskin.</span><span class="sxs-lookup"><span data-stu-id="3d969-138">Windows Hello for Business replaces passwords with strong two-factor authentication (2FA) for signing into a local computer.</span></span> <span data-ttu-id="3d969-139">Den ene faktoren er et asymmetrisk nøkkelpar, og det andre er en PIN-kode eller annen lokal bevegelse, for eksempel fingeravtrykk eller ansiktsgjenkjenning hvis enheten støtter den.</span><span class="sxs-lookup"><span data-stu-id="3d969-139">One factor is an asymmetric key pair, and the other is a PIN or other local gesture such as fingerprint or facial recognition if your device supports it.</span></span> <span data-ttu-id="3d969-140">Vi anbefaler at du erstatter passord med 2FA og Windows Hello for Business der det er mulig.</span><span class="sxs-lookup"><span data-stu-id="3d969-140">We recommend that you replace passwords with 2FA and Windows Hello for Business where possible.</span></span>

<span data-ttu-id="3d969-141">Hvis du vil konfigurere Hybrid Windows Hello for Bedrifter, kan du se [hybridnøkkelklareringWindows Hello for Business Prerequisites](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span><span class="sxs-lookup"><span data-stu-id="3d969-141">To configure Hybrid Windows Hello for Business, review the [Hybrid Key trust Windows Hello for Business Prerequisites](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs).</span></span> <span data-ttu-id="3d969-142">Følg deretter instruksjonene i [Konfigurere innstillinger for hybrid Windows Hello for Business-nøkkelklarering](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings).</span><span class="sxs-lookup"><span data-stu-id="3d969-142">Then follow the instructions in [Configure Hybrid Windows Hello for Business key trust settings](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings).</span></span> 
