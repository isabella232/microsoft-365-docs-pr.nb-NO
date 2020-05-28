---
title: Øke trusselbeskyttelse for Microsoft 365 for bedrifter
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
description: Konfigurer Office 365 Advanced Threat Protection og beskytt sensitive data mot phishing, skadelig programvare og andre trusler.
ms.openlocfilehash: 6fa4d1595c379aaccf3a0cbfca020fbd32376fb9
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400874"
---
# <a name="increase-threat-protection"></a>Øk trusselbeskyttelsen

Denne artikkelen hjelper deg med å øke beskyttelsen i Microsoft 365-abonnementet for å beskytte mot phishing, skadelig programvare og andre trusler. Disse anbefalingene er hensiktsmessige for organisasjoner med økt behov for sikkerhet, som advokatkontorer og helsestasjoner.

Før du begynner, må du kontrollere secure score for Office 365. Sikker poengsum for Office 365 analyserer organisasjonens sikkerhet basert på regelmessige aktiviteter og sikkerhetsinnstillinger, og tilordner en poengsum. Begynn med å notere din nåværende poengsum. For å øke poengsummen din, fyll ut handlingene som anbefales i denne artikkelen. Målet er ikke å oppnå maksimal poengsum, men å være klar over muligheter til å beskytte miljøet ditt som ikke påvirker produktiviteten negativt for brukerne dine. 

