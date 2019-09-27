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
description: Konfigurer Office 365 avansert trusselbeskyttelse, og Beskytt sensitive data.
ms.openlocfilehash: 8144bcebe8a0cdf28a5e092f592362922ccbdd48
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288749"
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

## <a name="set-up-azure-information-protection-features"></a>Konfigurere funksjoner for Azure informasjonsbeskyttelse

Azure Information Protection (AIP) hjelper deg med å klassifisere og eventuelt beskytte dokumentene og e-postmeldingene ved å bruke etiketter. Etiketter kan brukes automatisk av administratorer som definerer regler og betingelser, manuelt av brukere, eller ved å bruke en kombinasjon der brukere får anbefalinger.

I Outlook på nettet kan du bruke følgende innebygde etiketter og begrensninger på e-postene dine:
  
- **Ikke Videresend**: mottakerne kan lese meldingen, men de kan ikke videresende, skrive ut eller kopiere innhold
    
- **Krypter**: hele meldingen er kryptert. Mottakerne må bekrefte identiteten sin før de får tilgang til kryptert innhold og ikke kan fjerne kryptering.
    
- **Konfidensielt**: gir de ansatte i organisasjonen full tilgang til e-innhold og vedlegg, men ikke til personer utenfor organisasjonen. Data eiere kan spore og tilbakekalle innhold på et hvilket som helst tidspunkt.
    
- **Svært konfidensielt**: denne begrensningen kan brukes på svært konfidensielle data, slik at de ansatte til å vise, redigere og svare, men ikke videresende, skrive ut eller kopiere dataene. Data eiere kan spore og tilbakekalle innhold på et hvilket som helst tidspunkt.

### <a name="make-sure-azure-information-protection-is-activated"></a>Kontroller at Azure Information Protection er aktivert

Slik kontrollerer du at AIP er aktivert:

1. Logg på [Azure-portalen](https://portal.azure.com/).

2. Velg **alle tjenester** og skriv inn *Azure informasjonsbeskyttelse* i **søkeboksen**.

3. Når resultatene vises, klikker du på Start ved siden av **Azure Information Protection** for å gjøre det til en favoritt og lett å finne senere.

4. Velg aktivering av **Azure informasjonsbeskyttelse** \> **beskyttelse** og kontroller at statusen er satt til aktivert. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Vise policyen for Azure informasjonsbeskyttelse og standard etiketter 

Hvis du vil vise, og endre, de eksisterende etikettene:

1. Velg **klassifiserings** \> **etiketter**på instrumentbordet for Azure informasjonsbeskyttelse. <br/>![Standard etiketter for Azure Information Protection.](media/AIPLabels.png)

2. Du kan velge hvilken som helst etikett for å vise alternativer, du kan endre visningsnavnet, farger, etc.
 
3. Se [endre og opprette nye etiketter](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) hvis du vil lage dine egne. 

### <a name="install-the-azure-information-protection-client-manually"></a>Installere Azure Information Protection-klienten manuelt

Slik installerer du den AIP-klienten manuelt:

1. Dataoverføre **AzInfoProtection. exe** fra [Microsoft Dataoverføre Senter](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Du kan kontrollere at installasjonen fungerte ved å vise et Word-dokument og sørge for at alternativet **Beskytt** er tilgjengelig i kategorien **hjem** . <br/>![Kategorien beskyttelse i et Word-dokument.](media/Word_Protect.png)

Hvis du vil ha mer informasjon, kan [du se installere klienten](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
