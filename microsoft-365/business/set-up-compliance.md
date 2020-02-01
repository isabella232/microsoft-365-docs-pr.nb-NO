---
title: Øke trusselbeskyttelse for Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
description: Konfigurer samsvarsfunksjoner for å forhindre tap av data og merke sensitive data.
ms.openlocfilehash: 09619de03aafde37106fb3942890b457c488ad43
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593409"
---
# <a name="set-up-compliance-features"></a>Konfigurere samsvarsfunksjoner

Microsoft 365 Business leveres med funksjoner for å beskytte dataene og enhetene dine, og hjelper deg med å holde din og kundenes sensitive informasjon sikker.

## <a name="set-up-dlp-features"></a>Konfigurere DLP-funksjoner

Se [Opprette en DLP-policy fra en mal](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for et eksempel på hvordan du konfigurerer en policy for å beskytte mot personlig identifiserbar informasjon (PII). 
  
DLP leveres med mange policymaler som er klare til bruk for mange forskjellige nasjonale innstillinger. For eksempel Australia Financial Data, Canada Personal Information Act, Us Financial Data, og så videre. Se [Hva DLP-policymalene inkluderer](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for en fullstendig liste. Alle disse malene kan aktiveres på samme måte som pii-maleksemplet. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Definere e-postoppbevaring med Exchange Online-arkivering

 **Exchange Online Arkivering** lisensfunksjoner bidrar til å opprettholde samsvar og forskriftsmessige standarder ved å bevare e-postinnhold for eDiscovery. Det bidrar også til å redusere risikoen hvis det er et søksmål, og gir en måte å gjenopprette data etter et sikkerhetsbrudd eller når du trenger å gjenopprette slettede elementer. Du kan bruke rettstvist hold for å bevare alt innholdet til en bruker, eller bruke oppbevaringspolicyer til å tilpasse det du vil beholde.
  
**Rettstvist hold:** Du kan beholde alt postboksinnhold, inkludert slettede elementer, ved å sette hele postboksen til en bruker på sperrelse av rettssaker. 
    
Hvis du vil plassere en postboks på sperrelse, i administrasjonssenteret:
    
1. Gå til **Brukere** \> **aktive brukere**i venstre navigasjonsenhet.
    
2. Velg en bruker med postboksen du vil plassere på rettstvisthold. Utvid **E-postinnstillinger**i brukerruten, og velg **Rediger Exchange-egenskaper**ved siden av **Flere innstillinger**.
    
3. Velg ** postboksfunksjoner ** til venstre navigasjonsenhet på postbokssiden for brukeren, og velg deretter **Aktiver-koblingen** under **Rettstvist hold**.
    
4. I dialogboksen Sperre av **rettssaker** kan du angi prosedyresperrevarigheten i feltet **Prosedyresperrevarighet.** La feltet stå tomt hvis du vil plassere et uendelig hold. Du kan også legge til notater og lede eieren av postboksen til et webområde du kanskje må forklare mer om rettstvistholdet. \>**Lagre**.
    
**Oppbevaring:** Du kan for eksempel aktivere tilpassede oppbevaringspolicyer for å beholde for en bestemt tidsperiode eller slette innhold permanent på slutten av oppbevaringsperioden. Hvis du vil ha mer informasjon, kan du se [Oversikt over oppbevaringspolicyer](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-sensitivity-labels"></a>Konfigurere følsomhetsetiketter

Følsomhetsetiketter leveres med Azure Information Protection (AIP) Plan 1, og hjelper deg med å klassifisere og eventuelt beskytte dokumenter og e-postmeldinger ved å bruke etiketter. Etiketter kan brukes automatisk av administratorer som definerer regler og betingelser, manuelt av brukere eller ved hjelp av en kombinasjon der brukere får anbefalinger.

Hvis du vil konfigurere følsomhetsetiketter, kan du vise [opprette og administrere videoen for følsomhetsetiketter.](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)



### <a name="install-the-azure-information-protection-client-manually"></a>Installere Azure Information Protection-klienten manuelt

Slik installerer du AIP-klienten manuelt:

1. Last ned **AzinfoProtection_UL.exe** fra [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Du kan kontrollere at installasjonen fungerte ved å vise et Word-dokument og sørge for at **følsomhetsalternativet** er tilgjengelig i kategorien **Hjem.**
<br/>![Rullegardinlisten Beskyttelse-fanen i et Word-dokument.](media/word-sensitivity.png)

Hvis du vil ha mer informasjon, kan du se [Installere klienten](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
