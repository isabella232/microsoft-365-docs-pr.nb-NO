---
title: Opprette og redigere AutoPilot-profiler
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: Lær hvordan du oppretter, redigerer, sletter eller fjerner AutoPilot-profiler.
ms.openlocfilehash: 4305340a2fc5df8202cf4d85f9e2541690bf9ed0
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/17/2019
ms.locfileid: "37574722"
---
# <a name="create-and-edit-autopilot-profiles"></a><span data-ttu-id="c5cdc-103">Opprette og redigere AutoPilot-profiler</span><span class="sxs-lookup"><span data-stu-id="c5cdc-103">Create and edit AutoPilot profiles</span></span>

## <a name="create-a-profile"></a><span data-ttu-id="c5cdc-104">Opprette en profil</span><span class="sxs-lookup"><span data-stu-id="c5cdc-104">Create a profile</span></span>

<span data-ttu-id="c5cdc-105">En profil gjelder for en enhet eller en gruppe enheter.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-105">A profile applies to a device, or a group of devices,</span></span>
  
1. <span data-ttu-id="c5cdc-106">Velg **enheter** \> **autopilot**i Microsoft 365 bedrifts Administrasjonssenter.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-106">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="c5cdc-107">På siden **autopilot** velger du \> kategorien **profiler** **Opprett profil**.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-107">On the **AutoPilot** page, choose the **Profiles** tab \> **Create profile**.</span></span>
    
3. <span data-ttu-id="c5cdc-108">Skriv inn et profilnavn som hjelper deg å gjenkjenne den på siden **Opprett profil**, for eksempel Markedsføring, aktiver innstillingen du ønsker (se [Om profilinnstillinger for AutoPilot](autopilot-profile-settings.md) for mer informasjon), og trykk deretter på **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-108">On the **Create profile** page, enter a name for the profile that helps you identify it, for example Marketing, turn on the setting you want (see [About AutoPilot Profile settings](autopilot-profile-settings.md) for more information), and choose **Save**.</span></span>
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a><span data-ttu-id="c5cdc-110">Knytte profilen til en enhet</span><span class="sxs-lookup"><span data-stu-id="c5cdc-110">Apply profile to a device</span></span>

<span data-ttu-id="c5cdc-p101">Når du oppretter en profil, kan du knytte den til en enhet eller en gruppe enheter. Du kan velge en eksisterende profil i [Trinnvise instruksjoner](add-autopilot-devices-and-profile.md), du kan knytte den til nye enheter, eller du kan erstatte en eksisterende profil for en enhet eller en gruppe enheter.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-p101">After you create a profile you can apply it to a device or a group of devices. You can pick an existing profile in the [step-by-step guide](add-autopilot-devices-and-profile.md), you can apply it to new devices, or you can replace an existing profile for a device or group of devices.</span></span> 
  
1. <span data-ttu-id="c5cdc-113">Velg **Enheter**-fanen på siden **Klargjøre Windows**.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-113">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="c5cdc-114">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-114">Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.</span></span>
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a><span data-ttu-id="c5cdc-116">Redigere, slette eller fjerne en profil</span><span class="sxs-lookup"><span data-stu-id="c5cdc-116">Edit, delete, or remove a profile</span></span>

<span data-ttu-id="c5cdc-p102">Når du har tilordnet en profil til en enhet, kan du oppdatere den, selv om du allerede har gitt enheten til en bruker. Når enheten er koblet til Internett, laster den ned den siste versjonen av profilen din under installasjonsprosessen. Hvis brukeren gjenoppretter enheten til fabrikkinnstillinger, vil enheten på nytt laste ned de siste oppdateringene til profilen din.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-p102">Once you've assigned a profile to a device, you can update it, even if you've already given the device to a user. When the device connects to the internet, it downloads the latest version of your profile during the setup process. If the user restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 
  
### <a name="edit-a-profile"></a><span data-ttu-id="c5cdc-120">Redigere en profil</span><span class="sxs-lookup"><span data-stu-id="c5cdc-120">Edit a profile</span></span>

1. <span data-ttu-id="c5cdc-121">Velg **Profiler**-fanen på siden **Klargjøre Windows**.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-121">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="c5cdc-122">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-122">Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.</span></span>
    
    <span data-ttu-id="c5cdc-123">Hvis du gjør dette før en bruker kobler enheten til Internett, blir profilen brukt i installasjonsprosessen.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-123">If you do this before a user connects the device to the internet, then the profile gets applied to the setup process.</span></span>
    
### <a name="delete-a-profile"></a><span data-ttu-id="c5cdc-124">Slette en profil</span><span class="sxs-lookup"><span data-stu-id="c5cdc-124">Delete a profile</span></span>

1. <span data-ttu-id="c5cdc-125">Velg **Profiler**-fanen på siden **Klargjøre Windows**.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-125">On the **Prepare Windows** page, choose the **Profiles** tab.</span></span> 
    
2. <span data-ttu-id="c5cdc-126">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-126">Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.</span></span>
    
    <span data-ttu-id="c5cdc-127">Når du sletter en profil, blir den fjernet fra en enhet eller en gruppe enheter som den har blitt tilordnet.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-127">When you delete a profile, it gets removed from a device or a group of devices it was assigned to.</span></span>
    
### <a name="remove-a-profile"></a><span data-ttu-id="c5cdc-128">Fjerne en profil</span><span class="sxs-lookup"><span data-stu-id="c5cdc-128">Remove a profile</span></span>

1. <span data-ttu-id="c5cdc-129">Velg **Enheter**-fanen på siden **Klargjøre Windows**.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-129">On the **Prepare Windows** page, choose the **Devices** tab.</span></span> 
    
2. <span data-ttu-id="c5cdc-130">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span><span class="sxs-lookup"><span data-stu-id="c5cdc-130">Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.</span></span>
    
