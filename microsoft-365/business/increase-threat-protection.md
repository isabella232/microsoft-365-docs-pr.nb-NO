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
ms.custom:
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Konfigurer Office 365 avansert trusselbeskyttelse, og Beskytt sensitive data.
ms.openlocfilehash: 1827b70f1e4d78a072753390c1a99d7cb4bd5cfd
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/07/2019
ms.locfileid: "38030768"
---
# <a name="increase-threat-protection"></a>Øk trussel beskyttelsen

Denne artikkelen hjelper deg med å øke beskyttelsen i Microsoft 365-abonnementet for å beskytte mot phishing, skadelig programvare og andre trusler. Disse anbefalingene er egnet for organisasjoner med et økt behov for sikkerhet, som advokat kontorer, og helsevesenet klinikker.

Før du begynner, må du sjekke din Office 365 Secure score. Office 365 Secure score analyserer sikkerhet for Office 365-organisasjonen basert på dine vanlige aktiviteter og sikkerhetsinnstillinger, og tildeler en poengsum. Begynn med å notere din nåværende poengsum. Å ta de tiltakene som anbefales i denne artikkelen, øker poengsummen din. Målet er ikke å oppnå maksimal poengsum, men å være klar over muligheter til å beskytte miljøet som ikke negativt påvirker produktiviteten for brukerne. 

