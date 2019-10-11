---
title: Øk trussel beskyttelsen for Microsoft 365 Business
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Konfigurer samsvarsfunksjoner for å forhindre tap av data og merke sensitive data.
ms.openlocfilehash: a0ba2fa6dbe7c786d577ad7098c1790f569f5acc
ms.sourcegitcommit: 255e8194bb5767a9983d54d16e79d628732a1d97
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/11/2019
ms.locfileid: "37453924"
---
# <a name="set-up-compliance-features"></a>Definere samsvarsfunksjoner

Microsoft 365 Business leveres med funksjoner som beskytter dataene og enhetene dine, og hjelper deg med å holde dine og kundenes sensitive opplysninger sikre.

## <a name="set-up-dlp-features"></a>Definere DLP-funksjoner

Se [opprette en DLP-policy fra en mal](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for å få et eksempel på hvordan du konfigurerer en policy for å beskytte mot personlig identifiserbar informasjon (PII). 
  
DLP leveres med mange maler som er klare til bruk, for mange forskjellige nasjonale innstillinger. For eksempel, Australia Financial data, Canada personlig informasjon Act, amerikanske finansielle data, etc. Se [hva DLP policy malene inkluderer](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for en fullstendig liste. Alle disse malene kan aktiveres på samme måte som PII-mal eksempelet. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Konfigurere e-oppbevaring med Exchange Online-arkivering

 **Exchange Online arkiverings** lisens funksjoner bidrar til å opprettholde samsvar og forskriftsmessige standarder ved å bevare e-innhold for eDiscovery. Det bidrar også til å redusere risikoen i tilfelle en rettssak og gir en måte å gjenopprette data etter et sikkerhetsbrudd, eller når du trenger å gjenopprette slettede elementer. Du kan bruke rettslig sperre for å bevare alt innholdet til en bruker, eller bruke oppbevaringspolicyer til å tilpasse det du vil beholde.
  
**Rettstvist Hold:** Du kan beholde alt postboksinnhold inkludert slettede elementer ved å sette en brukers hele postboksen under rettslig sperre. 
    
Hvis du vil plassere en postboks under rettslig sperre, i administrasjonssenteret:
    
1. I venstre NAV går du til **brukere** \> **aktive brukere**.
    
2. Velg en bruker som har postboksen du vil plassere ved rettslig sperre, og i bruker ruten utvider du **e-postinnstillinger** og ved siden av **flere innstillinger** Velg **Rediger Exchange-egenskaper**.
    
3. På Postboks-siden for brukeren, velger * * postkassen funksjoner * * på venstre nav, og velg deretter **Aktiver** kobling under **rettslig sperre**.
    
4. I dialogboksen **rettslig sperre** kan du angi den rettstvist holde varigheten i feltet **rettstvist Hold varighet** , la feltet stå tomt hvis du vil plassere et uendelig hold. Du kan også legge til notater og dirigere postbokseieren til et webområde du kanskje må forklare mer om den rettslige sperren \> **Lagre**.
    
**Bevaring:** Du kan aktivere egendefinerte oppbevaringspolicyer, for eksempel for å beholde en bestemt tidsperiode eller slette innhold permanent på slutten av oppbevaringsperioden. Hvis du vil ha mer informasjon, kan du se [Oversikt over oppbevaringspolicyer](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-sensitivity-labels"></a>Sette opp følsomhet etiketter

Følsomhet etiketter kommer med Azure Information Protection (AIP) plan 1, og hjelper deg med å klassifisere og eventuelt beskytte dokumenter og e-post, ved å bruke etiketter. Etiketter kan brukes automatisk av administratorer som definerer regler og betingelser, manuelt av brukere, eller ved å bruke en kombinasjon der brukere får anbefalinger.

For å sette opp følsomhet etiketter, se [opprette og administrere følsomhet etiketter](https://support.office.com/en-us/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.



### <a name="install-the-azure-information-protection-client-manually"></a>Installere Azure Information Protection-klienten manuelt

Slik installerer du den AIP-klienten manuelt:

1. Dataoverføre **AzinfoProtection_UL. exe** fra [Microsoft Dataoverføre Senter](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Du kan kontrollere at installasjonen fungerte ved å vise et Word-dokument og sørge for at alternativet **følsomhet** er tilgjengelig i kategorien **hjem** .
<br/>![Kategorien beskyttelse i et Word-dokument.](media/word-sensitivity.png)

Hvis du vil ha mer informasjon, kan [du se installere klienten](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
