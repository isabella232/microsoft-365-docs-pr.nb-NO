---
title: Om innstillinger for AutoPilot-profil
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: AutoPilot profiler hjelper deg med å styre hvordan Windows blir installert på Brukerenheter. Profilene inneholder standard og valgfrie innstillinger som hopper Cortana installasjon.
ms.openlocfilehash: 5440286f1363780c87ab60514584c4addfeea0b2
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982246"
---
# <a name="about-autopilot-profile-settings"></a><span data-ttu-id="97aaa-104">Om innstillinger for AutoPilot-profil</span><span class="sxs-lookup"><span data-stu-id="97aaa-104">About AutoPilot Profile settings</span></span>

## <a name="autopilot-profile-settings"></a><span data-ttu-id="97aaa-105">AutoPilot profilinnstillinger</span><span class="sxs-lookup"><span data-stu-id="97aaa-105">AutoPilot profile settings</span></span>

<span data-ttu-id="97aaa-p102">Du kan styre hvordan Windows blir installert på Brukerenheter ved hjelp av AutoPilot-profiler. Profilene inneholder følgende innstillinger.</span><span class="sxs-lookup"><span data-stu-id="97aaa-p102">You can control how Windows gets installed on user devices by using the AutoPilot profiles. The profiles contain the following settings.</span></span>
  
 <span data-ttu-id="97aaa-108">**AutoPilot standard funksjoner (obligatorisk) som er angitt automatisk:**</span><span class="sxs-lookup"><span data-stu-id="97aaa-108">**AutoPilot default features (required) that are set automatically:**</span></span>
  
|<span data-ttu-id="97aaa-109">**Innstilling**</span><span class="sxs-lookup"><span data-stu-id="97aaa-109">**Setting**</span></span>|<span data-ttu-id="97aaa-110">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="97aaa-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="97aaa-111">Hoppe over Cortana, OneDrive og OEM-registrering</span><span class="sxs-lookup"><span data-stu-id="97aaa-111">Skip Cortana, OneDrive and OEM registration</span></span>  <br/> |<span data-ttu-id="97aaa-p103">Hopper over installasjonen av forbruker apps som Cortana og personlige OneDrive. Enhet-brukere kan installere disse senere så lenge han eller hun er en lokal administrator på enheten. Den opprinnelige produsent-registreringen er hoppet over fordi enheten blir administrert av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="97aaa-p103">Skips the installation of consumer apps like Cortana and personal OneDrive. The device user can install these later as long as he or she is a local admin on the device. The original manufacturer registration is skipped because the device will be managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="97aaa-115">Logg på erfaring med produsenten selskap</span><span class="sxs-lookup"><span data-stu-id="97aaa-115">Sign in experience with your company brand</span></span>  <br/> |<span data-ttu-id="97aaa-116">Hvis firmaet har en [legge til firmaets merking i Office 365 påloggingssiden](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), får brukeren enheten problem når du logger på.</span><span class="sxs-lookup"><span data-stu-id="97aaa-116">If your company has a [Add your company branding to Office 365 Sign In page](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), the device user will get that experience when signing in.</span></span>  <br/> |
|<span data-ttu-id="97aaa-117">MDM automatisk registrering med konfigurerte AAD kontoer.</span><span class="sxs-lookup"><span data-stu-id="97aaa-117">MDM auto-enrollment with configured AAD accounts.</span></span>  <br/> |<span data-ttu-id="97aaa-118">Brukeridentiteten blir administrert av Azure Active directory, og brukerne vil logge deg på Windows og Office 365 med legitimasjonen Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="97aaa-118">The user identity will be managed by Azure Active directory, and the users will sign into Windows and Office 365 with their Microsoft 365 Business credentials.</span></span>  <br/> |
   
 <span data-ttu-id="97aaa-119">**Valgfrie innstillinger:**</span><span class="sxs-lookup"><span data-stu-id="97aaa-119">**Optional settings:**</span></span>
  
|<span data-ttu-id="97aaa-120">**Innstilling**</span><span class="sxs-lookup"><span data-stu-id="97aaa-120">**Setting**</span></span>|<span data-ttu-id="97aaa-121">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="97aaa-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="97aaa-122">Hoppe over personverninnstillingene (deaktivert som standard)</span><span class="sxs-lookup"><span data-stu-id="97aaa-122">Skip privacy settings (Off by default)</span></span>  <br/> |<span data-ttu-id="97aaa-123">Hvis dette alternativet er satt til **på**, vil enheten brukeren ikke se lisensavtalen for enheten og Windows når han eller hun først logger på.</span><span class="sxs-lookup"><span data-stu-id="97aaa-123">If this option is set to **On**, the device user will not see the license agreement for the device and Windows when he or she first signs in.</span></span>  <br/> |
|<span data-ttu-id="97aaa-124">Ikke Tillat brukeren å bli den lokale administratoren</span><span class="sxs-lookup"><span data-stu-id="97aaa-124">Don't allow the user to become the local admin</span></span>  <br/> |<span data-ttu-id="97aaa-125">Hvis dette alternativet er satt til **på**, er ikke enheten brukeren kan installere eventuelle personlige programmer, for eksempel Cortana.</span><span class="sxs-lookup"><span data-stu-id="97aaa-125">If this option is set to **On**, the device user will not be able to install any personal apps, such as Cortana.</span></span>  <br/> |
   
