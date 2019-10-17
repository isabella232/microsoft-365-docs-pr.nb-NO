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
# <a name="create-and-edit-autopilot-profiles"></a>Opprette og redigere AutoPilot-profiler

## <a name="create-a-profile"></a>Opprette en profil

En profil gjelder for en enhet eller en gruppe enheter.
  
1. Velg **enheter** \> **autopilot**i Microsoft 365 bedrifts Administrasjonssenter.
  
2. På siden **autopilot** velger du \> kategorien **profiler** **Opprett profil**.
    
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
    
