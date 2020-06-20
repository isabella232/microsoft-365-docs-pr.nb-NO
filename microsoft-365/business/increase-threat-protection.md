---
title: Øke trusselbeskyttelsen for Microsoft 365 for bedrifter
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
description: Konfigurer Avansert trusselbeskyttelse for Office 365 og beskytt sensitive data mot phishing, skadelig programvare og andre trusler.
ms.openlocfilehash: d5510cdc082781fd9a1776e86b1bab1d8a2723d6
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/18/2020
ms.locfileid: "44786210"
---
# <a name="increase-threat-protection"></a>Øk trusselbeskyttelsen

Denne artikkelen hjelper deg med å øke beskyttelsen i Microsoft 365-abonnementet for å beskytte mot phishing, skadelig programvare og andre trusler. Disse anbefalingene er hensiktsmessige for organisasjoner med økt behov for sikkerhet, som advokatkontorer og helseklinikker.

Før du begynner, må du kontrollere sikkert poengsum for Office 365. Sikker poengsum for Office 365 analyserer organisasjonens sikkerhet basert på vanlige aktiviteter og sikkerhetsinnstillinger, og tilordner en poengsum. Begynn med å notere deg gjeldende poengsum. Hvis du vil øke poengsummen din, fullfører du handlingene som anbefales i denne artikkelen. Målet er ikke å oppnå maksimal poengsum, men å være oppmerksom på muligheter for å beskytte miljøet ditt som ikke påvirker produktiviteten negativt for brukerne dine. 

