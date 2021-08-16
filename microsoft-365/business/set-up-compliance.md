---
title: Øk trusselbeskyttelsen for Microsoft 365 Business Premium
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Konfigurer samsvarsfunksjoner for å forhindre tap av data og bidra til å holde sensitiv informasjon for deg og kundene dine sikre.
ms.openlocfilehash: ae5e5727db1f372c40aa4468329021525b6dfc8c5ebbf34705184e461df069e5
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53881853"
---
# <a name="set-up-compliance-features"></a>Konfigurere samsvarsfunksjoner

Din Microsoft 365 Business Premium leveres med funksjoner for å beskytte data og enheter, og hjelpe deg med å holde dine og kundenes sensitive opplysninger sikre.

## <a name="set-up-dlp-features"></a>Konfigurere DLP-funksjoner

Se [Opprette en DLP-policy fra en](../compliance/create-a-dlp-policy-from-a-template.md) mal for et eksempel på hvordan du konfigurerer en policy for å beskytte mot å beskytte tap av personlige data. 
  
DLP leveres med mange policymaler som er klare til bruk for mange forskjellige nasjonale land. For eksempel Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, og så videre. Se [Hva DLP-policymalene inneholder](../compliance/what-the-dlp-policy-templates-include.md) for en fullstendig liste. Alle disse malene kan aktiveres på samme måte som eksempelet på PII-malen. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Konfigurere e-postoppbevaring med Exchange Online Archiving

 **Exchange Online Archiving** lisensfunksjoner bidrar til å opprettholde samsvar og forskriftsmessige standarder ved å bevare e-postinnhold for eDiscovery. Det bidrar også til å redusere risikoen hvis det er et søksmål, og gir en måte å gjenopprette data på etter et sikkerhetsbrudd eller når du trenger å gjenopprette slettede elementer. Du kan bruke rettslig sperring for å bevare alt innholdet til en bruker, eller bruke oppbevaringspolicyer til å tilpasse det du vil bevare.
  
**Rettslig sperre:** Du kan bevare alt postboksinnhold, inkludert slettede elementer, ved å sette hele postboksen til en bruker på rettslig sperre. 
    
Slik plasserer du en postboks på rettslig sperre i administrasjonssenteret:
    
1. Gå til Brukere aktive  brukere i det venstre \> **navigasjonsfeltet.**
    
2. Velg en bruker som har postboksen du vil plassere på rettslig sperre. Utvid E-postinnstillinger **i** brukerruten, og ved siden av Flere innstillinger **velger** du **Rediger Exchange egenskaper**.
    
3. Velg ** postboksfunksjoner ** til venstre på postbokssiden for brukeren,  og velg deretter Aktiver-koblingen under **Rettslig sperring**.
    
4. I dialogboksen **Sperre for** rettslig sperre kan du angi varigheten for rettslig sperring i feltet Varighet **for** rettslig sperre. La feltet stå tomt hvis du vil plassere en uendelig sperring. Du kan også legge til notater og dirigere eieren av postboksen til et nettsted som du kanskje må forklare mer om rettslig sperre. \>**Lagre**.
    
**Oppbevaring:** Du kan aktivere tilpassede oppbevaringspolicyer, for eksempel for å bevare for en bestemt tidsperiode eller slette innhold permanent på slutten av oppbevaringsperioden. Hvis du vil ha mer informasjon, [kan du se Oversikt over oppbevaringspolicyer](../compliance/retention.md).

## <a name="set-up-sensitivity-labels"></a>Konfigurere følsomhetsetiketter

Følsomhetsetiketter leveres med Azure Information Protection (AIP) Plan 1, og hjelper deg med å klassifisere og eventuelt beskytte dokumenter og e-postmeldinger ved å bruke etiketter. Etiketter kan brukes automatisk av administratorer som definerer regler og betingelser, manuelt av brukere, eller ved hjelp av en kombinasjon der brukerne får anbefalinger.

Hvis du vil konfigurere følsomhetsetiketter, [kan du vise video om oppretting og behandling av følsomhetsetiketter.](../business-video/create-sensitivity-labels.md)



### <a name="install-the-azure-information-protection-client-manually"></a>Installere Azure Information Protection-klienten manuelt

Slik installerer du AIP-klienten manuelt:

1. Last **AzinfoProtection_UL.exe** fra [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Du kan kontrollere at installasjonen fungerte ved å vise et Word-dokument og kontrollere at **Følsomhet-alternativet** er tilgjengelig på **Hjem-fanen.**
<br/>![Rullegardinmenyen Beskyttelse-fanen i et Word-dokument.](../media/word-sensitivity.png)

Hvis du vil ha mer informasjon, [kan du se Installere klienten](/azure/information-protection/infoprotect-tutorial-step3).