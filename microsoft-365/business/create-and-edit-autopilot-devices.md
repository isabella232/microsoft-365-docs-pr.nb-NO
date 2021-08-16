---
title: Opprette og redigere AutoPilot-enheter
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Lær hvordan du laster opp enheter ved hjelp av AutoPilot i Microsoft 365 Business Premium. Du kan tilordne en profil til en enhet eller en gruppe enheter.
ms.openlocfilehash: ae3a760db4b94aac50301685a0c4f468e46ec8e9aa907a1b6fb35e03a9e541f0
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53867035"
---
# <a name="create-and-edit-autopilot-devices"></a>Opprette og redigere AutoPilot-enheter

## <a name="upload-a-list-of-devices"></a>Laste opp en liste over enheter

Du kan bruke trinnvis veiledning til å laste opp enheter, men du kan også laste opp enheter på [Enheter-fanen.](add-autopilot-devices-and-profile.md)  
  
Enheter må oppfylle disse kravene:
  
- Windows 10, versjon 1703 eller nyere
    
- Nye enheter som ikke har vært gjennom Windows en ut-av-boks-opplevelse

1. I Administrasjonssenter for Microsoft 365 velger du **Enheter** \> **AutoPilot**.
  
2. Velg **Enheter-fanen** Legg til enheter på **AutoPilot-siden.** \> 
    
    ![In the Devices tab, choose Add devices.](../media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Bla til **en CSV-fil** med enhetsliste som du forberedte Lagre lukk på panelet Legg [](../admin/misc/device-list.md) \> **til** \> **enheter.**
    
    Du kan få denne informasjonen fra maskinvareleverandøren, eller du kan bruke [Get-WindowsAutoPilotInfo PowerShell-skriptet](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) til å generere en CSV-fil. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Legge til en profil gjelder for en enhet eller en gruppe enheter

1. Velg **Enheter-fanen på** klargjøringssiden Windows, og merk av for én eller flere enheter.  
    
2. Velg en profil fra rullegardinlisten **Tilordnet profil** på panelet **Enhet**. 
    
    Se [Opprette og redigere AutoPilot-profiler](create-and-edit-autopilot-profiles.md) for instruksjoner hvis du ikke har noen profiler ennå. 
