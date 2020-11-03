---
title: Øke trussel beskyttelse for Microsoft 365 Business Premium
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Konfigurer samsvars funksjoner for å hindre tap av data, og bidra til at dine og kundenes sensitive opplysninger sikres.
ms.openlocfilehash: 2c95ad3f36df28af2c68cd11192bcfe92dfe29e3
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841177"
---
# <a name="set-up-compliance-features"></a>Konfigurere samsvars funksjoner

Microsoft 365 Business Premium leveres med funksjoner for å beskytte dataene og enhetene dine, og hjelper deg med å holde kundenes sensitive opplysninger sikre.

## <a name="set-up-dlp-features"></a>Konfigurere DLP-funksjoner

Se [opprette en DLP-policy fra en mal](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for et eksempel på hvordan du konfigurerer en policy for beskyttelse mot beskyttelse av tap av personlige data. 
  
DLP leveres med mange policyer som er klare til bruk for mange forskjellige nasjonale innstillinger. Økonomiske data, Canada, personlig informasjon, for eksempel, USA, økonomiske data og så videre. Se [hvordan policy malene for DLP inkluderer](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) en fullstendig liste. Alle disse malene kan være aktivert på samme måte som for eksempel malen PII. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Konfigurere e-postoppbevaring med Exchange Online-arkivering

 Lisens funksjoner for å **arkivere Exchange Online** hjelper deg med å vedlikeholde samsvar og forskriftsmessige standarder ved å beholde e-postinnhold for eDiscovery. Det bidrar også til å redusere risikoen hvis det finnes en lawsuit, og gir deg en mulighet til å gjenopprette data etter et brudd eller når du må gjenopprette slettede elementer. Du kan bruke søksmål hold for å bevare hele en brukers innhold, eller bruke oppbevarings policyer til å tilpasse hva du vil beholde.
  
**Rettslig sperre:** Du kan bevare alt innholdet i post boksen, inkludert slettede elementer ved å legge inn en brukers fullstendige post boks på en rettslig sperre. 
    
Hvis du vil plassere en post boks på en rettslig sperre, kan du i administrasjons senteret:
    
1. Gå til **brukere** som \> **aktive brukere** i venstre navigasjons rute.
    
2. Velg en bruker som har post boksen du vil plassere på en rettslig sperre. I bruker-ruten utvider du **e-postinnstillinger** og klikker **Rediger Exchange-egenskaper** ved siden av **flere innstillinger**.
    
3. På Postboks-siden for brukeren velger du * * post boks funksjoner * * i det venstre navigasjons feltet, og deretter velger du **Aktiver** -koblingen under **rettslig sperring**.
    
4. I dialog boksen retts **tvist** kan du angi den rettslige sperrings varigheten i **varighets** feltet for søksmål-vent. La feltet stå tomt hvis du vil plassere en uendelig sperring. Du kan også legge til notater og dirigere eieren av post boksen til et nettsted du kanskje må forklare mer om den rettslige sperringen. \>**Lagre**.
    
**Oppbevaring:** Du kan aktivere tilpassede oppbevarings policyer, for eksempel for å beholde en bestemt tids periode, eller slette innhold permanent på slutten av oppbevarings perioden. Hvis du vil ha mer informasjon, kan du se [Oversikt over oppbevarings policyer](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).

## <a name="set-up-sensitivity-labels"></a>Konfigurere følsomhet og etiketter

Følsomme etiketter leveres med Azure Information Protection, plan 1 og hjelper deg med å klassifisere, og du kan også beskytte dokumentene og e-postmeldingene dine ved å bruke etiketter. Etiketter kan brukes automatisk av administratorer som definerer regler og betingelser, manuelt av brukere eller ved å bruke en kombinasjon der brukere får anbefalinger.

Hvis du vil sette opp følsomhet for etiketter, kan du vise video om å [opprette og behandle følsomhet](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) .



### <a name="install-the-azure-information-protection-client-manually"></a>Installere Azure Information Protection-klienten manuelt

Slik installerer du den administrative klienten manuelt:

1. Last ned **AzinfoProtection_UL.exe** fra [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Du kan kontrollere at installasjonen fungerte ved å vise et Word-dokument og sørge for at alternativet **følsomhet** er tilgjengelig på **hjem** -fanen.
<br/>![Kategorien beskyttelse i et Word-dokument.](../media/word-sensitivity.png)

Hvis du vil ha mer informasjon, kan du se [installere klienten](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
