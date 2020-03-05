---
title: Oversikt over oppsett
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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Lær konfigurasjonstrinnene for Microsoft 365 Business, fra å abonnere, legge til et domene og brukere, til å konfigurere sikkerhetspolicyer og mer.
ms.openlocfilehash: 75ef784a886de754e7550d9e86af1242209346dd
ms.sourcegitcommit: d6c871bf3f94d9299d22695f5dbaf25dc1bd6ff9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2020
ms.locfileid: "42417230"
---
# <a name="overview-of-setup"></a><span data-ttu-id="8c101-103">Oversikt over oppsett</span><span class="sxs-lookup"><span data-stu-id="8c101-103">Overview of setup</span></span>

<span data-ttu-id="8c101-104">Se en kort video om installasjonsprogrammet for Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="8c101-104">Watch a short video about Microsoft 365 Business setup.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

<span data-ttu-id="8c101-105">Hvis du synes at denne videoen er nyttig, kan du se den [fullstendige opplæringsserien for små bedrifter og de som er nybegynnere i Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span><span class="sxs-lookup"><span data-stu-id="8c101-105">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).</span></span>

<span data-ttu-id="8c101-106">De fleste konfigurasjonstrinnene kan gjøres i installasjonsveiviseren, men de andre alternativene vises også.</span><span class="sxs-lookup"><span data-stu-id="8c101-106">Most of the setup steps can be done in the setup wizard, but the other options are also listed.</span></span>

## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="8c101-107">Trinn 1: Legg til domenet og brukerne</span><span class="sxs-lookup"><span data-stu-id="8c101-107">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="8c101-108">**[Legg til domenet ditt](set-up.md#add-your-domain-to-personalize-sign-in)** (hvis du kjøpte domenet under [registrering](sign-up.md), er dette trinnet allerede gjort.)</span><span class="sxs-lookup"><span data-stu-id="8c101-108">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="8c101-109">**Legg til brukere**.</span><span class="sxs-lookup"><span data-stu-id="8c101-109">**Add users**.</span></span> <span data-ttu-id="8c101-110">Du kan legge til brukere på en av de tre måtene:</span><span class="sxs-lookup"><span data-stu-id="8c101-110">You can add users in any of the three ways:</span></span>
        - <span data-ttu-id="8c101-111">I [veiviseren](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="8c101-111">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="8c101-112">Bruk katalogsynkronisering til å [legge til brukere ved hjelp av Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) hvis du har en lokal Active-katalog.</span><span class="sxs-lookup"><span data-stu-id="8c101-112">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="8c101-113">Du kan også [legge til brukere senere](add-users-m365b.md) i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="8c101-113">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="8c101-114">Trinn 2: Konfigurere sikkerhetspolicyer og konfigurere enheter</span><span class="sxs-lookup"><span data-stu-id="8c101-114">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="8c101-115">Bruk [installasjonsveiviseren](set-up.md#protect-your-organization) til å konfigurere enhetspolicyer.</span><span class="sxs-lookup"><span data-stu-id="8c101-115">Use the [Setup wizard](set-up.md#protect-your-organization) to configure device policies.</span></span> 
  - <span data-ttu-id="8c101-116">Du kan også legge til flere eller redigere dem senere i [administrasjonssenteret](view-policies-and-devices.md) og i [Intune-portalen](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="8c101-116">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="8c101-117">Installasjonsveiviseren vil også definere grunnleggende innstillinger for trusselbeskyttelse og hindring av tap av data.</span><span class="sxs-lookup"><span data-stu-id="8c101-117">The setup wizard will also set up basic threat protection and data loss prevention settings.</span></span>
  
  <span data-ttu-id="8c101-118">I tillegg til sikkerhetsinnstillingene i installasjonsveiviseren kan du øke sikkerheten ved å legge til følgende innstillinger:</span><span class="sxs-lookup"><span data-stu-id="8c101-118">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

- <span data-ttu-id="8c101-119">**Beskyttelse mot beskyttelse mot beskyttelse mot skadelig programvare for e-**</span><span class="sxs-lookup"><span data-stu-id="8c101-119">**Email malware protection**</span></span>
- <span data-ttu-id="8c101-120">**ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="8c101-120">**ATP anti-phishing**</span></span>
- <span data-ttu-id="8c101-121">**Exchange Online Archiving**</span><span class="sxs-lookup"><span data-stu-id="8c101-121">**Exchange Online Archiving**</span></span>
- <span data-ttu-id="8c101-122">**Azure Information Protection (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="8c101-122">**Azure Information Protection (Plan1**)</span></span>

<span data-ttu-id="8c101-123">Hvis du vil komme i gang, kan du se [Øke trusselbeskyttelsen](increase-threat-protection.md) og [konfigurere samsvarsfunksjoner](set-up-compliance.md).</span><span class="sxs-lookup"><span data-stu-id="8c101-123">To get started, see [increase threat protection](increase-threat-protection.md) and [set up compliance features](set-up-compliance.md).</span></span>

<span data-ttu-id="8c101-124">Se også [topp 10 måter å sikre Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for et veikart over anbefalte sikkerhetsfremgangsmåter.</span><span class="sxs-lookup"><span data-stu-id="8c101-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="8c101-125">Trinn 3: Konfigurere og administrere Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="8c101-125">Step 3: Set up and manage Windows 10 devices</span></span>

<span data-ttu-id="8c101-126">Når du har kjørt oppsettveiviseren, vil du ønske å proctect alle Windwos 10 datamaskiner i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="8c101-126">After you run the set up wizard, you will want to proctect all the Windwos 10 computers in your organization.</span></span>
  
- <span data-ttu-id="8c101-127">Windows 10 Pro er en [forutsetning](pre-requisites-for-data-protection.md) for Microsoft 365 Business, men hvis du har Windows 7 Pro, Windows 8 Pro eller Windows 8.1 Pro, gir abonnementet deg rett til en [oppgradering til Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="8c101-127">Windows 10 Pro is a [prerequisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
- <span data-ttu-id="8c101-128">Følg trinnene i [sikre Windows 10-PCer](secure-win-10-pcs.md) for å definere policyer for Windows 10-enheter.</span><span class="sxs-lookup"><span data-stu-id="8c101-128">Follow the steps in [secure Windows 10 PCs](secure-win-10-pcs.md) to set up policies for Windows 10 devices.</span></span>

<span data-ttu-id="8c101-129">Når du blir med i en Windows 10-enhet i Azure AD, blir policyene du angir for Windows 10-datamaskiner, brukt på den.</span><span class="sxs-lookup"><span data-stu-id="8c101-129">When you join a Windows 10 device to Azure AD, the policies you set for Windows 10 computers get applied to it.</span></span> <span data-ttu-id="8c101-130">Hvis du vil ha mer informasjon, kan du se [Konfigurere Windows-enheter for Brukere av Microsoft 365 Business](set-up-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="8c101-130">For more information, see [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md).</span></span>

## <a name="step-4-install-office-365-business"></a><span data-ttu-id="8c101-131">Trinn 4: Installere Office 365 Business</span><span class="sxs-lookup"><span data-stu-id="8c101-131">Step 4: Install Office 365 Business</span></span>
- <span data-ttu-id="8c101-132">Du kan installere Office automatisk i Windows-enhetene ved hjelp av [installasjonsveiviseren](set-up.md#deploy-office-365-client-apps).</span><span class="sxs-lookup"><span data-stu-id="8c101-132">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="8c101-133">La brukere [installere Office-apper](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows og enheter.</span><span class="sxs-lookup"><span data-stu-id="8c101-133">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="8c101-134">Avansert</span><span class="sxs-lookup"><span data-stu-id="8c101-134">Advanced</span></span>
- <span data-ttu-id="8c101-135">**Bruk Autopilot til å konfigurere nye enheter**</span><span class="sxs-lookup"><span data-stu-id="8c101-135">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="8c101-136">Du kan bruke [Windows Autopilot](add-autopilot-devices-and-profile.md) til å forhåndskonfigurere **nye** Windows 10-enheter for en bruker automatisk, men det kan være enklere å få en [partner](https://www.microsoft.com/solution-providers/search) som kan gjøre dette for deg.</span><span class="sxs-lookup"><span data-stu-id="8c101-136">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="8c101-137">Du kan også gå til [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), og be en skyteknologiekspert om å konfigurere nye enheter du kjøper.</span><span class="sxs-lookup"><span data-stu-id="8c101-137">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), and ask a cloud technology expert to set up new devices that you purchase.</span></span>

- <span data-ttu-id="8c101-138">**Få tilgang til lokale ressurser**</span><span class="sxs-lookup"><span data-stu-id="8c101-138">**Access on-premises resources**</span></span>

     - <span data-ttu-id="8c101-139">Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business til å beskytte Windows 10-enheter, samtidig som du opprettholder tilgangtil lokale ressurser som krever lokal godkjenning.</span><span class="sxs-lookup"><span data-stu-id="8c101-139">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="8c101-140">Følg trinnene i [Aktiver domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business](manage-windows-devices.md) for å konfigurere dette.</span><span class="sxs-lookup"><span data-stu-id="8c101-140">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="8c101-141">Dette er den foretrukne metoden, og enheter i denne tilstanden kalles Hybrid Azure AD-tilknyttede enheter.</span><span class="sxs-lookup"><span data-stu-id="8c101-141">This is the preferred method, and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="8c101-142">Hvis bedriften din har en lokal Active Directory som inneholder noen lokale ressurser (for eksempel fildelinger og skrivere), kan du gi Azure AD-tilknyttede enheter tilgang til disse ressursene ved å følge trinnene her: [Få tilgang til lokale ressurser fra en Azure AD-tilknyttet enhet i Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="8c101-142">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers), you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="8c101-143">Se også</span><span class="sxs-lookup"><span data-stu-id="8c101-143">See also</span></span>

[<span data-ttu-id="8c101-144">Opplæringsvideoer for Microsoft 365-bedrifter</span><span class="sxs-lookup"><span data-stu-id="8c101-144">Microsoft 365 Business training videos</span></span>](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