Hvis du vil ha mer informasjon, kan du se [Microsoft Secure Score](https://docs.microsoft.com/microsoft-365/security/mtp/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Øke beskyttelsesnivået mot skadelig programvare i e-post

Office 365- eller Microsoft 365-miljøet inneholder beskyttelse mot skadelig programvare. Du kan øke denne beskyttelsen ved å blokkere vedlegg med filtyper som vanligvis brukes til skadelig programvare. Slik øker du beskyttelse mot skadelig programvare i e-post:
  
1. Gå til [https://protection.office.com](https://protection.office.com) og logg på med påloggingsinformasjonen for administratorkontoen. 
    
2. Velg &amp; **Policy** Anti-Malware under Trusselbehandling i navigasjonsruten til venstre under **Trusselbehandling**i navigasjonsruten til \> **Anti-Malware**venstre.
    
3. Dobbeltklikk standardpolicyen for å redigere denne policyen for hele firmaet.
    
4. Velg **Innstillinger**.
    
5. Velg **På**under Filter for **vanlige vedleggstyper**. Filtypene som er blokkert er oppført i vinduet rett under denne kontrollen. Kontroller at du legger til disse filtypene:
   - ade, adp, ani, bas,, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, jobb, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif  <br/> 
   
   Om nødvendig kan du legge til eller slette filtyper senere.
    
6. Velg **Lagre.**
    
Hvis du vil ha mer informasjon, kan du se [Beskyttelse mot skadelig programvare](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Beskytt mot løsepengevirus

Ransomware begrenser tilgangen til data ved å kryptere filer eller låse dataskjermer. Det forsøker deretter å presse penger fra ofre ved å be om "løsepenger", vanligvis i form av kryptokurver som Bitcoin, i bytte for tilgang til data. 
  
For å beskytte mot løsepengevirus, opprett én eller flere regler for e-postflyt for å blokkere filtyper som vanligvis brukes til løsepengevirus. (Du har lagt til disse reglene i [heve nivået av beskyttelse mot skadelig programvare i e-post](#raise-the-level-of-protection-against-malware-in-mail) trinn.) Du kan også advare brukere som mottar disse vedleggene i e-post.

I tillegg til filene du blokkerte i forrige trinn, er det lurt å opprette en regel for å advare brukere før du åpner Office-filvedlegg som inneholder makroer. Ransomware kan være skjult inne makroer, så advare brukere ikke å åpne disse filene fra folk de ikke kjenner.

Slik oppretter du en posttransportregel:
  
1. Gå til administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> , og velg **Administrasjonssentre** \> **Exchange**.
    
2. Velg **regler**i **e-postflytkategorien.**
    
3. Velg **+** , og velg deretter Opprett en ny **regel**.
    
4. Velg **Flere alternativer** nederst i dialogboksen for å se hele settet med alternativer. 
    
5. Bruk innstillingene i tabellen nedenfor for regelen. Bruk standardverdiene for resten av innstillingene, med mindre du vil endre dem.
    
6. Velg **Lagre**.
    
|**Innstilling**|**Advare brukere før du åpner vedlegg for Office-filer**||
|:-----|:-----|:-----|
|Navn  <br/> |Anti-ransomware regel: advare brukere  <br/>  |
|Bruk denne regelen hvis . . .  <br/> |Ethvert vedlegg . . . filtypen samsvarer . . .  <br/> |
|Angi ord eller uttrykk  <br/> |Legg til disse filtypene:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Gjør følgende . . .  <br/> |Varsle mottakeren med en melding  <br/> |
|Gi meldingstekst  <br/> |Ikke åpne disse filtypene fra personer du ikke kjenner fordi de kan inneholde makroer med skadelig kode.  <br/> |
   
Hvis du vil ha mer informasjon, kan du ta en titt på:
  
- [Hvordan håndtere ransomware](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [Gjenopprette OneDrive](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Stopp automatisk videresending for e-post

Hackere som får tilgang til en brukers postboks, kan stjele e-post ved å angi postboksen til å videresende e-post automatisk. Dette kan skje selv uten brukerens bevissthet. Hvis du vil hindre at dette skjer, kan du konfigurere en regel for e-postflyt. 
  
Hvis du vil opprette en regel for e-posttransport, kan du se [denne korte videoen](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) eller følge denne fremgangsmåten:
  
1. I administrasjonssenteret for Microsoft 365 velger du **Administrasjonssentre** \> **Exchange**.
    
2. Velg **regler**i **e-postflytkategorien.**
    
3. Velg **+** , og velg deretter Opprett en ny **regel**.
    
4. Hvis du vil se alle alternativene, velger du **Flere alternativer** nederst i dialogboksen. 
    
5. Bruk innstillingene i tabellen nedenfor. Bruk standardverdiene for resten av innstillingene, med mindre du vil endre dem.
    
6. Velg **Lagre**.
    
|**Innstilling**|**Advare brukere før du åpner vedlegg for Office-filer**|
|:-----|:-----|
|Navn  <br/> |Forhindre automatisk videresending av e-post til eksterne domener  <br/> |
|Bruk denne regelen hvis ...  <br/> |Avsenderen . . . er ekstern/intern . . . Inne i organisasjonen  <br/> |
|Legg til betingelse  <br/> |Meldingseskapene . . . inkludere meldingstypen . . . Automatisk fremover  <br/> |
|Gjør følgende ...  <br/> |Blokkere meldingen . . . avvise meldingen og inkludere en forklaring.  <br/> |
|Gi meldingstekst  <br/> |Automatisk videresending av e-post utenfor denne organisasjonen forhindres av sikkerhetsgrunner.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Beskytt e-posten din mot phishing-angrep

Hvis du har konfigurert ett eller flere egendefinerte domener for Office 365- eller Microsoft 365-miljøet, kan du konfigurere målrettet beskyttelse mot nettfisking. ATP-beskyttelse mot phishing, som er en del av Office 365 Advanced Threat Protection, kan bidra til å beskytte organisasjonen mot ondsinnede representasjonsbaserte phishing-angrep og andre phishing-angrep. Hvis du ikke har konfigurert et egendefinert domene, trenger du ikke å gjøre dette.
  
Vi anbefaler at du kommer i gang med denne beskyttelsen ved å opprette en policy for å beskytte de viktigste brukerne og det egendefinerte domenet. 

Hvis du vil opprette en ATP-policy mot phishing, kan du se [denne korte treningsvideoen](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)eller fullføre følgende trinn:
  
1. Gå til [https://protection.office.com](https://protection.office.com). 
    
2. Velg &amp; **Policy**under **Trusselbehandling**i navigasjonsruten til venstre i navigasjonsruten til venstre.
    
3. Velg **ATP anti-phishing på Policy-siden.** **Policy**
    
4. Velg **+ Opprett**på **siden Anti-phishing.** En veiviser starter som går deg gjennom å definere retningslinjene for anti-phishing.
    
5. Angi navn, beskrivelse og innstillinger for policyen som anbefalt i tabellen nedenfor. Hvis du vil ha mer informasjon, kan du se Finne om alternativer for [anti-phishing-policy for ATP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options) 
    
6. Når du har gjennomgått innstillingene, velger du **Opprett denne policyen** eller **Lagre**etter behov.
    

|**Innstilling eller alternativ**<br/>|**Anbefalt innstilling** <br/>|
|:-----|:-----|
|Navn  <br/> |Domene og mest verdifulle kampanjeansatte  <br/> |
|Beskrivelse  <br/> |Sørg for at de viktigste ansatte og domenet vårt ikke blir etterlignet.  <br/> |
|Legge til brukere som skal beskyttes  <br/> |Velg **+ Legg til en betingelse, Mottakeren er**. Skriv inn brukernavn eller skriv inn e-postadressen til kandidaten, kampanjelederen og andre viktige medarbeidere. Du kan legge til opptil 20 interne og eksterne adresser som du vil beskytte mot representasjon.  <br/> |
|Legge til domener som skal beskyttes  <br/> |Velg **+ Legg til en betingelse, Mottakerdomenet er**. Skriv inn det egendefinerte domenet som er knyttet til Microsoft 365-abonnementet, hvis du definerte et. Du kan angi mer enn ett domene.  <br/> |
|Velg handlinger  <br/> |Hvis e-post sendes av en bruker som ikke er representert, velger du **Omadresser melding til en annen e-postadresse**, og deretter skriver du inn e-postadressen til sikkerhetsadministratoren. for eksempel *Alice <span> <span> @contoso.com*. Hvis e-post sendes av et domene som er representert, velger du **Karantenemelding**.  <br/> |
|Postboks intelligens  <br/> |Som standard velges postboksintelligens når du oppretter en ny policy mot phishing. La denne innstillingen **stå på** for best resultat.  <br/> |
|Legge til klarerte avsendere og domener  <br/> |Her kan du legge til ditt eget domene eller andre klarerte domener.  <br/> |
|Brukes på  <br/> |Velg **Mottakerdomenet er**. Velg **under** **Alle disse**. Velg **+ Legg til**. Merk av for navnet på domenet, for eksempel *contoso. <span> <span> com*, i listen, og velg deretter **Legg til**. Velg **Ferdig**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Beskytt mot skadelige vedlegg og filer med ATP Safe Attachments

Folk sender, mottar og deler regelmessig vedlegg, for eksempel dokumenter, presentasjoner, regneark og mer. Det er ikke alltid lett å si om et vedlegg er trygt eller ondsinnet bare ved å se på en e-postmelding. Office 365 Advanced Threat Protection inkluderer ATP Sikker vedlegg beskyttelse, men denne beskyttelsen er ikke aktivert som standard. Vi anbefaler at du oppretter en ny regel for å begynne å bruke denne beskyttelsen. Denne beskyttelsen strekker seg til filer i SharePoint, OneDrive og Microsoft Teams.
  
Hvis du vil opprette en policy for sikker atp-vedlegg, kan du se [denne korte videoen](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)eller fullføre følgende trinn:
  
1. Gå til [https://protection.office.com](https://protection.office.com) , og logg på med administratorkontoen din. 
    
2. Velg &amp; **Policy**under **Trusselbehandling**i navigasjonsruten til venstre i navigasjonsruten til venstre.
    
3. Velg **ATP-sikre vedlegg på**Policy-siden.
    
4. På siden Sikre vedlegg bruker du denne beskyttelsen bredt ved å merke av **for Aktiver ATP for SharePoint, OneDrive og Microsoft Teams.** 
    
5. Velg **+** for å opprette en ny policy. 
    
6. Bruk innstillingene i tabellen nedenfor. 
    
7. Når du har gjennomgått innstillingene, velger du **Opprett denne policyen** eller **Lagre**etter behov.
    

|**Innstilling eller alternativ**|**Anbefalt innstilling** <br/>|
|:-----|:-----|
|Navn  <br/> |Blokker gjeldende og fremtidige e-postmeldinger med oppdaget skadelig programvare.  <br/> |
|Beskrivelse  <br/> |Blokker nåværende og fremtidige e-poster og vedlegg med oppdaget skadelig programvare.  <br/> |
|Lagre ukjent respons på skadelig programvare  <br/> |Velg **Blokker - Blokker gjeldende og fremtidige e-poster og vedlegg med oppdaget skadelig programvare**.  <br/> |
|Omdirigere vedlegg ved gjenkjenning  <br/> |Aktiver omadressering (velg denne boksen) Angi administratorkontoen eller et postboksoppsett for karantene.          Bruk valget ovenfor hvis malware skanning etter vedlegg tidsavsløp eller feil oppstår (velg denne boksen).  <br/> |
|Brukes på  <br/> |Mottakerdomenet er . . . velge domenet ditt.  <br/> |
   
Hvis du vil ha mer informasjon, kan du se [Konfigurere Office 365 ATP-policyer mot phishing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).
  
## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Beskytt mot phishing-angrep med ATP Safe Links

Hackere skjuler noen ganger ondsinnede nettsteder i koblinger i e-post eller andre filer. Office 365 ATP Safe Links (ATP Safe Links), en del av Office 365 Advanced Threat Protection, kan bidra til å beskytte organisasjonen ved å gi tidsavanvisning av nettadresser (URL-adresser) i e-postmeldinger og Office-dokumenter. Beskyttelse er definert gjennom ATP Safe Links policyer.
  
Vi anbefaler at du gjør følgende:
  
- Endre standardpolicyen for å øke beskyttelsen.
    
- Legg til en ny policy rettet mot alle mottakere i domenet ditt.
    
Hvis du vil konfigurere ATP Safe Links, kan du se [denne korte treningsvideoen](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)eller fullføre følgende trinn:
  
1. Gå til [https://protection.office.com](https://protection.office.com) , og logg på med administratorkontoen din. 
    
2. Velg &amp; **Policy**under **Trusselbehandling**i navigasjonsruten til venstre i navigasjonsruten til venstre.
    
3. Velg **ATP Sikre koblinger på Policy-siden.**
    
Slik endrer du standardpolicyen:
  
1. Velg **standardpolicyen** under **Policyer som gjelder for hele organisasjonen**på siden Sikre koblinger. 
    
2. Velg **Microsoft 365 Apps for enterprise, Office for iOS og Android**under Innstillinger som gjelder for innhold unntatt **e-post**.
    
3. Velg **Lagre**. 
    
Slik oppretter du en ny policy rettet mot alle mottakere i domenet:
  
1. Velg for å opprette en ny policy under **Policyer som gjelder for hele organisasjonen**på siden Sikre koblinger. **+** 
    
2. Bruk innstillingene som er oppført i tabellen nedenfor.
    
3. Velg **Lagre**. 

|**Innstilling eller alternativ**|**Anbefalt innstilling** <br/>|
|:-----|:-----|
|Navn  <br/> |Policy for sikre koblinger for alle mottakere i domenet  <br/> |
|Velg handlingen for ukjente potensielt skadelige URL-adresser i meldinger  <br/> |Velg **På - URL-adresser vil bli omskrevet og sjekket mot en liste over kjente skadelige koblinger når brukeren klikker på koblingen**.  <br/> |
|Bruk trygge vedlegg til å skanne nedlastbart innhold  <br/> |Velg denne boksen.  <br/> |
|Brukes på  <br/> |Mottakerdomenet er . . . velge domenet ditt.  <br/> |
   
Hvis du vil ha mer informasjon, kan du se [Trygge koblinger for Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Gå til administrasjonssenteret for Intune

1. Logg på [Azure-portalen](https://portal.azure.com/).

2. Velg **Alle tjenester,** og skriv inn *Intune* i **søkeboksen**.

3. Når resultatene vises, velger du starten ved siden av **Microsoft Intune** for å gjøre det til en favoritt og lett å finne senere.

I tillegg til administrasjonssenteret kan du bruke Intune til å registrere og administrere organisasjonens enheter. Hvis du vil ha mer informasjon, kan du se [Funksjoner ved registreringsmetode for Windows-enheter](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) og [registreringsalternativer for enheter som administreres av Intune](https://docs.microsoft.com/intune/enrollment-options).
