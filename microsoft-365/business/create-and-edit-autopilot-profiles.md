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
ms.openlocfilehash: f7fdc2632e93c48e043fe158842f8395d6a89e14
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/14/2019
ms.locfileid: "38320242"
---
# <a name="create-and-edit-autopilot-profiles"></a>Opprette og redigere AutoPilot-profiler

## <a name="create-a-profile"></a>Opprette en profil

En profil gjelder for en enhet eller en gruppe enheter.
  
1. Velg **enheter** \> **autopilot**i Microsoft 365 bedrifts Administrasjonssenter.
  
2. På siden **autopilot** velger du \> kategorien **profiler** **Opprett profil**.
    
3. På **Opprett profil** -siden skriver du inn et navn for profilen som hjelper deg med å identifisere den, for eksempel markedsføring. Aktiver innstillingen du vil bruke, og velg deretter **Lagre**. Hvis du vil ha mer informasjon om innstillinger for AutoPilot-profilen, kan du se [om Profilinnstillinger for autopilot](autopilot-profile-settings.md).
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Knytte profilen til en enhet

Når du har opprettet en profil, kan du bruke den på en enhet eller en gruppe med enheter. Du kan velge en eksisterende profil i den [trinnvise veiledningen](add-autopilot-devices-and-profile.md) og bruke den på nye enheter, eller erstatte en eksisterende profil for en enhet eller gruppe med enheter. 
  
1. Velg **Enheter**-fanen på siden **Klargjøre Windows**. 
    
2. Merk av i avmerkingsboksen ved siden av et enhetsnavn, og velg en profil fra rulle \> **gardin listen** **tilordnet profil** i **enhets** panelet.
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Redigere, slette eller fjerne en profil

Når du har tilordnet en profil til en enhet, kan du oppdatere den, selv om du allerede har gitt enheten til en bruker. Når enheten er koblet til Internett, laster den ned den siste versjonen av profilen din under installasjonsprosessen. Hvis brukeren gjenoppretter enheten til fabrikkinnstillinger, vil enheten på nytt laste ned de siste oppdateringene til profilen din. 
  
### <a name="edit-a-profile"></a>Redigere en profil

1. Velg **Profiler**-fanen på siden **Klargjøre Windows**. 
    
2. Merk av i avmerkingsboksen ved siden av et enhetsnavn, og Oppdater alle \> **tilgjengelige innstillinger i** **profil** panelet.
    
    Hvis du gjør dette før en bruker kobler enheten til Internett, blir profilen brukt i installasjonsprosessen.
    
### <a name="delete-a-profile"></a>Slette en profil

1. Velg **Profiler**-fanen på siden **Klargjøre Windows**. 
    
2. Merk av i avmerkingsboksen ved siden av et enhetsnavn, og velg deretter **Slett profil** \> **lagring**i **profil** panelet.
    
    Når du sletter en profil, blir den fjernet fra en enhet eller en gruppe enheter som den har blitt tilordnet.
    
### <a name="remove-a-profile"></a>Fjerne en profil

1. Velg **Enheter**-fanen på siden **Klargjøre Windows**. 
    
2. Merk av i avmerkingsboksen ved siden av et enhetsnavn, og velg **ingen** fra rulle \> **gardin listen for**den **tilordnede profilen** i **enhets** panelet.
    
