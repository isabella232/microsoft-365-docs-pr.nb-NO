---
title: Feilsøke AutoPilot-enheter
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: article
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Lær hvordan du feilsøker feil du kan se når du arbeider med AutoPilot-enhetsfiler i Microsoft 365 Business Premium.
ms.openlocfilehash: 1078ab74b07952e4bb565555a081b98ecce9db5c
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578091"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Feilsøke AutoPilot-enheter

## <a name="device-file-error-messages"></a>Feilmeldinger om enhetsfil

Her er informasjon om noen av feilene du kan se når du arbeider med AutoPilot-enhetsfiler i Microsoft 365 Business Premium. 
  
|**Feilkode**|**Løsning for å prøve**|
|:-----|:-----|
|Ugyldig forespørselstekst  <br/> |Denne feilen skal skje sjelden, hvis du ser denne feilen, kan du prøve operasjonen på nytt.  <br/> |
|Hash-verdi for maskinvare for en enhet er ikke riktig.  <br/> |Hvis du ser denne feilen, betyr det at verdien du oppgav i CSV-filen for maskinvare-hash-en på én enhet, ikke er riktig. Kontroller først at verdien ble skrevet inn riktig. Hvis du tror at verdien er riktig, men denne feilen fremdeles oppstår, kan du be maskinvareleverandøren om hjelp.  <br/> |
|Enhet tilordnet til en annen leier  <br/> |Hvis du ser denne feilen, betyr det at verdien du oppgav i CSV-filen for enten serienummeret eller produktnøkkelen på én eller flere enheter, ikke er riktig. Kontroller først at verdien ble skrevet inn riktig. Hvis du tror at verdien er riktig, men denne feilen fremdeles oppstår, kan du be maskinvareleverandøren om hjelp.  <br/> |
|CSV-filen inneholder et ugyldig serienummer eller en produktnøkkel  <br/> |Hvis du ser denne feilen, betyr det at enheten du prøver å registrere, allerede er registrert av en annen organisasjon. Hvis du vil løse denne feilen, kan du be maskinvareleverandøren om hjelp.  <br/> |
|Denne enheten støttes ikke for konfigurasjon ved hjelp av AutoPilot  <br/> | Denne feilen betyr at enheten ikke oppfyller AutoPilot-distribusjonskravene. Enheter må oppfylle disse kravene:  <br/>  Windows 10 versjon 1703 eller senere.  <br/>  Nye enheter som ikke har vært gjennom Windows out-of-box-opplevelsen.  <br/> |
|Finner ikke enheten  <br/> |Denne feilen betyr at én eller flere enheter i CSV-filen ikke er registrert i organisasjonen. Hvis du vil løse dette problemet, kan du be maskinvareleverandøren om hjelp.  <br/> |
