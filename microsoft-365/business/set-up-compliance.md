---
title: Øke trusselen beskyttelse for Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
description: Angi Office 365 Avansert trussel beskyttelse, og beskytte sensitive data.
ms.openlocfilehash: 53741a7726222bb32329a401953be72257df95cc
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086356"
---
# <a name="set-up-compliance-features"></a>Sett opp funksjoner for kompatibilitet

Bedriften din Microsoft-365 leveres med funksjoner for å beskytte dine data og enheter og beskytte din egen og kundenes sensitiv informasjon.

## <a name="set-up-dlp-features"></a>Konfigurer DLP-funksjoner

Se [opprette en DLP policy fra en mal](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for et eksempel på hvordan du konfigurerer en policy for beskyttelse mot personlig identifiserbar informasjon (PII). 
  
DLP leveres med mange klare til bruk policymaler for mange forskjellige nasjonale innstillinger. For eksempel økonomiske Data for Australia, Canada personlig informasjon Act, amerikanske økonomiske Data, osv. Se [Hva the DLP maler for gruppepolicy inneholder](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) en fullstendig liste. Alle disse malene kan aktiveres ligner eksemplet PII mal. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Definer tilbakeholdelse av e-post med Exchange Online-arkivering

 **Exchange Online-arkivering** lisens funksjoner hjelper opprettholde overensstemmelse og forskriftsmessige standarder ved å beholde e-post innhold for eDiscovery. I tillegg bidrar til å redusere risiko i tilfelle en lawsuit og gjør det mulig å gjenopprette data etter brudd på sikkerheten, eller når du skal gjenopprette slettede elementer. Du kan bruke rettstvist hold for å beholde alt innholdet i en brukers eller bruke oppbevaringspolicyer til å tilpasse hva du vil beholde.
  
**Rettstvist sperring:** Du kan beholde alle postboksinnholdet inkludert Slettede elementer ved å plassere hele postboksen for en bruker i rettstvist holder. 
    
Hvis du vil plassere en postboks på rettstvist hold, i administrasjonssenteret:
    
1. Gå til **brukere** i den venstre nav, \> **aktive brukere**.
    
2. Velg en bruker som har postboksen du vil plassere på rettstvist holder og Utvid **e-postinnstillinger** i ruten til brukeren og ved siden av **flere innstillinger** velger du **Rediger Exchange egenskaper**.
    
3. På postboks-siden for brukeren å velge ** postboks funksjoner ** på venstre nav, og velg deretter **Aktiver** koblingen under **rettstvist holder**.
    
4. **Rettstvist holder** dialogboksen kan du angi rettstvisten Hold nede-varighet i **rettstvist Hold nede-varighet** -feltet, la feltet stå tomt hvis du vil plassere en uendelig sperring. Du kan også legge til merknader og direkte eieren av e-post-boksen til et webområde, må du kanskje forklare mer om rettstvisten holder \> **Lagre**.
    
**Oppbevaring:** Du kan aktivere tilpassede policyer for dokumentoppbevaring, for eksempel å bevare i en bestemt tidsperiode eller slette innholdet permanent på slutten av Oppbevaringstiden. Hvis du vil ha mer informasjon, se [Oversikt over policyer for dokumentoppbevaring](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).

## <a name="set-up-azure-information-protection-features"></a>Sett opp funksjoner for beskyttelse mot Azure-informasjon

Azure informasjon beskyttelse (AIP) hjelper deg med å klassifisere, og du kan også beskytte dokumenter og e-post, ved å bruke etiketter. Etiketter kan brukes automatisk som administratorer definerer regler og betingelser, manuelt av brukere eller ved å bruke en kombinasjon, der brukere får anbefalinger.

Du kan bruke følgende innebygde etiketter og begrensninger på e-poster i Outlook på weben:
  
- **Ikke Videresend**: kan mottakere lese meldingen, men de kan ikke videresende, skrive ut eller kopiere innhold
    
- **Kryptere**: hele meldingen er kryptert. Mottakerne må bekrefte sin identitet før du åpner kryptert innhold og kan ikke fjerne kryptering.
    
- **Konfidensielt**: gir ansatte i organisasjonen alle tillatelser til e-post-innhold og vedlegg, men ikke til personer utenfor organisasjonen. Dataeiere kan spore og oppheve innhold når som helst.
    
- **Høyst konfidensiell**: Denne restriksjonen kan brukes på svært konfidensielle data, slik at ansatte kan vise, redigere, og svar, men ikke videresende, skrive ut eller kopiere data. Dataeiere kan spore og oppheve innhold når som helst.

### <a name="make-sure-azure-information-protection-is-activated"></a>Kontroller at Azure informasjonsbeskyttelse er aktivert

Slik kontrollerer du at AIP er aktivert:

1. Logge på [Azure portal](https://portal.azure.com/).

2. Velg **alle tjenester** og type i *Azure informasjonsbeskyttelse* i **Søk-boksen**.

3. Når resultatet vises, klikker du start neste **Azure informasjonsbeskyttelse** for å gjøre den til favoritt og lett å finne senere.

4. Velg **Azure informasjonsbeskyttelse** \> **Beskyttelse aktivering** , og kontroller at statusen er satt til aktivert. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Vise informasjon om beskyttelse av Azure policy og standard etikettene 

Hvis du vil vise og endre, eksisterende etiketter:

1. Velg **klassifiseringer** på instrumentbordet Azure informasjonsbeskyttelse \> **etiketter**. <br/>![Standard etiketter for Azure informasjonsbeskyttelse.](media/AIPLabels.png)

2. Du kan velge en etikett til å vise alternativene, kan du endre visningsnavnet, farger og så videre.
 
3. Se [endre og opprette nye etiketter](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) Hvis du vil opprette dine egne. 

### <a name="install-the-azure-information-protection-client-manually"></a>Installere klienten Azure informasjonsbeskyttelse manuelt

Å manuelt installere AIP-klient:

1. Last ned **AzInfoProtection.exe** fra [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Du kan kontrollere at installasjonen arbeidet ved å vise et Word-dokument og kontrollere at alternativet **Beskytt** er tilgjengelige i kategorien **Hjem** . <br/>![Kategorien beskyttelse rullegardinlisten i et Word-dokument.](media/Word_Protect.png)

For mer informasjon, se [installere klienten](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).
