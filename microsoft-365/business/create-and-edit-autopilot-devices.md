---
title: Opprette og redigere AutoPilot-enheter
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Finn ut hvordan du laster opp enheter ved hjelp av AutoPilot i Microsoft 365 Business. Du kan tilordne en profil til en enhet eller en gruppe enheter.
ms.openlocfilehash: 640e4af7cccde83c87d90a875c1d44dead7255ca
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/15/2020
ms.locfileid: "42065990"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="43c0b-104">Opprette og redigere AutoPilot-enheter</span><span class="sxs-lookup"><span data-stu-id="43c0b-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="43c0b-105">Laste opp en liste over enheter</span><span class="sxs-lookup"><span data-stu-id="43c0b-105">Upload a list of devices</span></span>

<span data-ttu-id="43c0b-106">Du kan bruke trinnvis veiledning til å laste opp enheter, men du kan også laste opp enheter i [Enheter-fanen.](add-autopilot-devices-and-profile.md) \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="43c0b-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="43c0b-107">Enheter må oppfylle disse kravene:</span><span class="sxs-lookup"><span data-stu-id="43c0b-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="43c0b-108">Windows 10, versjon 1703 eller nyere</span><span class="sxs-lookup"><span data-stu-id="43c0b-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="43c0b-109">Nye enheter som ikke har vært gjennom Windows-opplevelsen</span><span class="sxs-lookup"><span data-stu-id="43c0b-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="43c0b-110">Velg **Enheter** \> **AutoPilot**i administrasjonssenteret for Microsoft 365 Business .</span><span class="sxs-lookup"><span data-stu-id="43c0b-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="43c0b-111">Velg kategorien **Enheter** \> **på** **AutoPilot-siden.**</span><span class="sxs-lookup"><span data-stu-id="43c0b-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="43c0b-113">Bla til en [CSV-fil](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) for enhetsliste som \> du forberedte **Lagre** \> **Lukk**i panelet Legg **til enheter** .</span><span class="sxs-lookup"><span data-stu-id="43c0b-113">On the **Add devices** panel, browse to a [Device list CSV file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="43c0b-114">Du kan få denne informasjonen fra maskinvareleverandøren, eller du kan bruke [Get-WindowsAutoPilotInfo PowerShell-skriptet](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) til å generere en CSV-fil.</span><span class="sxs-lookup"><span data-stu-id="43c0b-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="43c0b-115">Legge til en profil gjelder for en enhet eller en gruppe enheter</span><span class="sxs-lookup"><span data-stu-id="43c0b-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="43c0b-116">Velg kategorien **Enheter** på **Klargjør** Windows-siden, og merk av for én eller flere enheter.</span><span class="sxs-lookup"><span data-stu-id="43c0b-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="43c0b-117">Velg en profil fra rullegardinlisten **Tilordnet profil** på panelet **Enhet**.</span><span class="sxs-lookup"><span data-stu-id="43c0b-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="43c0b-118">Se [Opprette og redigere AutoPilot-profiler](create-and-edit-autopilot-profiles.md) for instruksjoner hvis du ikke har noen profiler ennå.</span><span class="sxs-lookup"><span data-stu-id="43c0b-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
