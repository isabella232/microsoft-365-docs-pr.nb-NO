---
title: Opprette og redigere AutoPilot-profiler
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
ms.assetid: 5cf7139e-cfa1-4765-8aad-001af1c74faa
description: 'Lær hvordan du kan opprette, redigere, slette eller fjerne AutoPilot-profiler. '
ms.openlocfilehash: 4658a27e5f2c64a52f8a7d08b3fc13df5e239dc3
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983136"
---
# <a name="create-and-edit-autopilot-profiles"></a>Opprette og redigere AutoPilot-profiler

## <a name="create-a-profile"></a>Opprette en profil

En profil gjelder for en enhet eller en gruppe enheter.
  
1. I Microsoft 365 Businessadministrasjonssenteret velger du **Distribuere Windows med AutoPilot** på kortet **Enhetshandlinger**. 
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. Velg kategorien **profiler** på siden **Klargjør Windows** \> **opprette profil**.
    
3. Skriv inn et profilnavn som hjelper deg å gjenkjenne den på siden **Opprett profil**, for eksempel Markedsføring, aktiver innstillingen du ønsker (se [Om profilinnstillinger for AutoPilot](autopilot-profile-settings.md) for mer informasjon), og trykk deretter på **Lagre**.
    
    ![Enter name and turn on settings in the Create profile panel.](media/63b5a00d-6a5d-48d0-9557-e7531e80702a.png)
  
### <a name="apply-profile-to-a-device"></a>Knytte profilen til en enhet

Når du oppretter en profil, kan du knytte den til en enhet eller en gruppe enheter. Du kan velge en eksisterende profil i [Trinnvise instruksjoner](add-autopilot-devices-and-profile.md), du kan knytte den til nye enheter, eller du kan erstatte en eksisterende profil for en enhet eller en gruppe enheter. 
  
1. Velg **Enheter**-fanen på siden **Klargjøre Windows**. 
    
2. Klikk i avmerkingsboksen ved siden av navnet på en enhet og i **enhet** -panelet, velger en profil fra rullegardinlisten **tilordnet profilen** \> **Lagre**.
    
    ![In the Device panel, select an Assigned profile to apply it.](media/ed0ce33f-9241-4403-a5de-2dddffdc6fb9.png)
  
## <a name="edit-delete-or-remove-a-profile"></a>Redigere, slette eller fjerne en profil

Når du har tilordnet en profil til en enhet, kan du oppdatere den, selv om du allerede har gitt enheten til en bruker. Når enheten er koblet til Internett, laster den ned den siste versjonen av profilen din under installasjonsprosessen. Hvis brukeren gjenoppretter enheten til fabrikkinnstillinger, vil enheten på nytt laste ned de siste oppdateringene til profilen din. 
  
### <a name="edit-a-profile"></a>Redigere en profil

1. Velg **Profiler**-fanen på siden **Klargjøre Windows**. 
    
2. Klikk i avmerkingsboksen ved siden av navnet på en enhet, og i **profilen** panelet oppdatere noen av de tilgjengelige innstillingene \> **Lagre**.
    
    Hvis du gjør dette før en bruker kobler enheten til Internett, blir profilen brukt i installasjonsprosessen.
    
### <a name="delete-a-profile"></a>Slette en profil

1. Velg **Profiler**-fanen på siden **Klargjøre Windows**. 
    
2. Klikk i avmerkingsboksen ved siden av navnet på en enhet, og klikk **Slett profil** i **profil** -panelet \> **Lagre**.
    
    Når du sletter en profil, blir den fjernet fra en enhet eller en gruppe enheter som den har blitt tilordnet.
    
### <a name="remove-a-profile"></a>Fjerne en profil

1. Velg **Enheter**-fanen på siden **Klargjøre Windows**. 
    
2. Klikk i avmerkingsboksen ved siden av navnet på en enhet og i **enhet** -panelet, velger du en **Ingen** fra rullegardinlisten **tilordnet profilen** \> **Lagre**.
    
