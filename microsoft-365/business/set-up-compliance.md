---
title: Øke trusselbeskyttelse for Microsoft 365 Business Premium
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
search.appverid:
- BCS160
- MET150
description: Konfigurer samsvarsfunksjoner for å forhindre tap av data og bidra til å holde kundenes sensitive informasjon sikret.
ms.openlocfilehash: e0d853223c7e6f455cba6e68ad173b137992d863
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/21/2020
ms.locfileid: "43635128"
---
# <a name="set-up-compliance-features"></a>Konfigurere samsvarsfunksjoner

Microsoft 365 Business Premium leveres med funksjoner for å beskytte data og enheter, og hjelper deg med å holde den sensitive informasjonen din og kundenes sensitive informasjon sikker.

## <a name="set-up-dlp-features"></a>Konfigurere DLP-funksjoner

Se [Opprette en DLP-policy fra en mal](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for eksempel hvordan du konfigurerer en policy for å beskytte mot personlig identifiserbar informasjon (PII). 
  
DLP leveres med mange policymaler som er klare til bruk for mange forskjellige nasjonale innstillinger. For eksempel, Australia Financial Data, Canada Personal Information Act, US Financial Data, og så videre. Se [Hva DLP-policymalene inneholder](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for en fullstendig liste. Alle disse malene kan aktiveres på samme måte som pii-maleksemplet. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Konfigurere e-postoppbevaring med Exchange Online-arkivering

 **Lisensfunksjoner for Exchange Online Arkivering** bidrar til å opprettholde samsvars- og forskriftsstandarder ved å bevare e-postinnhold for eDiscovery. Det bidrar også til å redusere risikoen hvis det er et søksmål, og gir en måte å gjenopprette data etter et sikkerhetsbrudd eller når du trenger å gjenopprette slettede elementer. Du kan bruke rettstvistsperring til å bevare alt innholdet i en bruker, eller bruke oppbevaringspolicyer til å tilpasse det du vil beholde.
  
**Rettstvist hold:** Du kan beholde alt postboksinnhold, inkludert slettede elementer, ved å sette hele postboksen til en bruker på rettstvist. 
    
Hvis du vil plassere en postboks på rettslig sperre, i administrasjonssenteret:
    
1. Gå til **Brukere** \> **aktive brukere**i venstre navigasjonsenhet.
    
2. Velg en bruker du vil plassere postboksen for å plassere på rettstvistsperring. I brukerruten utvider du **E-postinnstillinger**og ved siden av **Flere innstillinger**, velger **Rediger Exchange-egenskaper**.
    
3. Velg ** postboksfunksjoner ** til venstre, på postbokssiden for brukeren, og velg deretter **Koblingen Aktiver** under **Sperreavhold**.
    
4. I dialogboksen **sperreavrettslig sperre** kan du angi varigheten for rettstvistsperren i feltet **Sperrevarighet for rettstvist.** La feltet stå tomt hvis du vil plassere et uendelig hold. Du kan også legge til notater og dirigere eieren av postboksen til et nettsted du kanskje må forklare mer om rettstvistsperren. \>**Lagre**.
    
**Oppbevaring:** Du kan aktivere egendefinerte oppbevaringspolicyer, for eksempel for å bevare for en bestemt tidsperiode eller slette innhold permanent på slutten av oppbevaringsperioden. Hvis du vil ha mer informasjon, kan du se [Oversikt over oppbevaringspolicyer](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-sensitivity-labels"></a>Konfigurere følsomhetsetiketter

Følsomhetsetiketter leveres med Azure Information Protection (AIP) Plan 1, og hjelper deg med å klassifisere, og eventuelt beskytte dokumenter og e-postmeldinger ved å bruke etiketter. Etiketter kan brukes automatisk av administratorer som definerer regler og betingelser, manuelt av brukere, eller ved hjelp av en kombinasjon der brukerne får anbefalinger.

Hvis du vil konfigurere Følsomhetsetiketter, kan du vise [video om oppretting og administrering av følsomhetsetiketter.](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)



### <a name="install-the-azure-information-protection-client-manually"></a>Installere Azure Information Protection-klienten manuelt

Slik installerer du AIP-klienten manuelt:

1. Last ned **AzinfoProtection_UL.exe** fra [Microsoft nedlastingssenter](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Du kan kontrollere at installasjonen fungerte ved å vise et Word-dokument og kontrollere at alternativet **Følsomhet** er tilgjengelig i kategorien **Hjem.**
<br/>![Rullegardinlisten Beskyttelse-fanen i et Word-dokument.](../media/word-sensitivity.png)

Hvis du vil ha mer informasjon, kan du se [Installere klienten](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
