---
title: Om innstillinger for AutoPilot-profil
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
description: AutoPilot-profiler hjelper deg med å kontrollere hvordan Windows blir installert på bruker enheter. Profilene inneholder standard og valgfrie innstillinger, for eksempel hopp over Cortana-installasjon.
ms.openlocfilehash: 912a24e3d458986a4bcf7dcf903f80211996aca2
ms.sourcegitcommit: 8193b7da5b1a415835d02ca96883c351df7326ed
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/14/2019
ms.locfileid: "38321789"
---
# <a name="about-autopilot-profile-settings"></a>Om innstillinger for AutoPilot-profil

## <a name="autopilot-profile-settings"></a>Innstillinger for AutoPilot-profilen

Du kan bruke AutoPilot-profiler til å kontrollere hvordan Windows installeres på bruker enheter. Profilene inneholder følgende innstillinger.
  
 **Standard funksjoner for AutoPilot (påkrevd) som stilles inn automatisk:**
  
|**Innstilling**|**Beskrivelse**|
|:-----|:-----|
|Hopp over Cortana, OneDrive og OEM-registrering  <br/> |Hopper over installasjonen av forbruker programmer som Cortana og personlig OneDrive. Enheten brukeren kan installere disse senere så lenge brukeren er en lokal admin på enheten. Den opprinnelige produsenten registreringen er hoppet over fordi enheten vil bli administrert av Microsoft 365 Business.  <br/> |
|Logg på erfaring med firmaets merkevare  <br/> |Hvis firmaet har en [Legg til firmaets merkevarebygging til Office 365 påloggingssiden](https://support.office.com/article/a1229cdb-ce19-4da5-90c7-2b9b146aef0a), vil enheten brukeren får denne opplevelsen når du logger på.  <br/> |
|Automatisk MDM-registrering med konfigurerte AAD-kontoer.  <br/> |Bruker identiteten vil bli administrert av Azure Active Directory, og brukere vil logge på Windows og Office 365 med sine Microsoft 365 Business legitimasjon.  <br/> |
   
 **Valgfrie innstillinger:**
  
|**Innstilling**|**Beskrivelse**|
|:-----|:-----|
|Hopp over personverninnstillinger (av som standard)  <br/> |Hvis dette alternativet er satt til **på**, vil ikke enhets brukeren se lisensavtalen for enheten og Windows når han eller hun først logger på.  <br/> |
|Ikke la brukeren bli den lokale administratoren  <br/> |Hvis dette alternativet er satt til **på**, kan ikke enhets brukeren installere personlige apper, for eksempel Cortana.<br/> |
   