Hvis du vil ha mer informasjon, se [Microsoft Secure score](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Heve beskyttelsesnivået mot skadelig programvare i e-post

Office 365-eller Microsoft 365-miljøet omfatter beskyttelse mot skadelig programvare, men du kan øke denne beskyttelsen ved å blokkere vedlegg med filtyper som ofte brukes for skadelig programvare. For å øke malware beskyttelse i e-post:
  
1. Gå til [https://protection.office.com](https://protection.office.com) og Logg på med legitimasjonen for administratorkontoen din. 
    
2. &amp; I Office 365 sikkerhet Compliance Center, i den venstre navigasjonsruten under **trussel behandling**, velger du **policy** \> **anti-malware**.
    
3. Dobbeltklikk standardpolicyen for å redigere denne policyen for hele firmaet.
    
4. Klikk på **Innstillinger**.
    
5. Under **vanlige vedleggstyper filter**velger du **på**. Filtypene som blokkeres, vises i vinduet rett under denne kontrollen.  Pass på at du legger til disse filtyper:
   - ADE, ADP, ANI, BAS, balltre, CHM, cmd, com, cpl, CRT, HLP, HT, HTA, inf, ins, ISP, jobb, JS, jse, lnk, MDA, MDB, MDE, MDZ, msc, MSI, MSP, MST, PCD, reg, scr, SCT, SHS, URL, VB, VBE, VBS, VM, WSF, WSH, exe, PIF  <br/> Du kan legge til eller slette filtyper senere, om nødvendig.
    
6. Klikk **Lagre.**
    
Hvis du vil ha mer informasjon, kan du se [beskyttelse mot skadelig programvare](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Beskytt mot ransomware

Ransomware begrenser tilgangen til data ved å kryptere filer eller låse dataskjermer. Den forsøker deretter å pressepenger fra ofrene ved å be om "løsepenger", vanligvis i form av kryptovalutaer som Bitcoin, i bytte mot tilgang til data. 
  
Du kan beskytte mot ransomware ved å opprette én eller flere e-post flyt regler for å blokkere filtyper som vanligvis brukes til ransomware (disse ble lagt til i [heve nivået for beskyttelse mot skadelig programvare i e-post](#raise-the-level-of-protection-against-malware-in-mail) -trinn), eller for å advare brukere som mottar disse vedlegg i e-post.

I tillegg til filene du blokkerte i forrige trinn, er det også lurt å opprette en regel for å advare brukere før det åpnes vedlegg i Office-filer som inneholder makroer. Ransomware kan skjules i makroer, så vi advarer brukerne mot å åpne disse filene fra personer de ikke kjenner.

Slik oppretter du en regel for e-post transport:
  
1. <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> Gå til administrasjonssenteret og velg **administrasjons** \> senter **utveksling**.
    
2. Klikk **regler**i kategorien **e-postflyt** .
    
3. Klikk **+**, og klikk deretter **Opprett en ny regel**.
    
4. Klikk **flere alternativer** nederst i dialogboksen for å se hele settet med alternativer. 
    
5. Bruk innstillingene i følgende tabell for regelen. La resten av innstillingene være standard, med mindre du vil endre disse.
    
6. Klikk **Lagre**.
    
|**Innstilling**|**Advar brukere før åpning av vedlegg av Office-filer**||
|:-----|:-----|:-----|
|Navn  <br/> |Anti-ransomware regel: advare brukere  <br/>  |
|Bruk denne regelen hvis. . .  <br/> |Alle vedlegg. . . -filtypen samsvarer med. . .  <br/> |
|Angi ord eller uttrykk  <br/> |Legg til disse filtypene:  <br/> dotm, DOCM, XLSM, sltm, XLA, xlam, XLL, pptm, potm, PPAM, ppsm, sldm  <br/>|
|Gjør følgende. . .  <br/> |Varsle mottakeren med en melding  <br/> |
|Angi meldingstekst  <br/> |Ikke åpne denne typen filer fra personer du ikke kjenner, fordi de kan inneholde makroer med skadelig kode.  <br/> |
   
Hvis du vil ha mer informasjon, kan du se:
  
- [Hvordan håndtere ransomware](https://go.microsoft.com/fwlink/?linkid=2016501&amp;clcid=0x409)
    
- [Gjenopprette OneDrive](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)
    


## <a name="stop-auto-forwarding-for-email"></a>Stopp automatisk videresending for e-post

Hackere som får tilgang til en brukers postboks, kan stjele e-posten din ved å angi at postkassen automatisk skal videresende e-post. Dette kan skje selv uten brukerens oppmerksomhet. Du kan forhindre at dette skjer ved å konfigurere en regel for e-postflyt. 
  
Hvis du vil opprette en regel for e-post transport, kan du enten se på [denne korte videoen](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) eller følge disse trinnene:
  
1. I Administrasjonssenter for Microsoft 365, klikker du **administrasjonssentre** \> **Exchange**.
    
2. Klikk **regler**i kategorien **e-postflyt** .
    
3. Klikk **+**, og klikk deretter **Opprett en ny regel**.
    
4. Klikk **flere alternativer** nederst i dialogboksen for å se hele settet med alternativer. 
    
5. Bruk innstillingene i tabellen nedenfor. La resten av innstillingene være standard, med mindre du vil endre disse.
    
6. Klikk **Lagre**.
    
|**Innstilling**|**Advar brukere før åpning av vedlegg av Office-filer**|
|:-----|:-----|
|Navn  <br/> |Forhindre automatisk videresending av e-post til eksterne domener  <br/> |
|Bruk denne regelen hvis...  <br/> |Avsenderen. . . er ekstern/intern. . . Inne i organisasjonen  <br/> |
|Legg til betingelse  <br/> |Meldingsegenskapene. . . inkludere meldingstypen. . . Automatisk videresending  <br/> |
|Gjør følgende...  <br/> |Blokker meldingen. . . meldingen og ta med en forklaring.  <br/> |
|Angi meldingstekst  <br/> |Automatisk videresending av e-post utenfor denne organisasjonen er forhindret av sikkerhetsmessige årsaker.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Beskytt din e-post fra phishing-angrep

Hvis du har konfigurert ett eller flere egendefinerte domener for Office 365-eller Microsoft 365-miljøet ditt, kan du konfigurere målrettet beskyttelse mot phishing. ATP anti-phishing sikringen, del av kontor 365 avansert trusselen sikringen, kanne hjelpe beskytte din organisasjon fra ondsinnet etterligning-basert phishing angripe og annet phishing angripe. Hvis du ikke har konfigurert et egendefinert domene, trenger du ikke å gjøre dette.
  
Vi anbefaler at du kommer i gang med denne beskyttelsen ved å opprette en policy for å beskytte de viktigste brukerne og det egendefinerte domenet. 

  
Hvis du vil opprette en ATP anti-phishing-policy, kan du se [denne korte opplæringsvideoen](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)eller fullføre følgende trinn:
  
1. Gå til [https://protection.office.com](https://protection.office.com). 
    
2. Under **trussel behandling**i den &amp; venstre navigasjonsruten i Office 365 sikkerhet Compliance Center, velger du **policy**.
    
3. Velg **ATP anti-phishing**på **policy** -siden.
    
4. Velg **+ Opprett**på siden **anti-phishing** . En veiviser starter opp trinnene du gjennom å definere din anti-phishing-policy.
    
5. Angi navn, beskrivelse og innstillinger for policyen slik det er anbefalt i diagrammet nedenfor. Se [Lær om alternativer for ATP anti-phishing-policy](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options) for mer informasjon. 
    
6. Når du har gjennomgått innstillingene, velger du **Opprett denne policyen** eller **Lagre**, etter behov.
    

|**Innstilling eller alternativ**<br/>|**Anbefalt innstilling** <br/>|
|:-----|:-----|
|Navn  <br/> |Domene og mest verdifulle kampanje ansatte  <br/> |
|Beskrivelse  <br/> |Sikre at de fleste viktige ansatte og vårt domene ikke blir representert.  <br/> |
|Legg til brukere som skal beskyttes  <br/> |Velg **+ Legg til en betingelse, mottakeren er**. Skriv inn brukernavn eller skriv inn e-postadressen til kandidaten, kampanje administratoren og andre viktige stabsmedlemmer. Du kan legge til opptil 20 interne og eksterne adresser som du vil beskytte mot representasjon.  <br/> |
|Legg til domener for å beskytte  <br/> |Velg **+ Legg til en betingelse, mottakerdomenet er**. Angi det egendefinerte domenet som er knyttet til abonnementet på Microsoft 365, hvis du har definert et. Du kan angi mer enn ett domene.  <br/> |
|Velg handlinger  <br/> |Hvis e-post sendes av en representert bruker: Velg **Omdiriger melding til en annen e-postadresse**, og skriv deretter inn e-postadressen til sikkerhetsadministratoren. for eksempel *Alice<span><span>@contoso. com*.          Hvis e-post er sendt av et representert domene: Velg **karantene melding**.  <br/> |
|Postboks intelligens  <br/> |Som standard velges postboks intelligens når du oppretter en ny anti-phishing-policy. La denne innstillingen stå **på** for best resultat.  <br/> |
|Legge til klarerte avsendere og domener  <br/> |Her kan du legge til ditt eget domene eller andre klarerte domener.  <br/> |
|Brukt på  <br/> |Velg **mottakerdomenet er**. Velg **Velg**under **noen av disse**. Velg **+ Legg til**. Merk av i avmerkingsboksen ved siden av navnet på domenet, for eksempel *contoso.<span> com <span>*, i listen, og velg deretter **Legg til**. Velg **ferdig**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Beskytt mot skadelige vedlegg og filer med ATP safe vedlegg

De som regelmessig sender, mottar og deler vedlegg, for eksempel dokumenter, presentasjoner, regneark og mer. Det er ikke alltid lett å finne ut om et vedlegg er trygt eller skadelig bare ved å se på en e-postmelding. Den avanserte trussel beskyttelsen for Office 365 omfatter beskyttelse av ATP safe-vedlegg, men denne beskyttelsen er ikke aktivert som standard. Vi anbefaler at du oppretter en ny regel for å begynne å bruke denne beskyttelsen. Denne beskyttelsen utvides til filer i SharePoint, OneDrive og Microsoft Teams.
  
Hvis du vil opprette en policy for sikker tilkobling for ATP, kan du enten se på [denne korte videoen](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)eller fullføre følgende trinn:
  
1. Gå til [https://protection.office.com](https://protection.office.com) og Logg på med administratorkontoen din. 
    
2. Under **trussel behandling**i den &amp; venstre navigasjonsruten i Office 365 sikkerhet Compliance Center, velger du **policy**.
    
3. Velg **ATP-sikre vedlegg**på policy-siden.
    
4. På siden sikre vedlegg bruker du denne beskyttelsen bredt ved å merke av for **slå på ATP for SharePoint, OneDrive og Microsoft Teams** . 
    
5. Velg **+** for å opprette en ny policy. 
    
6. Bruk innstillingene i tabellen nedenfor. 
    
7. Når du har gjennomgått innstillingene, velger du **Opprett denne policyen** eller **Lagre**, etter behov.
    

|**Innstilling eller alternativ**|**Anbefalt innstilling** <br/>|
|:-----|:-----|
|Navn  <br/> |Blokker nåværende og fremtidige e-postmeldinger med oppdaget skadelig programvare.  <br/> |
|Beskrivelse  <br/> |Blokker nåværende og fremtidige e-poster og vedlegg med oppdaget malware.  <br/> |
|Lagre vedlegg ukjent malware respons  <br/> |Velg **blokker-blokker gjeldende og fremtidige e-poster og vedlegg med oppdaget malware**.  <br/> |
|Omadresser vedlegg ved gjenkjenning  <br/> |Aktiver omadressering (Velg denne boksen) Angi administratorkontoen eller et postboks oppsett for karantene.          Påfør over valget hvis Malware skanning for vedlegg blir tidsavbrutt eller feil oppstår (Velg denne boksen).  <br/> |
|Brukt på  <br/> |Mottakerens domene er. . . velge domenet ditt.  <br/> |
   
Hvis du vil ha mer informasjon, kan du se [konfigurere Office 365 ATP anti-phishing-policyer](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Beskytt mot phishing-angrep med ATP safe Links

Hackere skjuler noen ganger ondsinnede nettsteder i koblinger i e-post eller andre filer. Kontor 365 ATP pengeskap Golfbane (ATP pengeskap golfbane), del av kontor 365 avansert trusselen sikringen, kanne hjelpe beskytte din organisasjon av skaffer tid-av-falle i staver bekreftelse av webadresser (URLs) inne email beskjeder og kontor dokumenter. Beskyttelse defineres gjennom policyer for ATP-sikre koblinger.
  
Vi anbefaler at du gjør følgende:
  
- Endre standardpolicyen for å øke beskyttelsen.
    
- Legg til en ny policy som er rettet mot alle mottakere i domenet.
    
Hvis du vil konfigurere ATP safe Links, kan du se [denne korte opplæringsvideoen](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)eller fullføre følgende trinn:
  
1. Gå til [https://protection.office.com](https://protection.office.com) og Logg på med administratorkontoen din. 
    
2. Under **trussel behandling**i den &amp; venstre navigasjonsruten i Office 365 sikkerhet Compliance Center, velger du **policy**.
    
3. Velg **ATP-sikre koblinger**på policy-siden.
    
Slik endrer du standardpolicyen:
  
1. På siden sikre koblinger velger du **standard** policyen under **policyer som gjelder for hele organisasjonen**. 
    
2. Under **innstillinger som gjelder for innhold unntatt e-post**, velger du **Office 365 ProPlus, Office for IOS og Android**.
    
3. Klikk **Lagre**. 
    
Slik oppretter du en ny policy som er rettet mot alle mottakere i domenet:
  
1. Klikk **+** for å opprette en ny policy på siden sikre koblinger under **policyer som gjelder for hele organisasjonen**. 
    
2. Bruk innstillingene som er oppført i tabellen nedenfor.
    
3. Klikk **Lagre**. 

|**Innstilling eller alternativ**|**Anbefalt innstilling** <br/>|
|:-----|:-----|
|Navn  <br/> |Policy for sikre koblinger for alle mottakere i domenet  <br/> |
|Velg handlingen for ukjente, potensielt ondsinnede URL-adresser i meldinger  <br/> |Velge **opp på-URLs ville være omskrevet og avkrysset imot en liste over kjent ondsinnet golfbane når bruker falle i staver på koble sammen**.  <br/> |
|Bruk sikre vedlegg til å skanne nedlastbart innhold  <br/> |Merk av i denne boksen.  <br/> |
|Brukt på  <br/> |Mottakerens domene er. . . velge domenet ditt.  <br/> |
   
Hvis du vil ha mer informasjon, se [Office 365 ATP sikker koblinger](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Gå til administrasjonssenteret for Intune

1. Logg på [Azure-portalen](https://portal.azure.com/).

2. Velg **alle tjenester** og skriv inn i *Intune* i **søkeboksen**.

3. Når resultatene vises, klikker du på Start ved siden av **Microsoft Intune** for å gjøre det til en favoritt og lett å finne senere.

I tillegg til administrasjonssenteret kan du bruke Intune til å registrere og administrere organisasjonens enheter. Hvis du vil ha mer informasjon, kan du se [funksjoner etter registreringsmetode for Windows-enheter](https://docs.microsoft.com/intune/enrollment-method-capabs) og [registreringsalternativer for enheter som administreres av Intune](https://docs.microsoft.com/intune/enrollment-options).
