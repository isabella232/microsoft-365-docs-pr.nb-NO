---
title: Opprette og redigere AutoPilot-enheter
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
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
ms.assetid: 0f7b1d7c-4086-4331-8534-45d7886f9f34
description: Lær hvordan du laster opp enheter ved hjelp av AutoPilot i Microsoft 365 Business. Du kan tilordne en profil til en enhet eller en gruppe av enheter.
ms.openlocfilehash: cc1f81e9efd9b16e27b8abfbb0927d241535077e
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982936"
---
# <a name="create-and-edit-autopilot-devices"></a>Opprette og redigere AutoPilot-enheter

## <a name="upload-a-list-of-devices"></a>Laste opp en liste over enheter

Du kan bruke den [Trinnvise veiledningen](add-autopilot-devices-and-profile.md) til å laste opp enheter, men du kan også laste opp på **Enheter**-fanen. 
  
Enheter må oppfylle disse kravene:
  
- Windows 10 versjon 1703 eller senere.
    
- Nye enheter som ikke har vært gjennom Windows out-of-box experience.
    
1. I administrasjonssenteret for Microsoft 365 Business velger du **Distribuere Windows med AutoPilot** på **Enhetshandlinger**-kortet. 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. Velg kategorien **enheter** på siden **Klargjør Windows** \> **Legg til enheter**.
    
    ![In the Devices tab, choose Add devices.](media/6ba81e22-c873-40ad-8a72-ce64d15ea6ba.png)
  
3. Bla deg frem til en [liste over enheter CSV-fil](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) som du har forberedt på **Legg til enheter** -panelet \> **Lagre** \> **Lukk**.
    
    Du får denne informasjonen fra leverandøren av maskinvaren, eller du kan bruke [Get-WindowsAutoPilotInfo PowerShell-skriptet](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), som genererer en CSV-fil. 
    
## <a name="assign-a-profile-to-a-device-or-a-group-of-devices"></a>Legge til en profil gjelder for en enhet eller en gruppe enheter

1. På **Klargjøre Windows**-siden velger du **Enheter**-fanen og merker av for én eller flere enheter. 
    
2. Velg en profil fra rullegardinlisten **Tilordnet profil** på panelet **Enhet**. 
    
    Se [Opprette og redigere AutoPilot-profiler](create-and-edit-autopilot-profiles.md) for instruksjoner hvis du ikke har noen profiler ennå. 
    
