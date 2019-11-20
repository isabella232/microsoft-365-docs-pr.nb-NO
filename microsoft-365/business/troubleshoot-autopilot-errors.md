---
title: Feilsøke AutoPilot-enheter
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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Finn ut hvordan du feilsøker feil i AutoPilot-enheten.
ms.openlocfilehash: 1b5358bd6686c2548e82ec5297ac0ad675835718
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718703"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Feilsøke AutoPilot-enheter

## <a name="device-file-error-messages"></a>Feilmeldinger for enhetsfiler

Her er informasjon om noen av feilene du kan se mens du arbeider med AutoPilot enhetsfiler i Microsoft 365 Business. 
  
|**Feilkode**|**Fix å prøve**|
|:-----|:-----|
|Ugyldig forespørsels tekst  <br/> |Denne feilen oppstår sjelden, hvis du ser denne feilen, kan du prøve operasjonen på nytt.  <br/> |
|Maskinvarenummer verdi for en enhet er ikke riktig.  <br/> |Hvis du ser denne feilen, betyr det at verdien du angav i CSV-filen for maskinvarenummeret til én enhet, ikke er riktig. Først må du kontrollere at verdien ble skrevet inn riktig. Hvis du tror at verdien er riktig, men denne feilen fortsatt skjer, kan du be maskinvareleverandøren om hjelp.  <br/> |
|Enhet som er tilordnet en annen Tenant  <br/> |Hvis du ser denne feilen, betyr det at verdien du angav i CSV-filen for enten serienummeret eller produktnøkkelen til én eller flere enheter, ikke er riktig. Først må du kontrollere at verdien ble skrevet inn riktig. Hvis du tror at verdien er riktig, men denne feilen fortsatt skjer, kan du be maskinvareleverandøren om hjelp.  <br/> |
|CSV-filen inneholder et ugyldig serienummer eller en produktnøkkel  <br/> |Hvis du ser denne feilen, betyr det at enheten du prøver å registrere, allerede er registrert av en annen organisasjon. Spør maskinvareleverandøren om hjelp for å rette opp denne feilen.  <br/> |
|Denne enheten støttes ikke for installasjon ved hjelp av AutoPilot  <br/> | Denne feilen betyr at enheten ikke oppfyller kravene til distribusjon av AutoPilot. Enheter må oppfylle disse kravene:  <br/>  Windows 10 versjon 1703 eller senere.  <br/>  Ny anordninger det har ikke ' blitt igjennom Vinduer ut-av-bokse med erfaring.  <br/> |
|Finner ikke enheten  <br/> |Denne feilen betyr at én eller flere enheter i CSV-filen ikke er registrert i organisasjonen. Du kan løse dette problemet ved å be maskinvareleverandøren om hjelp.  <br/> |
