---
title: Sikre Windows 10-enheter
f1.keywords:
- CSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4WindowsConfig
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
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
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: Finn ut mer om hvordan du konfigurerer innstillingene for standard enhetspolicy som alle enheter Windows 10 når du logger deg på jobb- eller skolekontoen.
ms.openlocfilehash: d08d33807a6ad724412574c27aecddd8f228ee8d0b6f1e6725d2a0d6d75cab06
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53882045"
---
# <a name="secure-windows-10-devices"></a>Sikre Windows 10-enheter

Denne artikkelen gjelder for Microsoft 365 Business Premium.

Innstillingene du konfigurerer her er en del av standardpolicyen for enheter for Windows 10. Alle brukere som kobler til en Windows 10 enhet, inkludert mobile enheter og PC-er, mottar automatisk disse innstillingene ved å logge på med jobbkontoen sin. Vi anbefaler at du godtar standardpolicyen under konfigurasjonen og legger til policyer senere som retter seg mot bestemte grupper av brukere.
  
## <a name="settings-to-secure-windows-10-devices"></a>Innstillinger for å sikre Windows 10-enheter

Som standard er alle innstillingene **På**. Følgende innstillinger er tilgjengelige:
  


|Innstilling  <br/> |Beskrivelse  <br/> |
|:-----|:-----|
|Beskytte PC mot virus og andre trusler ved hjelp av Windows Defender Antivirus  <br/> |Krever at Windows Defender Antivirus er slått på for å beskytte PC-er fra farene ved å være koblet til Internett.  <br/> |
|Beskytte PC-er fra nettbaserte trusler i Microsoft Edge  <br/> |Slår på innstillinger i Microsoft Edge som beskytter brukere mot skadelige nettsteder og nedlastinger.  <br/> |
|Bruke BitLocker til å beskytte filer og mapper på PC-er mot uautorisert tilgang  <br/> |BitLocker beskytter dataene ved å kryptere harddiskene på datamaskinen og beskytter mot eksponering av dataene dersom en datamaskin mistes eller blir stjålet. Hvis du vil ha mer informasjon, kan du [se Vanlige spørsmål om Bitlocker](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions).  <br/> |
|Slå av skjermen på enheten når den har vært inaktiv i en viss periode  <br/> |Sørger for at bedriftsdata er beskyttet dersom en bruker er inaktiv. En bruker kan jobbe på et offentlig sted, som for eksempel en kaffebar, går bort eller blir distrahert i et øyeblikk, og lar enheten være sårbar for tilfeldig innsyn. Denne innstillingen lar deg bestemme hvor lenge en bruker kan være inaktiv før skjermen slås av.  <br/> |
|