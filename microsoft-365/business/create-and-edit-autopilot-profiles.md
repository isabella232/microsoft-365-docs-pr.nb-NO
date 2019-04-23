---
title: Opprette og redigere AutoPilot-profiler
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Lær hvordan du kan opprette, redigere, slette eller fjerne AutoPilot-profiler. '
ms.openlocfilehash: 85fc897b2f428afae8d55feeb577021adaa30f72
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277148"
---
# <a name="create-and-edit-autopilot-profiles"></a>Opprette og redigere AutoPilot-profiler

## <a name="create-a-profile"></a>Opprette en profil

En profil gjelder for en enhet eller en gruppe enheter.
  
1. Velg **enheter** i Microsoft 365 Business administrasjonssenteret, \> **AutoPilot**.
  
2. Velg kategorien **profiler** på **AutoPilot** -siden \> **opprette profil**.
    
3. Skriv inn et profilnavn som hjelper deg å gjenkjenne den på siden **Opprett profil**, for eksempel Markedsføring, aktiver innstillingen du ønsker (se [Om profilinnstillinger for AutoPilot](autopilot-profile-settings.md) for mer informasjon), og trykk deretter på **Lagre**.
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Knytte profilen til en enhet

Når du oppretter en profil, kan du knytte den til en enhet eller en gruppe enheter. Du kan velge en eksisterende profil i [Trinnvise instruksjoner](add-autopilot-devices-and-profile.md), du kan knytte den til nye enheter, eller du kan erstatte en eksisterende profil for en enhet eller en gruppe enheter. 
  
1. Velg **Enheter**-fanen på siden **Klargjøre Windows**. 
    
2. Click the check-box next to a device name and in the **Device** panel, choose a profile from the **Assigned profile** drop-down \> **Save**.
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Redigere, slette eller fjerne en profil

Når du har tilordnet en profil til en enhet, kan du oppdatere den, selv om du allerede har gitt enheten til en bruker. Når enheten er koblet til Internett, laster den ned den siste versjonen av profilen din under installasjonsprosessen. Hvis brukeren gjenoppretter enheten til fabrikkinnstillinger, vil enheten på nytt laste ned de siste oppdateringene til profilen din. 
  
### <a name="edit-a-profile"></a>Redigere en profil

1. Velg **Profiler**-fanen på siden **Klargjøre Windows**. 
    
2. Click the check-box next to a device name and in the **Profile** panel update any of the available settings \> **Save**.
    
    Hvis du gjør dette før en bruker kobler enheten til Internett, blir profilen brukt i installasjonsprosessen.
    
### <a name="delete-a-profile"></a>Slette en profil

1. Velg **Profiler**-fanen på siden **Klargjøre Windows**. 
    
2. Click the check-box next to a device name and in the **Profile** panel click **Delete profile** \> **Save**.
    
    Når du sletter en profil, blir den fjernet fra en enhet eller en gruppe enheter som den har blitt tilordnet.
    
### <a name="remove-a-profile"></a>Fjerne en profil

1. Velg **Enheter**-fanen på siden **Klargjøre Windows**. 
    
2. Click the check-box next to a device name and in the **Device** panel, choose a **None** from the **Assigned profile** drop-down \> **Save**.
    
