---
title: Øke trusselbeskyttelsen for Microsoft 365 Business Premium
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
description: Konfigurer samsvarsfunksjoner for å forhindre tap av data og bidra til å holde og kundenes sensitive informasjon sikker.
ms.openlocfilehash: 18886ff3a0ba5e99e63c70ef083d7a69c75bac91
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785836"
---
# <a name="set-up-compliance-features"></a>Konfigurere samsvarsfunksjoner

Microsoft 365 Business Premium leveres med funksjoner for å beskytte dataene og enhetene dine, og hjelper deg med å holde og kundenes sensitive informasjon sikker.

## <a name="set-up-dlp-features"></a>Konfigurere DLP-funksjoner

Se [Opprette en DLP-policy fra en mal,](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for eksempel på hvordan du definerer en policy for å beskytte mot personlig identifiserbar informasjon (PII). 
  
DLP leveres med mange policymaler som er klare til bruk for mange forskjellige lokaliteter. For eksempel, Australia Financial Data, Canada Personal Information Act, US Financial Data, og så videre. Se [Hva DLP-policymalene inkluderer](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) for en fullstendig liste. Alle disse malene kan aktiveres på samme måte som eksempelet på PII-malen. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Konfigurere oppbevaring av e-post med Exchange Online-arkivering

 **Exchange Online Arkivering** lisensfunksjoner bidra til å opprettholde samsvar og forskriftsmessig standarder ved å bevare e-postinnhold for eDiscovery. Det bidrar også til å redusere risikoen hvis det er et søksmål, og gir en måte å gjenopprette data etter et sikkerhetsbrudd eller når du trenger å gjenopprette slettede elementer. Du kan bruke rettslig sperre til å bevare alt innholdet til en bruker, eller bruke oppbevaringspolicyer til å tilpasse det du vil beholde.
  
**Rettstvister holder:** Du kan beholde alt postboksinnhold, inkludert slettede elementer, ved å sette hele postboksen til en bruker på rettslig sperre. 
    
Hvis du vil plassere en postboks på rettslig sperre, i administrasjonssenteret:
    
1. Gå til **Brukere** Aktive brukere i venstre \> **Active users**navigasjonsenhet.
    
2. Velg en bruker som har postboksen du vil plassere på rettslig sperre. Utvid **E-postinnstillinger**i brukerruten, og velg **Rediger Exchange-egenskaper**ved siden av **Flere innstillinger**.
    
3. Velg ** postboksfunksjoner ** i venstre navigasjonsrute på postbokssiden for brukeren, og velg deretter **Aktiver-koblingen** under **Prosedyresperre**.
    
4. I dialogboksen **prosedyresperre** kan du angi varigheten for rettstvisthold i feltet Varighet for **rettstvisthold.** La feltet stå tomt hvis du vil plassere et uendelig grep. Du kan også legge til notater og dirigere eieren av postboksen til et webområde du kanskje må forklare mer om rettstvistholdet. \>**Lagre**.
    
**Oppbevaring:** Du kan for eksempel aktivere tilpassede oppbevaringspolicyer for å bevare for en bestemt tidsperiode eller slette innhold permanent på slutten av oppbevaringsperioden. Hvis du vil ha mer informasjon, kan du se [Oversikt over oppbevaringspolicyer](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).

## <a name="set-up-sensitivity-labels"></a>Definere følsomhetsetiketter

Følsomhetsetiketter leveres med AIP-plan (Azure Information Protection) Plan 1, og hjelper deg med å klassifisere og eventuelt beskytte dokumenter og e-postmeldinger ved å bruke etiketter. Etiketter kan brukes automatisk av administratorer som definerer regler og betingelser, manuelt av brukere eller ved hjelp av en kombinasjon der brukerne får anbefalinger.

Hvis du vil konfigurere følsomhetsetiketter, kan du vise [opprette og administrere følsomhetsetiketter](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.



### <a name="install-the-azure-information-protection-client-manually"></a>Installere Azure Information Protection-klienten manuelt

Slik installerer du AIP-klienten manuelt:

1. Last ned **AzinfoProtection_UL.exe** fra [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Du kan kontrollere at installasjonen fungerte ved å vise et Word-dokument og sørge for at **alternativet Følsomhet** er tilgjengelig i kategorien **Hjem.**
<br/>![Rullegardinlisten Beskyttelsesfane i et Word-dokument.](../media/word-sensitivity.png)

Hvis du vil ha mer informasjon, kan du se [Installere klienten](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
