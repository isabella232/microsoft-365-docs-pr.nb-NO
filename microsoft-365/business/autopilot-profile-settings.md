---
title: Om innstillinger for AutoPilot-profil
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 99bfbf81-e719-4630-9b0f-c187edfa1f8a
description: AutoPilot-profiler hjelper deg med å kontrollere hvordan Windows blir installert på brukerenheter. Profilene inneholder standard- og valgfrie innstillinger som hopp over Cortana-installasjonen.
ms.openlocfilehash: 1cc8a3171bbc4a1e5cb531b9364c7791586fc339
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593337"
---
# <a name="about-autopilot-profile-settings"></a>Om innstillinger for AutoPilot-profil

## <a name="autopilot-profile-settings"></a>Innstillinger for AutoPilot-profil

Du kan bruke AutoPilot-profiler til å kontrollere hvordan Windows er installert på brukerenheter. Profilene inneholder følgende innstillinger.
  
 **AutoPilot standardfunksjoner (obligatorisk) som angis automatisk:**
  
|**Innstilling**|**Beskrivelse**|
|:-----|:-----|
|Hopp over Cortana-, OneDrive- og OEM-registrering  <br/> |Hopper over installasjonen av forbrukerapper som Cortana og personlig OneDrive. Enhetsbrukeren kan installere disse senere så lenge brukeren er en lokal administrator på enheten. Den opprinnelige produsenten registrering en hoppes over fordi enheten vil bli administrert av Microsoft 365 Business.  <br/> |
|Logg på erfaring med bedriftens merkevare  <br/> |Hvis firmaet har en Legg til firmamerking en [påloggingsside for Office 365](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), får enhetsbrukeren denne opplevelsen når du logger på.  <br/> |
|MDM automatisk registrering med konfigurerte AAD-kontoer.  <br/> |Brukeridentiteten administreres av Azure Active Directory, og brukere logger på Windows og Office 365 med legitimasjonen for Microsoft 365 Business.  <br/> |
   
 **Valgfrie innstillinger:**
  
|**Innstilling**|**Beskrivelse**|
|:-----|:-----|
|Hopp over personverninnstillinger (Av som standard)  <br/> |Hvis dette alternativet er satt til **På**, vil enhetsbrukeren ikke se lisensavtalen for enheten og Windows når han eller hun først logger på.  <br/> |
|Ikke la brukeren bli den lokale administratoren  <br/> |Hvis dette alternativet er satt til **På**, kan ikke enhetsbrukeren installere personlige apper, for eksempel Cortana.<br/> |
   
