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
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Oversikt over satt opp trinnene for Microsoft 365 Business.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086354"
---
# <a name="overview-of-setup"></a><span data-ttu-id="76a21-103">Oversikt over oppsett</span><span class="sxs-lookup"><span data-stu-id="76a21-103">Overview of setup</span></span>

<span data-ttu-id="76a21-104">Det meste av den er satt opp trinnene kan gjøres i installasjonsveiviseren, men de andre alternativene er også oppført.</span><span class="sxs-lookup"><span data-stu-id="76a21-104">Most of the set up steps can be done in the setup wizard, but the other options are also listed.</span></span>


## <a name="step-1-add-your-domain-and-users"></a><span data-ttu-id="76a21-105">Trinn 1: Legge til domenet og brukere</span><span class="sxs-lookup"><span data-stu-id="76a21-105">Step 1: Add your domain and users</span></span>

   - <span data-ttu-id="76a21-106">**[Legg til domenet ditt](set-up.md#add-your-domain-to-personalize-sign-in)** (Hvis du kjøpte domenet ditt ved å [registrere deg](sign-up.md), dette trinnet er allerede har gjort.)</span><span class="sxs-lookup"><span data-stu-id="76a21-106">**[Add your domain](set-up.md#add-your-domain-to-personalize-sign-in)** (if you bought your domain during [sign up](sign-up.md), this step is already done.)</span></span>

    - <span data-ttu-id="76a21-107">**Legg til brukere**.</span><span class="sxs-lookup"><span data-stu-id="76a21-107">**Add users**.</span></span> <span data-ttu-id="76a21-108">Du kan gjøre dette på en av tre måter:</span><span class="sxs-lookup"><span data-stu-id="76a21-108">You can do this in any of the three ways:</span></span>
        - <span data-ttu-id="76a21-109">I [veiviseren](set-up.md#add-users-in-the-wizard).</span><span class="sxs-lookup"><span data-stu-id="76a21-109">In the [wizard](set-up.md#add-users-in-the-wizard).</span></span>
        - <span data-ttu-id="76a21-110">Bruk katalogsynkronisering for å [legge til brukere ved hjelp av Azure AD-tilkobling](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) Hvis du har en lokale Active directory.</span><span class="sxs-lookup"><span data-stu-id="76a21-110">Use directory synchronization to [add users by using Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) if you have an on-premises Active directory.</span></span>
        - <span data-ttu-id="76a21-111">Du kan også [legge til senere brukere](add-users-m365b.md) i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="76a21-111">You can also [add users later](add-users-m365b.md) in the admin center.</span></span>
## <a name="step-2-set-up-security-policies-and-configure-devices"></a><span data-ttu-id="76a21-112">Trinn 2: Konfigurere sikkerhetspolicyer og konfigurere enheter</span><span class="sxs-lookup"><span data-stu-id="76a21-112">Step 2: Set up security policies and configure devices</span></span> 

  - <span data-ttu-id="76a21-113">Bruke [veiviseren for installasjon](set-up.md#set-up-security-policies-and-device-configurations) til å konfigurere enheten og sikkerhetspolicy.</span><span class="sxs-lookup"><span data-stu-id="76a21-113">Use the [Setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure device and security policies.</span></span> 
  - <span data-ttu-id="76a21-114">Du kan også legge til flere eller redigere dem senere i [administrasjonssenteret](view-policies-and-devices.md) og [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span><span class="sxs-lookup"><span data-stu-id="76a21-114">You can also add more or edit them later in the [admin center](view-policies-and-devices.md) and in the [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).</span></span>
  - <span data-ttu-id="76a21-115">I tillegg til sikkerhetsinnstillingene i veiviseren, kan du øke sikkerheten ved å legge til følgende innstillinger:</span><span class="sxs-lookup"><span data-stu-id="76a21-115">In addition to the security settings in the setup wizard, you can increase your security by adding the following settings:</span></span>

      - <span data-ttu-id="76a21-116">**Beskyttelse mot skadelig programvare for e-post**</span><span class="sxs-lookup"><span data-stu-id="76a21-116">**Email malware protection**</span></span>
      - <span data-ttu-id="76a21-117">**Avanserte Threat Protection (ATP) sikre koblinger**</span><span class="sxs-lookup"><span data-stu-id="76a21-117">**Advanced Threat Protection (ATP) Safe links**</span></span>
      - <span data-ttu-id="76a21-118">**ATP-Safe vedlegg**</span><span class="sxs-lookup"><span data-stu-id="76a21-118">**ATP Safe Attachments**</span></span>
      - <span data-ttu-id="76a21-119">**ATP anti-phishing**</span><span class="sxs-lookup"><span data-stu-id="76a21-119">**ATP anti-phishing**</span></span>
      - <span data-ttu-id="76a21-120">**Exchange Online Archiving**</span><span class="sxs-lookup"><span data-stu-id="76a21-120">**Exchange Online Archiving**</span></span>
      - <span data-ttu-id="76a21-121">**Data tap forebygging (DLP)**</span><span class="sxs-lookup"><span data-stu-id="76a21-121">**Data Loss Prevention (DLP)**</span></span>
      - <span data-ttu-id="76a21-122">**Azure informasjonsbeskyttelse (Plan1**)</span><span class="sxs-lookup"><span data-stu-id="76a21-122">**Azure Information Protection (Plan1**)</span></span>

          <span data-ttu-id="76a21-123">Å komme i gang, kan du se [konfigurere avanserte sikkerhetspolicyer](set-up-advanced-security.md).</span><span class="sxs-lookup"><span data-stu-id="76a21-123">To get started see, [set up advanced security policies](set-up-advanced-security.md).</span></span>

        <span data-ttu-id="76a21-124">Se også [topp 10 måter å sikre bedriften din Microsoft-365](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for et veikart for gode fremgangsmåter for sikkerhet.</span><span class="sxs-lookup"><span data-stu-id="76a21-124">See also [top 10 ways to secure your Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for a roadmap of best security practices.</span></span>

## <a name="step-3-set-up-and-manage-windows-10-devices"></a><span data-ttu-id="76a21-125">Trinn 3: Konfigurere og administrere Windows 10 enheter</span><span class="sxs-lookup"><span data-stu-id="76a21-125">Step 3: Set up and manage Windows 10 devices</span></span>

   <span data-ttu-id="76a21-126">Når du slår sammen en enhet for Windows 10 Azure AD, policyene du har angitt i [trinn 2](#step-2-set-up-security-policies-and-configure-devices) , brukes den.</span><span class="sxs-lookup"><span data-stu-id="76a21-126">When you join a Windows 10 device to Azure AD, the policies you set up in [Step 2](#step-2-set-up-security-policies-and-configure-devices) get applied to it.</span></span>

   - <span data-ttu-id="76a21-127">Windows 10 Pro er en [forutsetning](pre-requisites-for-data-protection.md) for Microsoft 365 Business, men hvis du har Windows 7 Pro, Windows 8 Pro eller Windows 8.1 Pro, abonnementet sikrer deg en [oppgradering til Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span><span class="sxs-lookup"><span data-stu-id="76a21-127">Windows 10 Pro is a [pre-requisite](pre-requisites-for-data-protection.md) for Microsoft 365 Business, but if you have Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your subscription entitles you to an [upgrade to  Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).</span></span>
    - <span data-ttu-id="76a21-128">Bruk [veiviseren](set-up.md#set-up-security-policies-and-device-configurations) til å konfigurere policyer for Windows 10 enheter.</span><span class="sxs-lookup"><span data-stu-id="76a21-128">Use the [setup wizard](set-up.md#set-up-security-policies-and-device-configurations) to configure policies for Windows 10 devices.</span></span>

## <a name="stes-4-install-office-365-business"></a><span data-ttu-id="76a21-129">Stes 4: Installere Office 365-Business</span><span class="sxs-lookup"><span data-stu-id="76a21-129">Stes 4: Install Office 365 Business</span></span>
- <span data-ttu-id="76a21-130">Du kan installere Office automatisk i Windows-enheter ved hjelp av [installasjonsveiviseren](set-up.md#deploy-office-365-client-apps).</span><span class="sxs-lookup"><span data-stu-id="76a21-130">You can automatically install Office in the Windows devices by using the [setup wizard](set-up.md#deploy-office-365-client-apps).</span></span>
- <span data-ttu-id="76a21-131">Automatisk [installerer Office](auto-install-or-uninstall-office.md) fra administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="76a21-131">Automatically [install Office](auto-install-or-uninstall-office.md) from the admin center.</span></span>
- <span data-ttu-id="76a21-132">La brukere [installere Office-programmer](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows og enheter.</span><span class="sxs-lookup"><span data-stu-id="76a21-132">Let users [install Office apps](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows and devices.</span></span>
     
## <a name="advanced"></a><span data-ttu-id="76a21-133">Avansert</span><span class="sxs-lookup"><span data-stu-id="76a21-133">Advanced</span></span>
- <span data-ttu-id="76a21-134">**Bruk Autopilot til å definere nye enheter**</span><span class="sxs-lookup"><span data-stu-id="76a21-134">**Use Autopilot to set up new devices**</span></span>
            
     <span data-ttu-id="76a21-135">Du kan bruke [Windows Autopilot](add-autopilot-devices-and-profile.md) å automatisk forhåndskonfigurere **nye** Windows 10 enheter for en bruker, men det kan være enklere å få en [partner](https://www.microsoft.com/solution-providers/search) som kan gjøre dette for deg.</span><span class="sxs-lookup"><span data-stu-id="76a21-135">You can use [Windows Autopilot](add-autopilot-devices-and-profile.md) to automatically pre-configure **new** Windows 10 devices for a user, but it might be easier to get a [partner](https://www.microsoft.com/solution-providers/search) who can do this for you.</span></span> <span data-ttu-id="76a21-136">Du kan også gå til [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) og be om en sky teknologi ekspert definere nye enheter du kjøpe for deg.</span><span class="sxs-lookup"><span data-stu-id="76a21-136">You can also go to [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) and ask a cloud technology expert set up new devices you purchase for you.</span></span>

- <span data-ttu-id="76a21-137">**Få tilgang til lokale ressurser**</span><span class="sxs-lookup"><span data-stu-id="76a21-137">**Access on-premises resources**</span></span>

     - <span data-ttu-id="76a21-138">Hvis organisasjonen bruker Windows Server Active Directory på lokaler, kan du definere Microsoft 365 Business til å beskytte Windows 10 enheter, samtidig som du har tilgang til lokale ressurser som krever lokal godkjenning.</span><span class="sxs-lookup"><span data-stu-id="76a21-138">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="76a21-139">Følg trinnene i [aktivere domenetilknyttede Windows 10 enheter som skal administreres av Microsoft 365 Business](manage-windows-devices.md) å sette opp dette.</span><span class="sxs-lookup"><span data-stu-id="76a21-139">Follow the steps in [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business](manage-windows-devices.md) to set this up.</span></span> <span data-ttu-id="76a21-140">Dette er den foretrukne metoden og enheter i denne tilstanden kalles Hybrid Azure AD koblet enheter.</span><span class="sxs-lookup"><span data-stu-id="76a21-140">This is the preferred method and devices in this state are called Hybrid Azure AD joined devices.</span></span>

    - <span data-ttu-id="76a21-141">Hvis firmaet har en lokal Active Directory, som inneholder noen lokale ressurser (for eksempel delte filer og skrivere), kan du gi din Azure AD-koblet enheter tilgang til disse ressursene ved å følge fremgangsmåten her: [Access lokale ressurser fra en Azure AD-koblet enheten i Microsoft 365 Business](access-resources.md).</span><span class="sxs-lookup"><span data-stu-id="76a21-141">If your business has a local Active Directory that contains some on-premises resources (such as file shares and printers) , you can give your Azure AD-joined devices access to these resources by following the steps here: [Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business](access-resources.md).</span></span>

  