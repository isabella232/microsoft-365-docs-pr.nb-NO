---
title: Opprette og redigere AutoPilot-enheter
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Lær hvordan du laster opp enheter ved hjelp av AutoPilot i Microsoft 365 Business. Du kan tilordne en profil til en enhet eller en gruppe av enheter.
ms.openlocfilehash: dee77a014ef519f3487a082edc3cf81058ec1c00
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/15/2019
ms.locfileid: "34071644"
---
# <a name="create-and-edit-autopilot-devices"></a><span data-ttu-id="145e9-104">Opprette og redigere AutoPilot-enheter</span><span class="sxs-lookup"><span data-stu-id="145e9-104">Create and edit AutoPilot devices</span></span>

## <a name="upload-a-list-of-devices"></a><span data-ttu-id="145e9-105">Laste opp en liste over enheter</span><span class="sxs-lookup"><span data-stu-id="145e9-105">Upload a list of devices</span></span>

<span data-ttu-id="145e9-106">Du kan bruke den [Trinnvise veiledningen](add-autopilot-devices-and-profile.md) til å laste opp enheter, men du kan også laste opp på **Enheter**-fanen.</span><span class="sxs-lookup"><span data-stu-id="145e9-106">You can use the [Step-by-step guide](add-autopilot-devices-and-profile.md) to upload devices, but you can also upload the in the **Devices** tab.</span></span> 
  
<span data-ttu-id="145e9-107">Enheter må oppfylle disse kravene:</span><span class="sxs-lookup"><span data-stu-id="145e9-107">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="145e9-108">Windows 10 versjon 1703 eller senere.</span><span class="sxs-lookup"><span data-stu-id="145e9-108">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="145e9-109">Nye enheter som ikke har vært gjennom Windows out-of-box experience.</span><span class="sxs-lookup"><span data-stu-id="145e9-109">New devices that have not been through Windows out-of-box experience.</span></span>

1. <span data-ttu-id="145e9-110">Velg **enheter** i Microsoft 365 Business administrasjonssenteret, \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="145e9-110">In the Microsoft 365 Business Admin center, choose **Devices** \> **AutoPilot**.</span></span>
  
2. <span data-ttu-id="145e9-111">Velg kategorien **enheter** på **AutoPilot** -siden \> **Legg til enheter**.</span><span class="sxs-lookup"><span data-stu-id="145e9-111">On the **AutoPilot** page, choose the **Devices** tab \> **Add devices**.</span></span>
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. <span data-ttu-id="145e9-113">Bla deg frem til en [liste over enheter CSV-fil](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) som du har forberedt på **Legg til enheter** -panelet \> **Lagre** \> **Lukk**.</span><span class="sxs-lookup"><span data-stu-id="145e9-113">On the **Add devices** panel, browse to a [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) that you have prepared \> **Save** \> **Close**.</span></span>
    
    <span data-ttu-id="145e9-114">Du får denne informasjonen fra leverandøren av maskinvaren, eller du kan bruke [Get-WindowsAutoPilotInfo PowerShell-skriptet](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), som genererer en CSV-fil.</span><span class="sxs-lookup"><span data-stu-id="145e9-114">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a csv file.</span></span> 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a><span data-ttu-id="145e9-115">Legge til en profil gjelder for en enhet eller en gruppe enheter</span><span class="sxs-lookup"><span data-stu-id="145e9-115">Assign a profile to a device or a group of devices</span></span>

1. <span data-ttu-id="145e9-116">På **Klargjøre Windows**-siden velger du **Enheter**-fanen og merker av for én eller flere enheter.</span><span class="sxs-lookup"><span data-stu-id="145e9-116">On the **Prepare Windows** page, choose the **Devices** tab and check the check box next to one or more devices.</span></span> 
    
2. <span data-ttu-id="145e9-117">Velg en profil fra rullegardinlisten **Tilordnet profil** på panelet **Enhet**.</span><span class="sxs-lookup"><span data-stu-id="145e9-117">On the **Device** panel, select a profile from the **Assigned profile** drop-down.</span></span> 
    
    <span data-ttu-id="145e9-118">Se [Opprette og redigere AutoPilot-profiler](create-and-edit-autopilot-profiles.md) for instruksjoner hvis du ikke har noen profiler ennå.</span><span class="sxs-lookup"><span data-stu-id="145e9-118">If you don't have any profiles yet, see [Create and edit AutoPilot profiles](create-and-edit-autopilot-profiles.md) for instructions.</span></span> 
    
