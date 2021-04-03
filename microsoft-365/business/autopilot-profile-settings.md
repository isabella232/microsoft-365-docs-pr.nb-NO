---
title: Om innstillinger for AutoPilot-profil
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: AutoPilot-profiler hjelper deg med å kontrollere hvordan Windows blir installert på brukerenheter. Profilene inneholder standardinnstillinger og valgfrie innstillinger, for eksempel hopp over Cortana-installasjonen.
ms.openlocfilehash: 86f8718131f0a0b93e18e65e39e02e7d65aded1a
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578511"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="ef719-104">Om innstillinger for AutoPilot-profil</span><span class="sxs-lookup"><span data-stu-id="ef719-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="ef719-105">Innstillinger for AutoPilot-profil</span><span class="sxs-lookup"><span data-stu-id="ef719-105">AutoPilot profile settings</span></span>

<span data-ttu-id="ef719-106">Du kan bruke AutoPilot-profiler til å kontrollere hvordan Windows er installert på brukerenheter.</span><span class="sxs-lookup"><span data-stu-id="ef719-106">You can use AutoPilot profiles to control how Windows is installed on user devices.</span></span> <span data-ttu-id="ef719-107">Profilene inneholder følgende innstillinger.</span><span class="sxs-lookup"><span data-stu-id="ef719-107">The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="ef719-108">**AutoPilot-standardfunksjoner (obligatorisk) som angis automatisk:**</span><span class="sxs-lookup"><span data-stu-id="ef719-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="ef719-109">**Innstilling**</span><span class="sxs-lookup"><span data-stu-id="ef719-109">**Setting**</span></span>|<span data-ttu-id="ef719-110">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="ef719-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ef719-111">Hopp over Cortana-, OneDrive- og OEM-registrering</span><span class="sxs-lookup"><span data-stu-id="ef719-111">Skip Cortana, OneDrive, and OEM registration</span></span>  <br/> |<span data-ttu-id="ef719-112">Hopper over installasjonen av forbrukerapper som Cortana og personlig OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ef719-112">Skips the installation of consumer apps like Cortana and personal OneDrive.</span></span> <span data-ttu-id="ef719-113">Enhetsbrukeren kan installere disse senere så lenge brukeren er lokal administrator på enheten.</span><span class="sxs-lookup"><span data-stu-id="ef719-113">The device user can install these later as long as the user is a local admin on the device.</span></span> <span data-ttu-id="ef719-114">Den opprinnelige produsentregistreringen hoppes over fordi enheten administreres av Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="ef719-114">The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="ef719-115">Logg på-opplevelsen med firmamerket ditt</span><span class="sxs-lookup"><span data-stu-id="ef719-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="ef719-116">Hvis firmaet har siden Legg til firmamerking i [Påloggingsside for Microsoft 365,](../admin/setup/customize-sign-in-page.md)får enhetsbrukeren denne opplevelsen når du logger på.</span><span class="sxs-lookup"><span data-stu-id="ef719-116">If your company has a [Add your company branding to Microsoft 365 Sign In page](../admin/setup/customize-sign-in-page.md), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="ef719-117">MDM automatisk registrering med konfigurerte AAD-kontoer.</span><span class="sxs-lookup"><span data-stu-id="ef719-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="ef719-118">Brukeridentiteten administreres av Azure Active Directory, og brukere logger seg på Windows og Microsoft 365 med microsoft 365 Business Premium-legitimasjonen sin.</span><span class="sxs-lookup"><span data-stu-id="ef719-118">The user identity will be managed by Azure Active Directory, and users will sign in to Windows and Microsoft 365 with their Microsoft 365 Business Premium credentials.</span></span>  <br/> |
   
 <span data-ttu-id="ef719-119">**Valgfrie innstillinger:**</span><span class="sxs-lookup"><span data-stu-id="ef719-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="ef719-120">**Innstilling**</span><span class="sxs-lookup"><span data-stu-id="ef719-120">**Setting**</span></span>|<span data-ttu-id="ef719-121">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="ef719-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ef719-122">Hopp over personverninnstillinger (av som standard)</span><span class="sxs-lookup"><span data-stu-id="ef719-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="ef719-123">Hvis dette alternativet er satt til **På**, vil ikke enhetsbrukeren se lisensavtalen for enheten og Windows når han eller hun logger på for første gang.</span><span class="sxs-lookup"><span data-stu-id="ef719-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="ef719-124">Ikke tillat brukeren å bli lokal administrator</span><span class="sxs-lookup"><span data-stu-id="ef719-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="ef719-125">Hvis dette alternativet er satt til **På**, kan ikke enhetsbrukeren installere noen personlige apper, for eksempel Cortana.</span><span class="sxs-lookup"><span data-stu-id="ef719-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span><br/> |
