---
title: Feilsøke AutoPilot-enheter
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: troubleshooting
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Lær hvordan du feilsøker AutoPilot filfeil.
ms.openlocfilehash: 9b8d8ab424dd3189ff5c228dab8f5c513ff5dafc
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982746"
---
# <a name="troubleshoot-autopilot-device-errors"></a>Feilsøke AutoPilot-enheter

## <a name="device-file-error-messages"></a>Feilmeldinger-filen for enheten

Her er informasjon om noen av feilene som du kan se mens du arbeider med filer i AutoPilot-enhet i Microsoft 365 Business. 
  
|**Feilkode**|**Løsning å prøve**|
|:-----|:-----|
|Ugyldig forespørselens brødtekst  <br/> |Denne feilen skjer sjelden, hvis du ser denne feilen, kan du prøve operasjonen på nytt.  <br/> |
|Maskinvarenummer for en enhet er ikke riktig.  <br/> |Hvis du ser denne feilen, betyr det at verdien du har angitt i CSV-filen for maskinvarenummeret for én enhet er ikke riktig. Først bekrefter du at verdien er riktig skrevet. Hvis du tror at verdien er riktig, men denne feilen skjer fortsatt, spør din maskinvareleverandør for hjelp.  <br/> |
|Enheten som er tilordnet til en annen leier  <br/> |Hvis du ser denne feilen, betyr det at verdien du har angitt i CSV-filen for serienummeret eller en produktnøkkel for én eller flere enheter ikke er riktig. Først bekrefter du at verdien er riktig skrevet. Hvis du tror at verdien er riktig, men denne feilen skjer fortsatt, spør din maskinvareleverandør for hjelp.  <br/> |
|CSV-filen inneholder en ugyldig serienummer eller produktnøkkelen  <br/> |Hvis du ser denne feilen betyr det at du er under forsøk på å registrere enheten allerede er registrert av en annen organisasjon. Hvis du vil løse dette problemet ved å be maskinvareleverandøren for å få hjelp.  <br/> |
|Denne enheten støttes ikke for installasjon ved hjelp av AutoPilot  <br/> | Denne feilen betyr at enheten ikke oppfyller kravene for AutoPilot-distribusjon. Enhetene må oppfylle disse kravene:  <br/>  Windows 10 versjon 1703 eller senere.  <br/>  Nye enheter som ikke har vært gjennom Windows out-of-box experience.  <br/> |
|Finner ikke enhet  <br/> |Denne feilen betyr at en eller flere enheter i CSV-filen ikke er registrert for organisasjonen. Hvis du vil løse dette problemet ved å be maskinvareleverandøren for å få hjelp.  <br/> |
   
