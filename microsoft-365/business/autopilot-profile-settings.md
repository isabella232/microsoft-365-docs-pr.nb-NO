---
title: Om innstillinger for AutoPilot-profil
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
f1_keywords:
- ZTDProfileSettings
- O365E_ZTDProfileSettings
- BCS365_ZTDProfileSettings
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
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: AutoPilot profiler hjelper deg med å styre hvordan Windows blir installert på Brukerenheter. Profilene inneholder standard og valgfrie innstillinger som hopper Cortana installasjon.
ms.openlocfilehash: d43a15e5f3dc83596b5c23dd0ceb416b24810298
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32276945"
---
# <a name="about-autopilot-profile-settings"></a>Om innstillinger for AutoPilot-profil

## <a name="autopilot-profile-settings"></a>AutoPilot profilinnstillinger

Du kan styre hvordan Windows blir installert på Brukerenheter ved hjelp av AutoPilot-profiler. Profilene inneholder følgende innstillinger.
  
 **AutoPilot standard funksjoner (obligatorisk) som er angitt automatisk:**
  
|**Innstilling**|**Beskrivelse**|
|:-----|:-----|
|Hoppe over Cortana, OneDrive og OEM-registrering  <br/> |Hopper over installasjonen av forbruker apps som Cortana og personlige OneDrive. Enhet-brukere kan installere disse senere så lenge han eller hun er en lokal administrator på enheten. Den opprinnelige produsent-registreringen er hoppet over fordi enheten blir administrert av Microsoft 365 Business.  <br/> |
|Logg på erfaring med produsenten selskap  <br/> |Hvis firmaet har en [legge til firmaets merking i Office 365 påloggingssiden](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), får brukeren enheten problem når du logger på.  <br/> |
|MDM automatisk registrering med konfigurerte AAD kontoer.  <br/> |Brukeridentiteten blir administrert av Azure Active directory, og brukerne vil logge deg på Windows og Office 365 med legitimasjonen Microsoft 365 Business.  <br/> |
   
 **Valgfrie innstillinger:**
  
|**Innstilling**|**Beskrivelse**|
|:-----|:-----|
|Hoppe over personverninnstillingene (deaktivert som standard)  <br/> |Hvis dette alternativet er satt til **på**, vil enheten brukeren ikke se lisensavtalen for enheten og Windows når han eller hun først logger på.  <br/> |
|Ikke Tillat brukeren å bli den lokale administratoren  <br/> |Hvis dette alternativet er satt til **på**, er ikke enheten brukeren kan installere eventuelle personlige programmer, for eksempel Cortana.  <br/> |
   
