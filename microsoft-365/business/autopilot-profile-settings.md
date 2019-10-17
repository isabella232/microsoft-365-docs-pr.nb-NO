---
title: Om innstillinger for AutoPilot-profil
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
description: AutoPilot-profiler hjelper deg med å kontrollere hvordan Windows blir installert på bruker enheter. Profilene inneholder standard og valgfrie innstillinger, for eksempel hopp over Cortana-installasjon.
ms.openlocfilehash: eb0d9a95c796909d024db1d061aaeace7d07ed1b
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/17/2019
ms.locfileid: "37574582"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="68799-104">Om innstillinger for AutoPilot-profil</span><span class="sxs-lookup"><span data-stu-id="68799-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="68799-105">Innstillinger for AutoPilot-profilen</span><span class="sxs-lookup"><span data-stu-id="68799-105">AutoPilot profile settings</span></span>

<span data-ttu-id="68799-106">Du kan kontrollere hvordan Windows blir installert på bruker enheter ved å bruke AutoPilot-profilene.</span><span class="sxs-lookup"><span data-stu-id="68799-106">You can control how Windows gets installed on user devices by using the AutoPilot profiles.</span></span> <span data-ttu-id="68799-107">Profilene inneholder følgende innstillinger.</span><span class="sxs-lookup"><span data-stu-id="68799-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="68799-108">**Standard funksjoner for AutoPilot (påkrevd) som stilles inn automatisk:**</span><span class="sxs-lookup"><span data-stu-id="68799-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="68799-109">**Innstilling**</span><span class="sxs-lookup"><span data-stu-id="68799-109">**Setting**</span></span>|<span data-ttu-id="68799-110">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="68799-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="68799-111">Hopp over Cortana, OneDrive og OEM-registrering</span><span class="sxs-lookup"><span data-stu-id="68799-111">Skip Cortana, OneDrive and OEM registration</span></span>  <br/> |<span data-ttu-id="68799-112">Hopper over installasjonen av forbruker programmer som Cortana og personlig OneDrive.</span><span class="sxs-lookup"><span data-stu-id="68799-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="68799-113">Enheten brukeren kan installere disse senere så lenge han eller hun er en lokal admin på enheten.</span><span class="sxs-lookup"><span data-stu-id="68799-113">The device user can install these later as long as he or she is a local admin on the device.</span></span> <span data-ttu-id="68799-114">Den opprinnelige produsenten registreringen er hoppet over fordi enheten vil bli administrert av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="68799-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="68799-115">Logg på erfaring med firmaets merkevare</span><span class="sxs-lookup"><span data-stu-id="68799-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="68799-116">Hvis firmaet har en [Legg til firmaets merkevarebygging til Office 365 påloggingssiden](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), vil enheten brukeren får denne opplevelsen når du logger på.</span><span class="sxs-lookup"><span data-stu-id="68799-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="68799-117">Automatisk MDM-registrering med konfigurerte AAD-kontoer.</span><span class="sxs-lookup"><span data-stu-id="68799-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="68799-118">Bruker identiteten vil bli administrert av Azure Active Directory, og brukerne vil logge på Windows og Office 365 med sine Microsoft 365 Business legitimasjon.</span><span class="sxs-lookup"><span data-stu-id="68799-118">The user identity will be managed by Azure Active directory, and the users will sign into Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="68799-119">**Valgfrie innstillinger:**</span><span class="sxs-lookup"><span data-stu-id="68799-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="68799-120">**Innstilling**</span><span class="sxs-lookup"><span data-stu-id="68799-120">**Setting**</span></span>|<span data-ttu-id="68799-121">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="68799-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="68799-122">Hopp over personverninnstillinger (av som standard)</span><span class="sxs-lookup"><span data-stu-id="68799-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="68799-123">Hvis dette alternativet er satt til **på**, vil ikke enhets brukeren se lisensavtalen for enheten og Windows når han eller hun først logger på.</span><span class="sxs-lookup"><span data-stu-id="68799-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="68799-124">Ikke la brukeren bli den lokale administratoren</span><span class="sxs-lookup"><span data-stu-id="68799-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="68799-125">Hvis dette alternativet er satt til **på**, kan ikke enhets brukeren installere personlige apper, for eksempel Cortana.</span><span class="sxs-lookup"><span data-stu-id="68799-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span>  <br/> |
   
