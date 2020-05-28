---
title: Opprette og redigere AutoPilot-profiler
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
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Lær hvordan du oppretter en AutoPilot-profil og bruker den på en enhet, i tillegg til å redigere eller slette en profil eller fjerne en profil fra en enhet.
ms.openlocfilehash: e58418813ed0b4d23a5fa7e1d23aae33d8850e7f
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400978"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="41347-103">Opprette og redigere AutoPilot-profiler</span><span class="sxs-lookup"><span data-stu-id="41347-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="41347-104">Opprette en profil</span><span class="sxs-lookup"><span data-stu-id="41347-104">Create a profile</span></span>

<span data-ttu-id="41347-105">En profil gjelder for en enhet eller en gruppe enheter.</span><span class="sxs-lookup"><span data-stu-id="41347-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="41347-106">Velg **Enheter** \> **AutoPilot**i administrasjonssenteret for Microsoft 365 .</span><span class="sxs-lookup"><span data-stu-id="41347-106">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="41347-107">Velg **profiler-fanen** Opprett profil på **AutoPilot-siden.** \> **Create profile**</span><span class="sxs-lookup"><span data-stu-id="41347-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="41347-108">Skriv inn et navn på profilen som hjelper deg med å identifisere den, for eksempel Markedsføring, på **Opprett profil-siden.**</span><span class="sxs-lookup"><span data-stu-id="41347-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing.</span></span> <span data-ttu-id="41347-109">Slå på innstillingen du vil bruke, og velg deretter **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="41347-109">Turn on the setting you want, and then choose **Save**.</span></span> <span data-ttu-id="41347-110">Hvis du vil ha mer informasjon om AutoPilot-profilinnstillinger, kan du se [Om innstillinger for AutoPilot-profil](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="41347-110">For more information about AutoPilot profile settings, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="41347-112">Knytte profilen til en enhet</span><span class="sxs-lookup"><span data-stu-id="41347-112">Apply profile to a device</span></span>

<span data-ttu-id="41347-113">Når du har opprettet en profil, kan du bruke den på en enhet eller en gruppe enheter.</span><span class="sxs-lookup"><span data-stu-id="41347-113">After you create a profile, you can apply it to a device or a group of devices.</span></span> <span data-ttu-id="41347-114">Du kan velge en eksisterende profil i den [trinnvise veiledningen](add-autopilot-devices-and-profile.md) og bruke den på nye enheter, eller erstatte en eksisterende profil for en enhet eller gruppe enheter.</span><span class="sxs-lookup"><span data-stu-id="41347-114">You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md) and apply it to new devices, or replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="41347-115">Velg **Enheter**-fanen på siden **Klargjøre Windows**.</span><span class="sxs-lookup"><span data-stu-id="41347-115">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="41347-116">Merk av for et enhetsnavn, og velg en profil fra rullegardinlisten **Tilordnet profil** i **Enhet-panelet.** \> **Save**</span><span class="sxs-lookup"><span data-stu-id="41347-116">Select the check box next to a device name, and in the **Device** panel, choose a profile from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="41347-118">Redigere, slette eller fjerne en profil</span><span class="sxs-lookup"><span data-stu-id="41347-118">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="41347-p103">Når du har tilordnet en profil til en enhet, kan du oppdatere den, selv om du allerede har gitt enheten til en bruker. Når enheten er koblet til Internett, laster den ned den siste versjonen av profilen din under installasjonsprosessen. Hvis brukeren gjenoppretter enheten til fabrikkinnstillinger, vil enheten på nytt laste ned de siste oppdateringene til profilen din.</span><span class="sxs-lookup"><span data-stu-id="41347-p103">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="41347-122">Redigere en profil</span><span class="sxs-lookup"><span data-stu-id="41347-122">Edit a profile</span></span>

1. <span data-ttu-id="41347-123">Velg **Profiler**-fanen på siden **Klargjøre Windows**.</span><span class="sxs-lookup"><span data-stu-id="41347-123">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="41347-124">Merk av i avmerkingsboksen ved siden av et enhetsnavn, og oppdater alle tilgjengelige innstillinger Lagre i **Profil-panelet.** \> **Save**</span><span class="sxs-lookup"><span data-stu-id="41347-124">Select the check box next to a device name, and in the **Profile** panel, update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="41347-125">Hvis du gjør dette før en bruker kobler enheten til Internett, blir profilen brukt i installasjonsprosessen.</span><span class="sxs-lookup"><span data-stu-id="41347-125">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="41347-126">Slette en profil</span><span class="sxs-lookup"><span data-stu-id="41347-126">Delete a profile</span></span>

1. <span data-ttu-id="41347-127">Velg **Profiler**-fanen på siden **Klargjøre Windows**.</span><span class="sxs-lookup"><span data-stu-id="41347-127">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="41347-128">Merk av for et enhetsnavn, og velg **Slett profillagre** i **Profil-panelet.** \> **Save**</span><span class="sxs-lookup"><span data-stu-id="41347-128">Select the check box next to a device name, and in the **Profile** panel, select **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="41347-129">Når du sletter en profil, blir den fjernet fra en enhet eller en gruppe enheter som den har blitt tilordnet.</span><span class="sxs-lookup"><span data-stu-id="41347-129">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="41347-130">Fjerne en profil</span><span class="sxs-lookup"><span data-stu-id="41347-130">Remove a profile</span></span>

1. <span data-ttu-id="41347-131">Velg **Enheter**-fanen på siden **Klargjøre Windows**.</span><span class="sxs-lookup"><span data-stu-id="41347-131">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="41347-132">Merk av for et enhetsnavn, og velg **Ingen** fra rullegardinlisten **Tilordnet profil** i **Enhet-panelet.** \> **Save**</span><span class="sxs-lookup"><span data-stu-id="41347-132">Select the check box next to a device name, and in the **Device** panel, choose **None** from the **Assigned profile** drop-down list \> **Save**.</span></span>
    
