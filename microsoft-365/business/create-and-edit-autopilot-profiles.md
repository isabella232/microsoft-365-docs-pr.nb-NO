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
# <a name="create-and-edit-autopilot-profiles"></a>Opprette og redigere AutoPilot-profiler

## <a name="create-a-profile"></a>Opprette en profil

En profil gjelder for en enhet eller en gruppe enheter.
  
1. Velg **Enheter** \> **AutoPilot**i administrasjonssenteret for Microsoft 365 .
  
2. Velg **profiler-fanen** Opprett profil på **AutoPilot-siden.** \> **Create profile**
    
3. Skriv inn et navn på profilen som hjelper deg med å identifisere den, for eksempel Markedsføring, på **Opprett profil-siden.** Slå på innstillingen du vil bruke, og velg deretter **Lagre**. Hvis du vil ha mer informasjon om AutoPilot-profilinnstillinger, kan du se [Om innstillinger for AutoPilot-profil](autopilot-profile-settings.md).
    
    ![Enter name and turn on settings in the Create profile panel.](../media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Knytte profilen til en enhet

Når du har opprettet en profil, kan du bruke den på en enhet eller en gruppe enheter. Du kan velge en eksisterende profil i den [trinnvise veiledningen](add-autopilot-devices-and-profile.md) og bruke den på nye enheter, eller erstatte en eksisterende profil for en enhet eller gruppe enheter. 
  
1. Velg **Enheter**-fanen på siden **Klargjøre Windows**. 
    
2. Merk av for et enhetsnavn, og velg en profil fra rullegardinlisten **Tilordnet profil** i **Enhet-panelet.** \> **Save**
    
    ![In the Device panel, select an Assigned profile to apply it.](../media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Redigere, slette eller fjerne en profil

Når du har tilordnet en profil til en enhet, kan du oppdatere den, selv om du allerede har gitt enheten til en bruker. Når enheten er koblet til Internett, laster den ned den siste versjonen av profilen din under installasjonsprosessen. Hvis brukeren gjenoppretter enheten til fabrikkinnstillinger, vil enheten på nytt laste ned de siste oppdateringene til profilen din. 
  
### <a name="edit-a-profile"></a>Redigere en profil

1. Velg **Profiler**-fanen på siden **Klargjøre Windows**. 
    
2. Merk av i avmerkingsboksen ved siden av et enhetsnavn, og oppdater alle tilgjengelige innstillinger Lagre i **Profil-panelet.** \> **Save**
    
    Hvis du gjør dette før en bruker kobler enheten til Internett, blir profilen brukt i installasjonsprosessen.
    
### <a name="delete-a-profile"></a>Slette en profil

1. Velg **Profiler**-fanen på siden **Klargjøre Windows**. 
    
2. Merk av for et enhetsnavn, og velg **Slett profillagre** i **Profil-panelet.** \> **Save**
    
    Når du sletter en profil, blir den fjernet fra en enhet eller en gruppe enheter som den har blitt tilordnet.
    
### <a name="remove-a-profile"></a>Fjerne en profil

1. Velg **Enheter**-fanen på siden **Klargjøre Windows**. 
    
2. Merk av for et enhetsnavn, og velg **Ingen** fra rullegardinlisten **Tilordnet profil** i **Enhet-panelet.** \> **Save**
    
