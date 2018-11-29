---
title: Sikkerhetsfunksjonene i Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Lær mer om sikkerhetsfunksjonene som følger med Microsoft 365 Business.
ms.openlocfilehash: bfddb419dbe5db441741a73ecb49e3d52649e382
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983176"
---
# <a name="microsoft-365-business-security-features"></a>Sikkerhetsfunksjonene i Microsoft 365 Business

Microsoft 365 Business tilbyr forenklet sikkerhetsfunksjoner til å beskytte dine data på PCer, telefoner og tavler.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Sikkerhetsfunksjonene i Microsoft 365 Business admin center

Du kan behandle mange av sikkerhetsfunksjonene for Microsoft 365 Business i administrasjonssenteret, som gir deg en enklere måte å slå disse funksjonene på eller av. I administrasjonssenteret kan du gjøre følgende:
  
![Screenshot of the Devices card in the admin center](media/9982e784-dbf9-4a76-a159-bb3e2e5aa23f.png)
  
- [Angi innstillinger for programmet for Android eller iOS-enheter](app-protection-settings-for-android-and-ios.md) . 
    
    Disse innstillingene omfatter sletter filer fra en inaktiv enheten etter en angitt periode, kryptere arbeidsfiler, som krever at brukere angir en PIN-kode, og så videre.
    
- [Angi innstillinger for programmet for Windows 10 enheter](protection-settings-for-windows-10-devices.md) . 
    
    Disse innstillingene kan brukes til firmadataene på begge eies av firmaet eller personlig eies enheter.
    
