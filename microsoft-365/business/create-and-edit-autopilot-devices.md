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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Lær hvordan du laster opp enheter ved hjelp av AutoPilot i Microsoft 365 Business. Du kan tilordne en profil til en enhet eller en gruppe enheter.
ms.openlocfilehash: 9ae94266f5a41d8d115fc92f0f080a6fdbdc9f15
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288019"
---
# <a name="create-and-edit-autopilot-devices"></a>Opprette og redigere AutoPilot-enheter

## <a name="upload-a-list-of-devices"></a>Laste opp en liste over enheter

Du kan bruke den [Trinnvise veiledningen](add-autopilot-devices-and-profile.md) til å laste opp enheter, men du kan også laste opp på **Enheter**-fanen. 
  
Enheter må oppfylle disse kravene:
  
- Windows 10 versjon 1703 eller senere.
    
- Nye enheter som ikke har vært gjennom Windows out-of-box experience.

1. Velg **enheter** \> **autopilot**i Microsoft 365 bedrifts Administrasjonssenter.
  
2. På siden **autopilot** velger du \> kategorien **enheter** og **legger til enheter**.
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. På **Legg til enheter** -panelet blar du til [en enhet-liste CSV-fil](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) som du \> har klargjort **Lagre** \> **lukking**.
    
    Du får denne informasjonen fra leverandøren av maskinvaren, eller du kan bruke [Get-WindowsAutoPilotInfo PowerShell-skriptet](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), som genererer en CSV-fil. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Legge til en profil gjelder for en enhet eller en gruppe enheter

1. På **Klargjøre Windows**-siden velger du **Enheter**-fanen og merker av for én eller flere enheter. 
    
2. Velg en profil fra rullegardinlisten **Tilordnet profil** på panelet **Enhet**. 
    
    Se [Opprette og redigere AutoPilot-profiler](create-and-edit-autopilot-profiles.md) for instruksjoner hvis du ikke har noen profiler ennå. 
    
