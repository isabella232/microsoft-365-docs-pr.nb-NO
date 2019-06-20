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
ms.openlocfilehash: b6e9941eee9de4f295b0f8056c1c91b7076e530c
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086357"
---
# <a name="increase-threat-protection"></a>Øke trusselen beskyttelse

Denne artikkelen hjelper deg med å øke beskyttelsen i Microsoft 365-abonnementet til å beskytte deg mot phishing, malware og andre trusler. Disse anbefalingene er passende for organisasjoner med et økt behov for sikkerhet, som loven kontorer og health care øvelsene.

Før du begynner, kan du se Office 365 sikre poengsummen. Office 365 sikre poengsum analyserer organisasjonens Office 365-sikkerhet som er basert på vanlige aktiviteter og sikkerhetsinnstillinger og tilordner en poengsum. Begynn med å ta ned gjeldende poengsummen. Å utføre handlinger som er anbefalt i denne artikkelen, øker poengsummen. Målet er ikke å oppnå maksimal poengsum, men å være oppmerksom på muligheter til å beskytte miljøet som ikke negativt påvirke produktiviteten for brukerne. 

Hvis du vil ha mer informasjon, kan du se [Microsoft Secure poengsum](https://docs.microsoft.com/en-us/office365/securitycompliance/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Senke nivået for beskyttelse mot skadelig programvare i e-post

Office 365- eller Microsoft 365 miljøet omfatter beskyttelse mot skadelig programvare, men du kan øke denne beskyttelsen ved å blokkere vedlegg med filtyper som ofte brukes for skadelig programvare. Å øke beskyttelse mot skadelig programvare i e-post:
  
1. Gå til [https://protection.office.com](https://protection.office.com) og logge på med påloggingsinformasjonen for admin-kontoen. 
    
2. I Office 365-sikkerhet &amp; samsvar Center, i den venstre navigasjonsruten under **Threat management**, velger du **policyen** \> **Beskyttelse mot skadelig programvare**.
    
3. Dobbeltklikk standardpolicyen for å redigere denne policyen for firmaet.
    
4. Klikk **Innstillinger**.
    
5. Velg **på**under **Vanlige typer Filter for vedlegg**. Filtyper som blokkeres er oppført i vinduet rett under denne kontrollen.  Kontroller at du legger til disse filetypes:
   - ADE-fil, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, moduler, Internett-leverandøren, jobb, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, URL-adressen, vb, vbe, vbs, wsc, wsf, wsh, exe, PIF-filen  <br/> Du kan legge til eller slette filtyper senere om nødvendig.
    
6. Klikk **Lagre.**
    
Hvis du vil ha mer informasjon, kan du se [beskyttelse mot skadelig programvare](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Beskytte mot ransomware

Ransomware begrenser tilgangen til dataene ved å kryptere filer eller låse dataskjermer. Deretter forsøker å extort penger fra ofre ved å be om "ransom", vanligvis i form av cryptocurrencies som Bitcoin, i bytte mot tilgang til data. 
  
Du kan beskytte mot ransomware ved å opprette én eller flere e-post flyt regler til å blokkere filtyper som ofte brukes for ransomware (disse ble lagt til i trinn [senke nivået for beskyttelse mot skadelig programvare i e-post](#raise-the-level-of-protection-against-malware-in-mail) ), eller å advare brukere som mottar disse vedlegg i e-post.

I tillegg til filene som du har blokkert i forrige trinn, er det også lurt å opprette en regel for å advare brukere før du åpner Office-filvedlegg som inneholder makroer. Ransomware kan skjules i makroer, så vil vi varsle brukere kan ikke åpne disse filene fra personer de ikke kjenner.

Slik oppretter du en regel for transport av e-post:
  
1. Gå til administrasjonssenteret ved <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> , og velg **centers Admin** \> **Exchange**.
    
2. Klikk **regler**i kategorien **e-postflyt** .
    
3. Klikk **+**, og klikk deretter **Opprett en ny regel**.
    
4. Klikk **flere alternativer** nederst i dialogboksen for å se det fullstendige settet med alternativer. 
    
5. Bruk innstillingene i følgende tabell for regelen. La resten av innstillingene på standard, med mindre du vil endre disse.
    
6. Klikk **Lagre**.
    
|**Innstilling**|**Advare brukere før du åpner vedleggene i Office-filer**||
|:-----|:-----|:-----|
|Navn  <br/> |Anti-ransomware regel: advare brukere  <br/>  |
|Bruk denne regelen om. . .  <br/> |Alle vedlegg. . . samsvarer med filtypen. . .  <br/> |
|Angi et ord eller uttrykk  <br/> |Legg til disse filtypene:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Gjør følgende: . .  <br/> |Varsle mottakeren en melding  <br/> |
|Angi meldingsteksten  <br/> |Ikke åpne denne typen filer fra personer du ikke kjenner fordi de kan inneholde makroer med skadelig kode.  <br/> |
   
Hvis du vil ha mer informasjon, kan du se:
  
- [Hvordan du håndterer ransomware](https://go.microsoft.com/fwlink/?linkid=2016501&amp;clcid=0x409)
    
- [Gjenopprette din OneDrive](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)
    


## <a name="stop-auto-forwarding-for-email"></a>Stopp automatisk videresending, en funksjon for e-post

Hackere som får tilgang til en brukers postboks kan stjele e-post ved å angi postboksen automatisk videresende e-post. Dette kan skje selv uten brukerens awareness. Du kan forhindre at dette skjer ved å konfigurere en e-post flyt regel. 
  
Hvis du vil opprette en regel for transport av e-post, se på [Denne korte videoen](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) , eller du følger du denne fremgangsmåten:
  
1. Velg **Admin centers** i administrasjonssenteret for Microsoft 365 \> **Exchange**.
    
2. Klikk **regler**i kategorien **e-postflyt** .
    
3. Klikk **+**, og klikk deretter **Opprett en ny regel**.
    
4. Klikk **flere alternativer** nederst i dialogboksen for å se det fullstendige settet med alternativer. 
    
5. Bruk innstillingene i følgende tabell. La resten av innstillingene på standard, med mindre du vil endre disse.
    
6. Klikk **Lagre**.
    
|**Innstilling**|**Advare brukere før du åpner vedleggene i Office-filer**|
|:-----|:-----|
|Navn  <br/> |Forhindre automatisk videresending av e-post til eksterne domener  <br/> |
|Bruk denne regelen Hvis...  <br/> |Avsenderen. . . er ekstern/intern. . . Innenfor organisasjonen  <br/> |
|Legg til betingelse  <br/> |Meldingsegenskapene. . . Inkluder meldingstypen. . . Automatisk videresending  <br/> |
|Gjør følgende...  <br/> |Blokkere meldingen. . . forkaster du meldingen, og inkluderer en forklaring.  <br/> |
|Angi meldingsteksten  <br/> |Automatisk videresende e-post utenfor denne organisasjonen er hindret av sikkerhetsgrunner.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Beskytt din e-post fra phishing-angrep

Hvis du har konfigurert en eller flere egendefinerte domener for Office 365- eller Microsoft 365-miljø, kan du konfigurere målrettede anti-phishing-beskyttelse. ATP anti-phishing-beskyttelse, en del av Office 365 Avansert Threat Protection, kan hjelpe deg med å beskytte organisasjonen mot skadelig representasjon-baserte phishing-angrep og andre phishing-angrep. Hvis du ikke har angitt et egendefinert domene, trenger du ikke å gjøre dette.
  
Vi anbefaler at du i gang med denne typen beskyttelse ved å opprette en policy for å beskytte de viktigste brukerne og det tilpassede domenet. 

  
Hvis du vil opprette en ATP anti-phishing-policy, se på [Denne korte videoen opplæringen](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c), eller Bruk følgende fremgangsmåte:
  
1. Gå til [https://protection.office.com](https://protection.office.com). 
    
2. I Office 365-sikkerhet &amp; samsvar Center, i den venstre navigasjonsruten under **Threat management**, velger du **policyen**.
    
3. Velg **ATP anti-phishing**på **Policy** -siden.
    
4. Velg **+ Opprett**på siden **Anti-phishing** . En veiviser startes som går du gjennom definerer anti-phishing-policy.
    
5. Angi navn, beskrivelse og innstillinger for policyen som anbefalt i diagrammet nedenfor. Se [Lær om ATP anti-phishing policyalternativer](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409) for flere detaljer. 
    
6. Etter at du har gått gjennom innstillingene, velger du **Opprett denne policyen** eller **Lagre**, etter behov.
    

|**Innstillingen eller alternativet**<br/>|**Anbefalt innstilling** <br/>|
|:-----|:-----|
|Navn  <br/> |Domene og mest verdifulle kampanjen stab  <br/> |
|Beskrivelse  <br/> |Kontroller de viktigste stab og vårt domene er som imiteres.  <br/> |
|Legge til brukere for å beskytte  <br/> |Velg **Legg til en betingelse, mottakeren er +**. Skriv inn brukernavn, eller Skriv inn e-postadressen til kandidaten kampanje manager og andre viktige personalet. Du kan legge til opptil 20 interne og eksterne adressene du vil beskytte mot representasjon.  <br/> |
|Legge til domener til å beskytte  <br/> |Velg **Legg til en betingelse, mottaker domenet er +**. Angi det egendefinerte domenet som er tilknyttet abonnementet på Microsoft 365 hvis du har definert en. Du kan angi mer enn ett domene.  <br/> |
|Velg Handlinger  <br/> |Hvis e-post som er sendt av en representert bruker: Velg **omdirigere meldinger til en annen e-postadresse**, og skriv deretter inn e-postadressen til administratoren sikkerhet; for eksempel *Anne<span><span>@contoso.com*.          Hvis e-post som er sendt av en representert domene: Velg **karantene melding**.  <br/> |
|Postboks intelligence  <br/> |Postboks intelligence velges som standard når du oppretter en ny policy for anti-phishing. La denne innstillingen **på** de beste resultatene.  <br/> |
|Legge til klarerte avsendere og domener  <br/> |Her kan du legge til ditt eget domene eller andre klarerte domener.  <br/> |
|Brukes til å  <br/> |Velg **mottakerens domene er**. Under **noen av disse**, velger du **Velg**. Velg **+ Legg til**. Merk av for navnet på domenet, for eksempel *contoso.<span> <span>com*, i listen, og velg deretter **Legg til**. Velg **fullført**.  <br/> |
   
Hvis du vil ha mer informasjon, kan du se [definere policyer for Office 365 ATP anti-phishing](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Beskyttelse mot skadelige vedlegg og filer med sikker ATP-vedlegg

Personer regelmessig sende, motta og dele vedlegg, for eksempel dokumenter, presentasjoner, regneark og mer. Det er ikke alltid lett å finne ut om et vedlegg er trygt eller skadelig bare ved å se på en e-postmelding. Office 365 Avansert Threat Protection inkluderer ATP trygt vedlegg beskyttelse, men denne typen beskyttelse er ikke aktivert som standard. Vi anbefaler at du oppretter en ny regel for å begynne å bruke denne beskyttelsen. Denne beskyttelsen gjelder filer i SharePoint, OneDrive og Teams for Microsoft.
  
Hvis du vil opprette en sikker vedlegg ATP-policy, se [Denne korte videoen](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)eller fullføre følgende trinn:
  
1. Gå til [https://protection.office.com](https://protection.office.com) og logge på med admin-kontoen din. 
    
2. I Office 365-sikkerhet &amp; samsvar Center, i den venstre navigasjonsruten under **Threat management**, velger du **policyen**.
    
3. Velg **ATP trygt vedlegg**på Policy-siden.
    
4. Bruke denne beskyttelsen reparasjoner på siden Klarerte vedlegg ved å merke av for **Slå på ATP-Antallet for SharePoint, OneDrive, og Microsoft Team** . 
    
5. Velg **+** til å opprette en ny policy. 
    
6. Bruk innstillingene i følgende tabell. 
    
7. Etter at du har gått gjennom innstillingene, velger du **Opprett denne policyen** eller **Lagre**, etter behov.
    

|**Innstillingen eller alternativet**|**Anbefalt innstilling** <br/>|
|:-----|:-----|
|Navn  <br/> |Blokker gjeldende og fremtidige e-postmeldinger med oppdaget skadelig programvare.  <br/> |
|Beskrivelse  <br/> |Blokkere gjeldende og fremtidige e-postmeldinger og vedlegg med oppdaget skadelig programvare.  <br/> |
|Lagre vedlegg ukjent malware svar  <br/> |Velg **blokk - blokkerer gjeldende og fremtidige e-postmeldinger og vedlegg med oppdaget skadelig programvare**.  <br/> |
|Omadressere vedlegg på gjenkjenning  <br/> |Aktiverer omadressering (Merk dette) angir du kontoen administrator eller en Postboksoppsett for karantene.          Hvis skadelig programvare skanner etter vedlegg blir tidsavbrutt, eller det oppstår feil, bruker du valget ovenfor (Merk dette).  <br/> |
|Brukes til å  <br/> |Mottakerens domene er. . . Velg domenet ditt.  <br/> |
   
Hvis du vil ha mer informasjon, kan du se [definere policyer for Office 365 ATP anti-phishing](https://go.microsoft.com/fwlink/?linkid=2016505&amp;clcid=0x409).
  


## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Beskytte deg mot phishing-angrep med sikker ATP-koblinger

Hackere skjule noen ganger skadelige webområder i koblinger i e-post eller andre filer. Office 365 ATP sikre koblinger (ATP sikre koblinger), en del av Office 365 Avansert Threat Protection, kan beskytte organisasjonen ved å gi tid for Klikk verifisering av webadressene (URL-adressene) i e-postmeldinger og Office-dokumenter. Beskyttelse er definert gjennom sikre koblinger i ATP-policyer.
  
Vi anbefaler at du gjør følgende:
  
- Endre standardpolicyen for å øke beskyttelsen.
    
- Legge til en ny policy som er rettet mot alle mottakere i domenet.
    
Hvis du vil sikre ATP-koblinger, se på [Denne korte videoen opplæringen](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa), eller Bruk følgende fremgangsmåte:
  
1. Gå til [https://protection.office.com](https://protection.office.com) og logge på med admin-kontoen din. 
    
2. I Office 365-sikkerhet &amp; samsvar Center, i den venstre navigasjonsruten under **Threat management**, velger du **policyen**.
    
3. Velg **ATP sikre koblinger**på Policy-siden.
    
Slik endrer du standardpolicy:
  
1. På siden Klarerte koblinger under **policyer som gjelder for hele organisasjonen**, kan du velge **standard** -policyen. 
    
2. Under **innstillinger som gjelder for innhold, bortsett fra e-post**, velger du **Office 365 ProPlus, Office for iOS og Android**.
    
3. Klikk **Lagre**. 
    
Slik oppretter du en ny policy som er rettet mot alle mottakere i domenet:
  
1. På siden Klarerte koblinger under **policyer som gjelder for hele organisasjonen**, klikker du **+** til å opprette en ny policy. 
    
2. Bruke innstillingene som er oppført i følgende tabell.
    
3. Klikk **Lagre**. 

|**Innstillingen eller alternativet**|**Anbefalt innstilling** <br/>|
|:-----|:-----|
|Navn  <br/> |Sikre koblinger policy for alle mottakere i domenet  <br/> |
|Velg handlingen for ukjent potensielt skadelig URL-adresser i meldinger  <br/> |Velg **på - URL-adresser skal være skrevet på nytt og kontrollert mot en liste over kjente skadelige koblinger når brukeren klikker på koblingen**.  <br/> |
|Bruk sikker vedlegg til å skanne nedlastbart innhold  <br/> |Merk av for.  <br/> |
|Brukes til å  <br/> |Mottakerens domene er. . . Velg domenet ditt.  <br/> |
   
Hvis du vil ha mer informasjon, kan du se [Office 365 ATP sikre koblinger](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Gå til administrasjonssenteret Intune

1. Logge på [Azure portal](https://portal.azure.com/).

2. Velg **alle tjenester** og type i *Intune* i **Søk-boksen**.

3. Når resultatet vises, klikker du start neste til **Microsoft Intune** å gjøre den til favoritt og lett å finne senere.

I tillegg til administrasjonssenteret, kan du bruke Intune til å registrere og administrere organisasjonens enheter. Hvis du vil ha mer informasjon, kan du se [Egenskaper av registrerings-metoden for Windows-enheter](https://docs.microsoft.com/intune/enrollment-method-capabs) og [Alternativer for registrering for enheter som styres av Intune](https://docs.microsoft.com/intune/enrollment-options).
