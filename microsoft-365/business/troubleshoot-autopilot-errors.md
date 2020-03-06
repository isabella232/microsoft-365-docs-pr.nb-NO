---
title: Feilsøke AutoPilot-enheter
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: troubleshooting
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Lær hvordan du feilsøker feil du kan se mens du arbeider med AutoPilot-enhetsfiler i Microsoft 365 Business.
ms.openlocfilehash: 7569f18097a1f5959b3dd491958c78886e1e05d6
ms.sourcegitcommit: 41c0bc5cf50f4ca63b4286d1ea0f58ab82984b7a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2020
ms.locfileid: "42547475"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Feilsøke AutoPilot-enheter

## <a name="device-file-error-messages"></a>Feilmeldinger i enhetsfilen

Her er informasjon om noen av feilene du kan se mens du arbeider med AutoPilot-enhetsfiler i Microsoft 365 Business. 
  
|**Feilkode**|**Fiks for å prøve**|
|:-----|:-----|
|Ugyldig forespørselstekst  <br/> |Denne feilen bør skje sjelden, hvis du ser denne feilen, kan du prøve operasjonen på nytt.  <br/> |
|Maskinvarehashverdien for en enhet er ikke riktig.  <br/> |Hvis du ser denne feilen, betyr det at verdien du oppga i CSV-filen for maskinvarehashen på én enhet, ikke er riktig. Kontroller først at verdien ble skrevet inn på riktig måte. Hvis du tror at verdien er riktig, men denne feilen fortsatt skjer, kan du be maskinvareleverandøren om hjelp.  <br/> |
|Enhet tilordnet til en annen leier  <br/> |Hvis du ser denne feilen, betyr det at verdien du oppga i CSV-filen for serienummeret eller produktnøkkelen til én eller flere enheter, ikke er riktig. Kontroller først at verdien ble skrevet inn på riktig måte. Hvis du tror at verdien er riktig, men denne feilen fortsatt skjer, kan du be maskinvareleverandøren om hjelp.  <br/> |
|CSV-filen inneholder et ugyldig serienummer eller produktnøkkel  <br/> |Hvis du ser denne feilen, betyr det at enheten du prøver å registrere allerede er registrert av en annen organisasjon. Hvis du vil løse denne feilen, kan du be maskinvareleverandøren om hjelp.  <br/> |
|Denne enheten støttes ikke for oppsett ved hjelp av AutoPilot  <br/> | Denne feilen betyr at enheten ikke oppfyller autopilotdistribusjonskravene. Enheter må oppfylle disse kravene:  <br/>  Windows 10 versjon 1703 eller senere.  <br/>  Nye enheter som ikke har vært gjennom Windows out-of-box-opplevelse.  <br/> |
|Finner ikke enheten  <br/> |Denne feilen betyr at én eller flere enheter i CSV-filen ikke er registrert i organisasjonen. Hvis du vil løse dette problemet, kan du be maskinvareleverandøren om hjelp.  <br/> |