Hvis du vil ha mer informasjon, kan du se [Microsoft Secure Score](https://docs.microsoft.com/microsoft-365/security/mtp/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Øk beskyttelsesnivået mot skadelig programvare i e-post

Office 365- eller Microsoft 365-miljøet inneholder beskyttelse mot skadelig programvare. Du kan øke denne beskyttelsen ved å blokkere vedlegg med filtyper som vanligvis brukes for skadelig programvare. Slik øker du beskyttelse mot skadelig programvare i e-post:
  
1. Gå til [https://protection.office.com](https://protection.office.com) og logg på med legitimasjonen for administratorkontoen. 
    
2. Velg Policy &amp; mot skadelig programvare under **Trusselbehandling**i **Policy** navigasjonsruten til venstre i sikkerhetssamsvarssenteret. \> **Anti-Malware**
    
3. Dobbeltklikk standardpolicyen for å redigere denne policyen for hele firmaet.
    
4. Velg **Innstillinger**.
    
5. Velg **På**under **Filter for vanlige vedleggstyper**. Filtyper som er blokkert, er oppført i vinduet rett under denne kontrollen. Kontroller at du legger til disse filtypene:
   - ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, jobb, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif  <br/> 
   
   Om nødvendig kan du legge til eller slette filtyper senere.
    
6. Velg **Lagre.**
    
Hvis du vil ha mer informasjon, kan du se [Beskyttelse mot skadelig programvare](https://go.microsoft.com/fwlink/?linkid=2015692&amp;clcid=0x409).
  
## <a name="protect-against-ransomware"></a>Beskytt mot løsepengevirus

Ransomware begrenser tilgangen til data ved å kryptere filer eller låse dataskjermer. Den forsøker deretter å presse penger fra ofre ved å be om "løsepenger", vanligvis i form av kryptokurver som Bitcoin, i bytte for tilgang til data. 
  
For å beskytte mot løsepengevirus, opprett ett eller flere regler for e-postflyt for å blokkere filtyper som ofte brukes for løsepengevirus. (Du har lagt til disse reglene i [å øke beskyttelsesnivået mot skadelig programvare i e-posttrinn.)](#raise-the-level-of-protection-against-malware-in-mail) Du kan også advare brukere som mottar disse vedleggene via e-post.

I tillegg til filene du blokkerte i forrige trinn, er det lurt å opprette en regel for å advare brukere før du åpner Office-filvedlegg som inneholder makroer. Ransomware kan skjules inne makroer, så advare brukerne om ikke å åpne disse filene fra folk de ikke kjenner.

Slik oppretter du en regel for e-posttransport:
  
1. Gå til administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> , og velg **Administrasjonssentre** \> **Exchange**.
    
2. Velg **regler**i **kategorien e-postflyt.**
    
3. Velg **+** , og velg deretter Opprett en ny **regel**.
    
4. Velg **Flere alternativer** nederst i dialogboksen for å se hele settet med alternativer. 
    
5. Bruk innstillingene i tabellen nedenfor for regelen. Bruk standardverdiene for resten av innstillingene, med mindre du vil endre dem.
    
6. Velg **Lagre**.
    
|**Innstilling**|**Advar brukere før du åpner vedlegg til Office-filer**||
|:-----|:-----|:-----|
|Navn  <br/> |Anti-ransomware regelen: advare brukere  <br/>  |
|Bruk denne regelen hvis . . .  <br/> |Ethvert vedlegg . . . filtypen samsvarer . . .  <br/> |
|Angi ord eller uttrykk  <br/> |Legg til disse filtypene:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm  <br/>|
|Gjør følgende . . .  <br/> |Varsle mottakeren med en melding  <br/> |
|Angi meldingstekst  <br/> |Ikke åpne disse typer filer fra personer du ikke vet fordi de kan inneholde makroer med skadelig kode.  <br/> |
   
Hvis du vil ha mer informasjon, kan du ta en titt på:
  
- [Hvordan håndtere ransomware](https://go.microsoft.com/fwlink/?linkid=2016501)
    
- [Gjenopprette OneDrive](https://support.office.com/article/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Stopp automatisk videresending for e-post

Hackere som får tilgang til en brukers postboks, kan stjele e-post ved å angi at postboksen automatisk skal videresende e-post. Dette kan skje selv uten brukerens bevissthet. Hvis du vil hindre at dette skjer, konfigurerer du en regel for e-postflyt. 
  
Hvis du vil opprette en regel for e-posttransport, kan du enten se [denne korte videoen](https://support.office.com/article/f9d693ba-5c78-47c0-b156-8e461e062aa7) eller følge denne fremgangsmåten:
  
1. Velg **Administrasjonssentre** Exchange i administrasjonssenteret for Microsoft \> **Exchange**365.
    
2. Velg **regler**i **kategorien e-postflyt.**
    
3. Velg **+** , og velg deretter Opprett en ny **regel**.
    
4. Hvis du vil se alle alternativene, velger du **Flere alternativer** nederst i dialogboksen. 
    
5. Bruk innstillingene i tabellen nedenfor. Bruk standardverdiene for resten av innstillingene, med mindre du vil endre dem.
    
6. Velg **Lagre**.
    
|**Innstilling**|**Advar brukere før du åpner vedlegg til Office-filer**|
|:-----|:-----|
|Navn  <br/> |Forhindre automatisk videresending av e-post til eksterne domener  <br/> |
|Bruk denne regelen hvis ...  <br/> |Avsenderen . . . er ekstern/intern. . . Inne i organisasjonen  <br/> |
|Legg til betingelse  <br/> |Meldingsegenskapene . . . inkludere meldingstypen . . . Automatisk fremover  <br/> |
|Gjør følgende ...  <br/> |Blokker meldingen . . . avvise meldingen og inkludere en forklaring.  <br/> |
|Angi meldingstekst  <br/> |Automatisk videresending av e-post utenfor denne organisasjonen forhindres av sikkerhetsgrunner.  <br/> |


## <a name="protect-your-email-from-phishing-attacks"></a>Beskytt e-posten mot phishing-angrep

Hvis du har konfigurert ett eller flere egendefinerte domener for Office 365- eller Microsoft 365-miljøet, kan du konfigurere målrettet beskyttelse mot nettfisking. ATP anti-phishing-beskyttelse, en del av Office 365 Advanced Threat Protection, kan bidra til å beskytte organisasjonen mot ondsinnede imitasjonsbaserte phishing-angrep og andre phishing-angrep. Hvis du ikke har konfigurert et egendefinert domene, trenger du ikke å gjøre dette.
  
Vi anbefaler at du kommer i gang med denne beskyttelsen ved å opprette en policy for å beskytte de viktigste brukerne og det egendefinerte domenet. 

Hvis du vil opprette en ATP anti-phishing-policy, kan du se [denne korte opplæringsvideoen](https://support.office.com/article/86c425e1-1686-430a-9151-f7176cce4f2c)eller fullføre følgende trinn:
  
1. Gå til [https://protection.office.com](https://protection.office.com). 
    
2. Velg Policy &amp; under **Trusselbehandling**i navigasjonsruten til venstre **Policy**i sikkerhetssamsvarssenteret.
    
3. Velg **ATP anti-phishing på Policy-siden.** **Policy**
    
4. Velg **+ Opprett** **på anti-phishing-siden.** En veiviser starter som veileder deg gjennom å definere anti-phishing-policyen.
    
5. Angi navn, beskrivelse og innstillinger for policyen som anbefalt i tabellen nedenfor. Hvis du vil ha mer informasjon, kan du se [Lære om alternativene for atp-policy er ikke-phishing-policy](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies#learn-about-atp-anti-phishing-policy-options). 
    
6. Når du har gjennomgått innstillingene, velger du **Opprett denne policyen** eller **Lagre**, etter behov.
    

|**Innstilling eller alternativ**<br/>|**Anbefalt innstilling** <br/>|
|:-----|:-----|
|Navn  <br/> |Domene og mest verdifulle kampanjemedarbeidere  <br/> |
|Beskrivelse  <br/> |Sørg for at de viktigste ansatte og vårt domene ikke blir etterlignet.  <br/> |
|Legg til brukere for å beskytte  <br/> |Velg **+ Legg til en betingelse, Mottakeren er**. Skriv inn brukernavn eller skriv inn e-postadressen til kandidaten, kampanjelederen og andre viktige medarbeidere. Du kan legge til opptil 20 interne og eksterne adresser du vil beskytte mot representasjon.  <br/> |
|Legg til domener for å beskytte  <br/> |Velg **+ Legg til en betingelse, Mottakerdomenet er**. Angi det egendefinerte domenet som er knyttet til Microsoft 365-abonnementet, hvis du definerte et. Du kan angi mer enn ett domene.  <br/> |
|Velg handlinger  <br/> |Hvis e-post sendes av en utga bruker: Velg **Omadresser melding til en annen e-postadresse**, og skriv deretter inn e-postadressen til sikkerhetsadministratoren. For eksempel *Alice <span> <span> @contoso.com*. Hvis e-post sendes av et utga domene: Velg **karantenemelding**.  <br/> |
|Postboks intelligens  <br/> |Som standard velges postboksintelligens når du oppretter en ny anti-phishing-policy. La denne innstillingen **være På** for best resultat.  <br/> |
|Legge til klarerte avsendere og domener  <br/> |Her kan du legge til ditt eget domene eller andre klarerte domener.  <br/> |
|Brukes på  <br/> |Velg **Mottakerdomenet er**. Velg **Velg**under **Noen av disse**. Velg **+ Legg til**. Merk av for navnet på domenet, for eksempel *contoso. <span> <span> com*, i listen, og velg deretter **Legg til**. Velg **Ferdig**.  <br/> |
  
## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Beskytt mot skadelige vedlegg og filer med ATP Safe Attachments

Folk sender, mottar og deler vedlegg regelmessig, for eksempel dokumenter, presentasjoner, regneark og mer. Det er ikke alltid lett å si om et vedlegg er trygt eller ondsinnet bare ved å se på en e-postmelding. Office 365 Advanced Threat Protection inkluderer ATP Safe Attachment-beskyttelse, men denne beskyttelsen er ikke aktivert som standard. Vi anbefaler at du oppretter en ny regel for å begynne å bruke denne beskyttelsen. Denne beskyttelsen strekker seg til filer i SharePoint, OneDrive og Microsoft Teams.
  
Hvis du vil opprette en ATP sikker vedleggpolicy, kan du enten se [denne korte videoen](https://support.office.com/article/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)eller fullføre følgende trinn:
  
1. Gå til [https://protection.office.com](https://protection.office.com) , og logg på med administratorkontoen din. 
    
2. Velg Policy &amp; under **Trusselbehandling**i navigasjonsruten til venstre **Policy**i sikkerhetssamsvarssenteret.
    
3. Velg **ATP-sikre vedlegg**på Policy-siden.
    
4. På siden Sikre vedlegg bruker du denne beskyttelsen bredt ved å merke av **for Aktiver ATP for SharePoint, OneDrive og Microsoft Teams.** 
    
5. Velg **+** for å opprette en ny policy. 
    
6. Bruk innstillingene i tabellen nedenfor. 
    
7. Når du har gjennomgått innstillingene, velger du **Opprett denne policyen** eller **Lagre**, etter behov.
    

|**Innstilling eller alternativ**|**Anbefalt innstilling** <br/>|
|:-----|:-----|
|Navn  <br/> |Blokker nåværende og fremtidige e-postmeldinger med oppdaget skadelig programvare.  <br/> |
|Beskrivelse  <br/> |Blokker nåværende og fremtidige e-poster og vedlegg med oppdaget skadelig programvare.  <br/> |
|Lagre ukjente vedlegg  <br/> |Velg **Blokker - Blokker gjeldende og fremtidige e-poster og vedlegg med oppdaget skadelig programvare**.  <br/> |
|Omdirigere vedlegg på gjenkjenning  <br/> |Aktiver omadressering (velg denne boksen) Skriv inn administratorkontoen eller et postboksoppsett for karantene.          Bruk utvalget ovenfor hvis skadelig programvare som skanner etter vedlegg, blir tidsriktig eller feil oppstår (velg denne boksen).  <br/> |
|Brukes på  <br/> |Mottakerdomenet er . . . velge domenet ditt.  <br/> |
   
Hvis du vil ha mer informasjon, kan du se [Konfigurere office 365 ATP anti-phishing-policyer](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).
  
## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Beskytt mot phishing-angrep med ATP Safe Links

Hackere skjuler noen ganger ondsinnede nettsteder i lenker i e-post eller andre filer. Sikker kobling til Office 365 ATP,en del av Office 365 Advanced Threat Protection, kan bidra til å beskytte organisasjonen ved å gi tidskontroll av nettadresser (URL-adresser) i e-postmeldinger og Office-dokumenter. Beskyttelse defineres gjennom ATP Safe Links-policyer.
  
Vi anbefaler at du gjør følgende:
  
- Endre standardpolicyen for å øke beskyttelsen.
    
- Legg til en ny policy som er målrettet mot alle mottakere i domenet.
    
Hvis du vil konfigurere ATP Safe Links, kan du se [denne korte opplæringsvideoen](https://support.office.com/article/61492713-53c2-47da-a6e7-fa97479e97fa)eller fullføre følgende trinn:
  
1. Gå til [https://protection.office.com](https://protection.office.com) , og logg på med administratorkontoen din. 
    
2. Velg Policy &amp; under **Trusselbehandling**i navigasjonsruten til venstre **Policy**i sikkerhetssamsvarssenteret.
    
3. Velg **ATP-sikre koblinger**på Policy-siden.
    
Slik endrer du standardpolicyen:
  
1. Velg **Standardpolicyen** under **Policyer som gjelder for hele organisasjonen**på siden Sikre koblinger. 
    
2. Velg **Microsoft 365 Apps for enterprise, Office for iOS og Android**under Innstillinger som gjelder for innhold unntatt **e-post.**
    
3. Velg **Lagre**. 
    
Slik oppretter du en ny policy som er målrettet mot alle mottakere i domenet:
  
1. Velg for å opprette en ny policy under **Policyer som gjelder for hele organisasjonen**på siden Sikre **+** koblinger. 
    
2. Bruk innstillingene som er oppført i tabellen nedenfor.
    
3. Velg **Lagre**. 

|**Innstilling eller alternativ**|**Anbefalt innstilling** <br/>|
|:-----|:-----|
|Navn  <br/> |Retningslinjer for sikker koblinger for alle mottakere i domenet  <br/> |
|Velg handlingen for ukjente potensielt skadelige nettadresser i meldinger  <br/> |Velg **På - URL-adresser vil bli omskrevet og sjekket mot en liste over kjente skadelige koblinger når brukeren klikker på linken**.  <br/> |
|Bruk Sikre vedlegg til å skanne nedlastbart innhold  <br/> |Velg denne boksen.  <br/> |
|Brukes på  <br/> |Mottakerdomenet er . . . velge domenet ditt.  <br/> |
   
Hvis du vil ha mer informasjon, kan du se Sikre koblinger for [Office 365 ATP](https://go.microsoft.com/fwlink/?linkid=2016138&amp;clcid=0x409).

## <a name="go-to-intune-admin-center"></a>Gå til Intune administrasjonssenter

1. Logg på [Azure-portalen](https://portal.azure.com/).

2. Velg **Alle tjenester,** og skriv inn *Intune* i **søkeboksen**.

3. Når resultatene vises, velger du starten ved siden av **Microsoft Intune** for å gjøre det til en favoritt og lett å finne senere.

I tillegg til administrasjonssenteret kan du bruke Intune til å registrere og administrere organisasjonens enheter. Hvis du vil ha mer informasjon, kan du se [Funksjoner ved registreringsmetode for Windows-enheter](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) og [registreringsalternativer for enheter som administreres av Intune](https://docs.microsoft.com/intune/enrollment-options).
