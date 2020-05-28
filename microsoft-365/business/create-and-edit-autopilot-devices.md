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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Finn ut hvordan du laster opp enheter ved hjelp av AutoPilot i Microsoft 365 Business Premium. Du kan tilordne en profil til en enhet eller en gruppe enheter.
ms.openlocfilehash: 8c3d029d682ae30444bdc7d30a4790a8f982e0e0
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400998"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="f758a-104">Opprette og redigere AutoPilot-enheter</span><span class="sxs-lookup"><span data-stu-id="f758a-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="f758a-105">Laste opp en liste over enheter</span><span class="sxs-lookup"><span data-stu-id="f758a-105">Upload a list of devices</span></span>

<span data-ttu-id="f758a-106">Du kan bruke den [trinnvise veiledningen](add-autopilot-devices-and-profile.md) til å laste opp enheter, men du kan også laste opp enheter i **Enheter-fanen.**</span><span class="sxs-lookup"><span data-stu-id="f758a-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload devices in the **Devices** tab.</span></span> 
  
<span data-ttu-id="f758a-107">Enheter må oppfylle disse kravene:</span><span class="sxs-lookup"><span data-stu-id="f758a-107">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="f758a-108">Windows 10, versjon 1703 eller nyere</span><span class="sxs-lookup"><span data-stu-id="f758a-108">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="f758a-109">Nye enheter som ikke har vært gjennom Windows out-of-box-opplevelse</span><span class="sxs-lookup"><span data-stu-id="f758a-109">New devices that haven't been through Windows out-of-box experience</span></span>

1. <span data-ttu-id="f758a-110">Velg **Enheter** \> **AutoPilot**i administrasjonssenteret for Microsoft 365 .</span><span class="sxs-lookup"><span data-stu-id="f758a-110">In the Microsoft 365 admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="f758a-111">Velg **kategorien Enheter** på **AutoPilot-siden.** \> **Add devices**</span><span class="sxs-lookup"><span data-stu-id="f758a-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="f758a-113">Bla til en [CSV-fil](https://docs.microsoft.com/microsoft-365/admin/misc/device-list) for enhetsliste som du klarreder Lagre lukk , i panelet **Legg til enheter** \> **Save** \> **Close**.</span><span class="sxs-lookup"><span data-stu-id="f758a-113">On the **Add devices** panel, browse to a [Device list CSV file](https://docs.microsoft.com/microsoft-365/admin/misc/device-list) that you prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="f758a-114">Du kan få denne informasjonen fra maskinvareleverandøren, eller du kan bruke [Get-WindowsAutoPilotInfo PowerShell-skriptet](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) til å generere en CSV-fil.</span><span class="sxs-lookup"><span data-stu-id="f758a-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="f758a-115">Legge til en profil gjelder for en enhet eller en gruppe enheter</span><span class="sxs-lookup"><span data-stu-id="f758a-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="f758a-116">Velg **Kategorien Enheter** på **Klargjør** Windows-siden, og merk av for én eller flere enheter.</span><span class="sxs-lookup"><span data-stu-id="f758a-116">On the **Prepare Windows** page, choose the **Devices** tab, and select the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="f758a-117">Velg en profil fra rullegardinlisten **Tilordnet profil** på panelet **Enhet**.</span><span class="sxs-lookup"><span data-stu-id="f758a-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="f758a-118">Se [Opprette og redigere AutoPilot-profiler](create-and-edit-autopilot-profiles.md) for instruksjoner hvis du ikke har noen profiler ennå.</span><span class="sxs-lookup"><span data-stu-id="f758a-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
