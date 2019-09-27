---
title: Oversikt over oppsett
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Oversikt over oppsett trinnene for Microsoft 365 Business.
ms.openlocfilehash: f156d236a783942ec06d457c9b7ca087d12d6f58
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288579"
---
# <a name="overview-of-setup"></a><span data-ttu-id="6cf86-103">Oversikt over oppsett</span><span class="sxs-lookup"><span data-stu-id="6cf86-103">Overview of setup</span></span>

<span data-ttu-id="6cf86-104">De fleste av de angitte trinnene kan gjøres i installasjonsveiviseren, men de andre alternativene er også oppført.</span><span class="sxs-lookup"><span data-stu-id="6cf86-104">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>


## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="6cf86-105">Trinn 1: Legg til domenet og brukerne</span><span class="sxs-lookup"><span data-stu-id="6cf86-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="6cf86-106">**[Legg til domenet ditt](set-up.md#add-your-domain-to-personalize-sign-in)** (Hvis du kjøpte domenet under [registreringen](sign-up.md), er dette trinnet allerede gjort.)</span><span class="sxs-lookup"><span data-stu-id="6cf86-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="6cf86-107">**Legge til brukere**.</span><span class="sxs-lookup"><span data-stu-id="6cf86-107">**Add users**.</span></span> <span data-ttu-id="6cf86-108">Du kan gjøre dette på en av de tre måtene:</span><span class="sxs-lookup"><span data-stu-id="6cf86-108">You can do this in any of the three ways:</span></span>
        - <span data-ttu-id="6cf86-109">I [veiviseren](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="6cf86-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="6cf86-110">Bruk katalogsynkronisering for å [legge til brukere ved hjelp av Azure ad-tilkobling](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) hvis du har en lokal Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6cf86-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="6cf86-111">Du kan også [legge til brukere senere](add-users-m365b.md) i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="6cf86-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="6cf86-112">Trinn 2: konfigurere sikkerhetspolicyer og konfigurere enheter</span><span class="sxs-lookup"><span data-stu-id="6cf86-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="6cf86-113">Bruk [installasjonsveiviseren](set-up.md#set-up-security-policies-and-device-configurations) til å konfigurere enhets-og sikkerhetspolicyer.</span><span class="sxs-lookup"><span data-stu-id="6cf86-113">Use the [Setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure device and security policies.</span></span> 
  - <span data-ttu-id="6cf86-114">Du kan også legge til flere eller redigere dem senere i [administrasjonssenteret](view-policies-and-devices.md) og i [Intune-portalen](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="6cf86-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="6cf86-115">I tillegg til sikkerhetsinnstillingene i installasjonsveiviseren kan du øke sikkerheten ved å legge til følgende innstillinger:</span><span class="sxs-lookup"><span data-stu-id="6cf86-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="6cf86-116">**Email malware beskyttelse**</span><span class="sxs-lookup"><span data-stu-id="6cf86-116">**Email malware protection**</span></span>
      - <span data-ttu-id="6cf86-117">**Avanserte trusselbeskyttelse (ATP) sikker linker**</span><span class="sxs-lookup"><span data-stu-id="6cf86-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="6cf86-118">**Sikre vedlegg i ATP**</span><span class="sxs-lookup"><span data-stu-id="6cf86-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="6cf86-119">**ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="6cf86-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="6cf86-120">**Exchange Online Archiving**</span><span class="sxs-lookup"><span data-stu-id="6cf86-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="6cf86-121">**Hindring av tap av data (DLP)**</span><span class="sxs-lookup"><span data-stu-id="6cf86-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="6cf86-122">**Azure informasjonsbeskyttelse (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="6cf86-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="6cf86-123">[Sett opp avanserte sikkerhetspolicyer](set-up-advanced-security.md)for å komme i gang med å se.</span><span class="sxs-lookup"><span data-stu-id="6cf86-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="6cf86-124">Se også [topp 10 måter å sikre din Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for et veikart for beste sikkerhet praksis.</span><span class="sxs-lookup"><span data-stu-id="6cf86-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="6cf86-125">Trinn 3: konfigurere og administrere Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="6cf86-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="6cf86-126">Når du blir med i en Windows 10-enhet til Azure AD, blir policyene du konfigurerer i [trinn 2](#step-2-set-up-security-policies-and-configure-devices) , brukt på den.</span><span class="sxs-lookup"><span data-stu-id="6cf86-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="6cf86-127">Windows 10 Pro er en [forutsetning](pre-requisites-for-data-protection.md) for Microsoft 365 Business, men hvis du har Windows 7 Pro, Windows 8 Pro eller Windows 8,1 Pro, gir abonnementet deg rett til en [oppgradering til Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="6cf86-127">Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="6cf86-128">Bruk [installasjonsveiviseren](set-up.md#set-up-security-policies-and-device-configurations) til å konfigurere policyer for Windows 10-enheter.</span><span class="sxs-lookup"><span data-stu-id="6cf86-128">Use the [setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure policies for Windows 10 devices.</span></span>

## <a name="stes-4-install-office-365-business"></a><span data-ttu-id="6cf86-129">Stes 4: installere Office 365 Business</span><span class="sxs-lookup"><span data-stu-id="6cf86-129">Stes 4: Install Office 365 Business</span></span>
- <span data-ttu-id="6cf86-130">Du kan installere Office automatisk i Windows-enheter ved hjelp av [installasjonsveiviseren](set-up.md#deploy-office-365-client-apps).</span><span class="sxs-lookup"><span data-stu-id="6cf86-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="6cf86-131">Automatisk [installere Office](auto-install-or-uninstall-office.md) fra administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="6cf86-131">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
- <span data-ttu-id="6cf86-132">La brukere [installere Office-apper](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows og enheter.</span><span class="sxs-lookup"><span data-stu-id="6cf86-132">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="6cf86-133">Avansert</span><span class="sxs-lookup"><span data-stu-id="6cf86-133">Advanced</span></span>
- <span data-ttu-id="6cf86-134">**Bruk autopilot til å konfigurere nye enheter**</span><span class="sxs-lookup"><span data-stu-id="6cf86-134">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="6cf86-135">Du kan bruke [Windows autopilot](add-autopilot-devices-and-profile.md) til å forhånds konfigurere **nye** Windows 10-enheter for en bruker automatisk, men det kan være enklere å få en [partner](https://www.microsoft.com/solution-providers/search) som kan gjøre dette for deg.</span><span class="sxs-lookup"><span data-stu-id="6cf86-135">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="6cf86-136">Du kan også gå til [Microsoft store](https://go.microsoft.com/fwlink/?linkid=874598) og be en ekspert på skyteknologi sette opp nye enheter du kjøper for deg.</span><span class="sxs-lookup"><span data-stu-id="6cf86-136">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

- <span data-ttu-id="6cf86-137">**Få tilgang til lokale ressurser**</span><span class="sxs-lookup"><span data-stu-id="6cf86-137">**Access on-premises resources**</span></span>

     - <span data-ttu-id="6cf86-138">Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business for å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgang til lokale ressurser som krever lokal godkjenning.</span><span class="sxs-lookup"><span data-stu-id="6cf86-138">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="6cf86-139">Følg trinnene i [aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business](manage-windows-devices.md) for å konfigurere dette.</span><span class="sxs-lookup"><span data-stu-id="6cf86-139">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="6cf86-140">Dette er den foretrukne metoden og enhetene i denne tilstanden kalles Hybrid Azure AD koblet enheter.</span><span class="sxs-lookup"><span data-stu-id="6cf86-140">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="6cf86-141">Hvis virksomheten har en lokal Active Directory som inneholder noen lokale ressurser (for eksempel delte filressurser og skrivere), kan du gi Azure AD-tilknyttede enheter tilgang til disse ressursene ved å følge fremgangsmåten her: [få tilgang til lokale ressurser fra en Azure AD-sammenkoblet enhet i Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="6cf86-141">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  