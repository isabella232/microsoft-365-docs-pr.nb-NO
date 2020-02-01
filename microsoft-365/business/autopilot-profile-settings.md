---
title: Om innstillinger for AutoPilot-profil
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
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
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: AutoPilot-profiler hjelper deg med å kontrollere hvordan Windows blir installert på brukerenheter. Profilene inneholder standard- og valgfrie innstillinger som hopp over Cortana-installasjonen.
ms.openlocfilehash: 1cc8a3171bbc4a1e5cb531b9364c7791586fc339
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593337"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="086c1-104">Om innstillinger for AutoPilot-profil</span><span class="sxs-lookup"><span data-stu-id="086c1-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="086c1-105">Innstillinger for AutoPilot-profil</span><span class="sxs-lookup"><span data-stu-id="086c1-105">AutoPilot profile settings</span></span>

<span data-ttu-id="086c1-106">Du kan bruke AutoPilot-profiler til å kontrollere hvordan Windows er installert på brukerenheter.</span><span class="sxs-lookup"><span data-stu-id="086c1-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="086c1-107">Profilene inneholder følgende innstillinger.</span><span class="sxs-lookup"><span data-stu-id="086c1-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="086c1-108">**AutoPilot standardfunksjoner (obligatorisk) som angis automatisk:**</span><span class="sxs-lookup"><span data-stu-id="086c1-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="086c1-109">**Innstilling**</span><span class="sxs-lookup"><span data-stu-id="086c1-109">**Setting**</span></span>|<span data-ttu-id="086c1-110">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="086c1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="086c1-111">Hopp over Cortana-, OneDrive- og OEM-registrering</span><span class="sxs-lookup"><span data-stu-id="086c1-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="086c1-112">Hopper over installasjonen av forbrukerapper som Cortana og personlig OneDrive.</span><span class="sxs-lookup"><span data-stu-id="086c1-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="086c1-113">Enhetsbrukeren kan installere disse senere så lenge brukeren er en lokal administrator på enheten.</span><span class="sxs-lookup"><span data-stu-id="086c1-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="086c1-114">Den opprinnelige produsenten registrering en hoppes over fordi enheten vil bli administrert av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="086c1-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="086c1-115">Logg på erfaring med bedriftens merkevare</span><span class="sxs-lookup"><span data-stu-id="086c1-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="086c1-116">Hvis firmaet har en Legg til firmamerking en [påloggingsside for Office 365](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), får enhetsbrukeren denne opplevelsen når du logger på.</span><span class="sxs-lookup"><span data-stu-id="086c1-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="086c1-117">MDM automatisk registrering med konfigurerte AAD-kontoer.</span><span class="sxs-lookup"><span data-stu-id="086c1-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="086c1-118">Brukeridentiteten administreres av Azure Active Directory, og brukere logger på Windows og Office 365 med legitimasjonen for Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="086c1-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="086c1-119">**Valgfrie innstillinger:**</span><span class="sxs-lookup"><span data-stu-id="086c1-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="086c1-120">**Innstilling**</span><span class="sxs-lookup"><span data-stu-id="086c1-120">**Setting**</span></span>|<span data-ttu-id="086c1-121">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="086c1-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="086c1-122">Hopp over personverninnstillinger (Av som standard)</span><span class="sxs-lookup"><span data-stu-id="086c1-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="086c1-123">Hvis dette alternativet er satt til **På**, vil enhetsbrukeren ikke se lisensavtalen for enheten og Windows når han eller hun først logger på.</span><span class="sxs-lookup"><span data-stu-id="086c1-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="086c1-124">Ikke la brukeren bli den lokale administratoren</span><span class="sxs-lookup"><span data-stu-id="086c1-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="086c1-125">Hvis dette alternativet er satt til **På**, kan ikke enhetsbrukeren installere personlige apper, for eksempel Cortana.</span><span class="sxs-lookup"><span data-stu-id="086c1-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
   