- [Angi innstillinger for enhet for Windows 10 enheter](protection-settings-for-windows-10-pcs.md) . 
    
    Du kan aktivere [BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) -kryptering til å beskytte dataene i tilfelle en enhet er mistet eller stjålet, og aktiverer [Windows utnytte Guard](https://go.microsoft.com/fwlink/p/?linkid=871404) til gir avansert beskyttelse mot ransomware. 
    
- [Fjerne firmadata fra enheter](remove-company-data.md)
    
    Du kan tørke firmadata eksternt hvis en enhet blir stjålet, eller en ansatt forlater firmaet.
    
- [Tilbakestille Windows-10 enheter til fabrikkinnstillinger](reset-devices-to-factory-settings.md) . 
    
    Du kan tilbakestille Windows 10-enheter som har Enhetsinnstillinger for databeskyttelse brukes.
    
## <a name="additional-security-features"></a>Ekstra sikkerhetsfunksjoner 

Avanserte funksjoner i Microsoft 365 Business er tilgjengelig for å hjelpe deg med å beskytte bedriften mot cyber trusler og beskytte sensitiv informasjon.
  
- **[Office 365 avanserte Threat Protection](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Avansert Threat Protection (ATP) verne bidrar til å bedriften mot avanserte phishing og ransomware angrep som er laget for å bryte ansatt eller kundeinformasjon. Funksjoner:
    
  - Avanserte vedlegg skanning og AI-drevet analyse for å oppdage og fjerne farlige meldinger.
    
  - Automatisk kontrollerer web-koblinger i e-post for å vurdere om de er en del av et phishing-forsøk. Dette holder deg sikker tilgang til usikre webområder.
    
- **[Oversikt over datapolicyer tap forebygging](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    Du kan definere DLP til å automatisk gjenkjenne sensitiv informasjon, som kredittkortnumre, personnummer, etc. å forhindre deres utilsiktet deling utenfor firmaet.
    
- **[Exchange Online Archiving](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online-arkivering lisens gjør at meldingene kan lett bli arkivert med sammenhengende data backup. Den lagrer alt i en brukers e-postmeldinger, inkludert Slettede elementer, i tilfelle de kreves for gjenkjenning eller gjenoppretting senere. Du kan også bruke ulike oppbevaringspolicyer å beholde e-data for rettstvist sperringer, eDiscovery, eller for å oppfylle krav til samsvar.
    
- **[Azure informasjonsbeskyttelse](https://go.microsoft.com/fwlink/p/?linkid=871406)**
    
    Informasjon om beskyttelse hjelper du styre tilgang til sensitiv informasjon i e-post og dokumenter med kontroller som "Ikke Videresend" og "Kopieres ikke". Du kan klassifisere sensitiv informasjon som "Konfidensielt", og du kan angi hvordan klassifisert informasjon kan deles utenfor og innenfor virksomheten. Bedriftsnivå kryptering er enkelt å bruke e-post og dokumenter til å holde informasjonen din privat. Microsoft 365 Business inneholder alle funksjonene i [Azure informasjon beskyttelse Plan 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Du kan også installere tillegget for beskyttelse mot Azure-informasjon-klienten for Office-programmer. Hvis du vil ha mer informasjon, kan du se [Azure informasjonsbeskyttelse klienten administratoren guide](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide).
    
- **[Alle egenskapene i Intune i Azure portal](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Tilgang til Intune administrasjonssenteret i Azure portal kan du definere ytterligere sikkerhetsfunksjoner, for eksempel administrasjon av MacOS enheter, iPhone og Android enheter sammen med avansert Enhetsbehandling for Windows, som ikke er tilgjengelige via Microsoft 365 business administrasjonssenteret.
    
De neste avsnittene beskriver hvordan du kan administrere disse funksjonene i sikkerheten &amp; overholdelsessenteret og Intune administrasjonssenteret. Forenklet kontrollene vil bli lagt til administrasjonssenteret for Microsoft 365 Business over tid.
  
## <a name="set-up-advanced-threat-protection-features"></a>Konfigurer avanserte Threat Protection funksjoner

- **Beskyttelse mot usikre vedlegg:** ATP identifiserer skadelig innhold ved å åpne e-postvedlegg i et virtuelt miljø og utføre analyse av den resulterende atferden. Innholdet er evaluert for å finne sin hensikt (enten vanlig eller skadelig), og ATP blokkerer leveringen av usikre vedlegg, bidrar til å beskytte deg mot phishing-forsøk og ransomware infeksjoner. Hvis du vil aktivere beskyttelse for vedlegg, kan du se [definere policyer for Office 365 ATP trygt vedlegg](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775).
    
- Beskytte miljøet når brukere klikker skadelig koblinger: ATP undersøker også koblinger i e-post når en bruker klikker dem.. Hvis en kobling er usikre, er brukeren varsles om ikke å gå til webområdet eller informert om at webområdet er blokkert. Dette bidrar til å beskytte deg mot phishing-forsøk. Du kan [definere policyer for Office 365 ATP-klarerte koblinger](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) eller [definere policyer for Office 365 ATP-klarerte koblinger](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).
    
## <a name="set-up-dlp-features"></a>Konfigurer DLP-funksjoner

Se [opprette en DLP policy fra en mal](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for et eksempel på hvordan du konfigurerer en policy for beskyttelse mot personlig identifiserbar informasjon (PII). 
  
DLP leveres med mange klare til bruk policymaler for mange forskjellige nasjonale innstillinger. For eksempel økonomiske Data for Australia, Canada personlig informasjon Act, amerikanske økonomiske Data, osv. Se [Hva the DLP maler for gruppepolicy inneholder](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) en fullstendig liste. Alle disse malene kan aktiveres ligner eksemplet PII mal. 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a>Definer tilbakeholdelse av e-post med Exchange Online-arkivering

 **Exchange Online-arkivering** lisens funksjoner gir deg muligheten til å opprettholde overensstemmelse og forskriftsmessige standarder ved å beholde e-post innhold med tanke på eDiscovery. I tillegg bidrar til å redusere risiko i tilfelle rettstvist og gjør det mulig å gjenopprette data etter brudd på sikkerheten eller når du skal gjenopprette slettede elementer. Hvis du vil aktivere disse funksjonene, kan du bruke rettstvist hold for å beholde alt innholdet i en brukers, eller bruke oppbevaringspolicyer for større tilpasning. 
  
**Rettstvist sperring:** Du kan beholde alle postboksinnholdet inkludert Slettede elementer ved å plassere hele postboksen for en bruker i rettstvist holder. 
    
Hvis du vil plassere en postboks på rettstvist hold, i administrasjonssenteret:
    
1. Gå til **brukere** i den venstre nav, \> **aktive brukere**.
    
2. Velg en bruker som har postboksen du vil plassere på rettstvist holder og Utvid **e-postinnstillinger** i ruten til brukeren og ved siden av **flere innstillinger** velger du **Rediger Exchange egenskaper**.
    
3. På postboks-siden for brukeren å velge ** postboks funksjoner ** på venstre nav, og velg deretter **Aktiver** koblingen under **rettstvist holder**.
    
4. **Rettstvist holder** dialogboksen kan du angi rettstvisten Hold nede-varighet i **rettstvist Hold nede-varighet** -feltet, la feltet stå tomt hvis du vil plassere en uendelig sperring. Du kan også legge til merknader og direkte eieren av e-post-boksen til et webområde, må du kanskje forklare mer om rettstvisten holder \> **Lagre**.
    
**Oppbevaring:** Du kan aktivere tilpassede policyer for dokumentoppbevaring, for eksempel å bevare i en bestemt tidsperiode eller slette innholdet permanent på slutten av Oppbevaringstiden. Hvis du vil ha mer informasjon, se [Oversikt over policyer for dokumentoppbevaring](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).
## <a name="set-up-azure-information-protection-features"></a>Sett opp funksjoner for beskyttelse mot Azure-informasjon

Azure informasjon beskyttelse (AIP) er en sky-basert løsning som bidrar til en organisasjon til å klassifisere og du kan også beskytte dokumenter og e-postmeldinger ved å bruke etiketter. Etiketter kan brukes automatisk som administratorer definerer regler og betingelser, manuelt av brukere, eller en kombinasjon, der brukere får anbefalinger.

Muligheten til å bruke følgende begrensninger når du sender e-postmeldinger i Outlook på weben er automatisk aktivert for alle brukere:
  
- **Ikke Videresend**: kan mottakere lese meldingen, men de kan ikke videresende, skrive ut eller kopiere innhold
    
- **Kryptere**: hele meldingen er kryptert. Mottakerne må gjøre ekstra for å bekrefte sin identitet før du åpner kryptert innhold og kan ikke fjerne kryptering.
    
- **Konfidensielt**: gir ansatte i organisasjonen alle tillatelser til e-post-innhold og vedlegg, men ikke til personer utenfor organisasjonen. Dataeiere kan spore og oppheve innhold når som helst.
    
- **Høyst konfidensiell**: Denne restriksjonen kan brukes på svært konfidensielle data, slik at ansatte kan vise, redigere, og svar, men ikke videresende, skrive ut eller kopiere data. Dataeiere kan spore og oppheve innhold når som helst.

### <a name="make-sure-azure-information-protection-is-activated"></a>Kontroller at Azure informasjonsbeskyttelse er aktivert

Slik kontrollerer du at AIP er aktivert:

1. Logge på [administrasjonssenteret Azure Active Directory](https://portal.azure.com/).

    Du kan også Synge i ved å finne **centers Admin** \> **Azure Active Directory** i venstre navigasjon i administrasjonssenteret.

2. Velg **alle tjenester** og tyoe i *Azure informasjonsbeskyttelse* i **Søk-boksen**.

3. Når resultatet vises, klikker du start neste **Azure informasjonsbeskyttelse** for å gjøre den til favoritt og lett å finne senere.

4. Velg **Azure informasjonsbeskyttelse** \> **Beskyttelse aktivering** , og kontroller at statusen er satt til aktivert. 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a>Vise informasjon om beskyttelse av Azure policy og standard etikettene 

Hvis du vil vise og endre, eksisterende etiketter:

1. Velg **klassifiseringer** på instrumentbordet Azure informasjonsbeskyttelse \> ** etiketter. <br/>![Standard etiketter for Azure informasjonsbeskyttelse.](media/AIPLabels.png)

2. Du kan velge en etikett til å vise alternativene, kan du endre visningsnavnet, farger og så videre.
 
3. Se [endre og opprette nye etiketter](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) Hvis du vil opprette dine egne. 

### <a name="install-the-azure-information-protection-client-manually"></a>Installere klienten Azure informasjonsbeskyttelse manuelt

Å manuelt installere AIP-klient:

1. Last ned **AzInfoProtection.exe** fra [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).
 
2. Du kan kontrollere at installasjonen arbeidet ved å vise et Word-dokument og kontrollere at alternativet **Beskytt** er tilgjengelige i kategorien **Hjem** . <br/>![Kategorien beskyttelse rullegardinlisten i et Word-dokument.](media/Word_Protect.png)

For mer informasjon, se [installere klienten](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3)
    
## <a name="faq"></a>Vanlige spørsmål

 ### <a name="are-these-security-features-available-in-all-markets"></a>Er disse sikkerhetsfunksjonene som er tilgjengelige i alle markeder?
  
Ja, disse funksjonene er tilgjengelige i alle land der Microsoft 365 Business selges.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Hvordan finner jeg sikkerheten &amp; overholdelsessenteret?
  
1. [Logg på Microsoft 365 Business](https://portal.microsoft.com/) ved hjelp av admin-rettigheter. 
    
2. I den venstre nav, Finn **centers Admin** og utvide den. 
    
    ![Velg Admin-sentre i den venstre nav i administrasjonssenteret for Microsoft 365.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Velg **Sikkerhet &amp; kompatibilitet** å gå til sikkerhet &amp; overholdelsessenteret. 
    
 ### <a name="how-do-i-find-the-intune-admin-center"></a>Hvordan finner administrasjonssenteret Intune?
  
  
1. [Logg på Microsoft 365 Business](https://portal.microsoft.com/) ved hjelp av admin-rettigheter. 
    
2. I den venstre nav, Finn **centers Admin** og utvide den. 
    
3. Velg **Intune** for å gå til administrasjonssenteret Intune. 
    

