---
title: Øke trusselbeskyttelsen for Microsoft 365 for Bedrifter
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
description: Konfigurer Microsoft Defender for Office 365 og beskytt sensitive data mot phishing, skadelig programvare og andre trusler.
ms.openlocfilehash: 4b5142efbf4392f017cd9b96f6a9c36ef2000bb7
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245148"
---
# <a name="increase-threat-protection"></a>Øke trusselbeskyttelsen

Denne artikkelen hjelper deg med å øke beskyttelsen i Microsoft 365 for å beskytte deg mot phishing, skadelig programvare og andre trusler. Disse anbefalingene passer for organisasjoner med et økt behov for sikkerhet, for eksempel jusskontorer og helsestasjonskontorer.

Før du begynner, må du Office 365 sikker poengsum. Office 365 Sikker poengsum analyserer organisasjonens sikkerhet basert på vanlige aktiviteter og sikkerhetsinnstillinger, og tilordner en poengsum. Begynn med å notere den gjeldende poengsummen. Hvis du vil øke poengsummen, fullfører du handlingene som anbefales i denne artikkelen. Målet er ikke å oppnå maksimal poengsum, men å være oppmerksom på muligheter til å beskytte miljøet som ikke påvirker produktiviteten negativt for brukerne.

Hvis du vil ha mer informasjon, kan du se [Microsoft Secure Score](../security/defender/microsoft-secure-score.md).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Heve beskyttelsesnivået mot skadelig programvare i e-post

Miljøet Office 365 eller Microsoft 365 omfatter beskyttelse mot skadelig programvare. Du kan øke denne beskyttelsen ved å blokkere vedlegg med filtyper som vanligvis brukes for skadelig programvare. Slik øker du beskyttelse mot skadelig programvare i e-post:

1. Gå til [https://protection.office.com](https://protection.office.com) og logg på med administratorkontoens legitimasjon.

2. Velg Policy anti-malware under Trusselbehandling i navigasjonsruten til venstre i &amp; sikkerhetssamsvarsenteret.  \> 

3. Dobbeltklikk standardpolicyen for å redigere denne policyen for hele firmaet.

4. Velg **Innstillinger**.

5. Velg **På under Filter for vanlige** vedleggstyper .  Filtypene som blokkeres, vises i vinduet rett under denne kontrollen. Kontroller at du legger til disse filtypene:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   Hvis det er nødvendig, kan du legge til eller slette filtyper senere.

6. Velg **Lagre.**

Hvis du vil ha mer informasjon, kan du [se Beskyttelse mot skadelig programvare i EOP](../security/office-365-security/anti-malware-protection.md).

## <a name="protect-against-ransomware"></a>Beskytt mot løsepengevirus

Løsepengevirus begrenser tilgang til data ved å kryptere filer eller låse dataskjermer. Den forsøker deretter å utpresse penger fra ofre ved å be om løsepenger, vanligvis i form av kryptovalutaer som Bitcoin, i bytte mot tilgang til data.

Hvis du vil beskytte deg mot løsepengevirus, kan du opprette én eller flere regler for e-postflyt for å blokkere filtyper som vanligvis brukes for løsepengevirus. (Du har lagt til disse reglene i trinnet øke beskyttelsesnivået mot skadelig programvare i [e-posttrinnet.)](#raise-the-level-of-protection-against-malware-in-mail) Du kan også varsle brukere som mottar disse vedleggene via e-post.

I tillegg til filene du blokkerte i forrige trinn, er det lurt å opprette en regel for å advare brukere før du åpner Office filvedlegg som inneholder makroer. Løsepengevirus kan skjules i makroer, så advar brukerne om ikke å åpne disse filene fra personer de ikke kjenner.

Slik oppretter du en regel for e-posttransport:

1. Gå til administrasjonssenteret på <https://admin.microsoft.com> , og velg **Administrasjonssentre** \> **Exchange**.

2. Velg regler **i e-postflytkategorien.** 

3. Velg **+** , og velg deretter Opprett en ny **regel**.

4. Velg **Flere alternativer** nederst i dialogboksen for å se hele settet med alternativer.

5. Bruk innstillingene i tabellen nedenfor for regelen. Bruk standardverdiene for resten av innstillingene, med mindre du vil endre dem.

6. Velg **Lagre**.

|Innstilling|Varsle brukere før de åpner vedlegg Office filer||
|---|---|---|
|Navn|Regel for beskyttelse mot løsepengevirus: advare brukere|
|Bruk denne regelen hvis . . .|Et hvilket som helst vedlegg . . . samsvarer med filtypen . . .|
|Angi ord eller uttrykk|Legg til disse filtypene:  <br/> dotm, docm, xlsm, sltm, xla, xlam, xll, pptm, potm, ppam, ppsm, sldm|
|Gjør følgende . . .|Varsle mottakeren med en melding|
|Oppgi meldingstekst|Ikke åpne disse filtypene fra personer du ikke kjenner, fordi de kan inneholde makroer med skadelig kode.|

Hvis du vil ha mer informasjon, kan du se:

- [Løsepengevirus: slik reduserer du risikoen](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [Gjenopprette OneDrive](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Stoppe automatisk videresending for e-post

Hackere som får tilgang til en brukers postboks, kan stjele e-post ved å angi at postboksen skal videresende e-post automatisk. Dette kan skje selv uten brukerens bevissthet. Hvis du vil hindre at dette skjer, konfigurerer du en regel for e-postflyt.

Hvis du vil opprette en regel for e-posttransport, kan du [enten se denne korte videoen](../business-video/stop-email-auto-forward.md) eller følge disse trinnene:

1. Velg Microsoft 365 **administrasjonssenter** i \> **Exchange**.

2. Velg regler **i e-postflytkategorien.** 

3. Velg **+** , og velg deretter Opprett en ny **regel**.

4. Hvis du vil se alle alternativene, **velger** du Flere alternativer nederst i dialogboksen.

5. Bruk innstillingene i tabellen nedenfor. Bruk standardverdiene for resten av innstillingene, med mindre du vil endre dem.

6. Velg **Lagre**.

|Innstilling|Varsle brukere før de åpner vedlegg Office filer|
|---|---|
|Navn|Hindre automatisk videresending av e-post til eksterne domener|
|Bruk denne regelen hvis ...|Avsenderen . . . er ekstern/intern . . . I organisasjonen|
|Legg til betingelse|Meldingsegenskapene . . . inkludere meldingstypen . . . Automatisk fremover|
|Gjør følgende ...|Blokkere meldingen . . . avvis meldingen og ta med en forklaring.|
|Oppgi meldingstekst|Automatisk videresending av e-post utenfor denne organisasjonen er forhindret av sikkerhetsårsaker.|


## <a name="protect-your-email-from-phishing-attacks"></a>Beskytte e-posten mot phishing-angrep

Hvis du har konfigurert ett eller flere egendefinerte domener for Office 365- eller Microsoft 365-miljøet, kan du konfigurere målrettet beskyttelse mot phishing. Beskyttelse mot phishing, som er en del av Microsoft Defender for Office 365, kan bidra til å beskytte organisasjonen mot skadelige etterligningsbaserte phishing-angrep og andre phishing-angrep. Hvis du ikke har konfigurert et egendefinert domene, trenger du ikke å gjøre dette.

Vi anbefaler at du kommer i gang med denne beskyttelsen ved å opprette en policy for å beskytte de viktigste brukerne og det egendefinerte domenet.

Hvis du vil opprette en phishing-policy i Microsoft Defender for Office 365, kan du se denne korte [opplæringsvideoen](../business-video/setup-anti-phishing.md)eller fullføre følgende trinn:

1. Gå til [https://protection.office.com](https://protection.office.com).

2. Velg Policy under Trusselbehandling i navigasjonsruten til venstre i &amp; sikkerhetssamsvarssenteret. 

3. Velg **Anti-phishing** på **Policy-siden.**

4. Velg + **Opprett på siden Anti-phishing** **.** En veiviser starter som hjelper deg med å definere phishing-policyen.

5. Angi navnet, beskrivelsen og innstillingene for policyen som anbefalt i tabellen nedenfor. Hvis du vil ha mer informasjon, kan du se Lær [om phishing-policy i Microsoft Defender for Office 365 alternativer.](../security/office-365-security/set-up-anti-phishing-policies.md)

6. Når du har sett gjennom innstillingene, velger du **Opprett denne policyen** eller **Lagre** etter behov.

|Innstilling eller alternativ|Anbefalt innstilling|
|---|---|
|Navn|Domene og mest verdifulle kampanjepersonell|
|Beskrivelse|Sørg for at de viktigste ansatte og domenet vårt ikke blir etterlignet.|
|Legge til brukere for å beskytte|Velg **+ Legg til en betingelse, Mottakeren er**. Skriv inn brukernavn, eller skriv inn e-postadressen til kandidaten, kampanjelederen og andre viktige ansatte. Du kan legge til opptil 20 interne og eksterne adresser som du vil beskytte mot representasjon.|
|Legge til domener for å beskytte|Velg **+ Legg til en betingelse, Mottakerdomenet er**. Angi det egendefinerte domenet som er knyttet Microsoft 365 abonnementet, hvis du har definert et. Du kan angi mer enn ett domene.|
|Velg handlinger|Hvis e-post sendes av en representasjonsbruker: Velg Omadresser melding til en annen e-postadresse **,** og skriv deretter inn e-postadressen til sikkerhetsadministratoren. Eksempel: *Anne <span> <span> @contoso.com*. Hvis e-post sendes av et etterlignet domene: Velg **Karantenemelding**.|
|Postboksintelligens|Som standard velges postboksintelligens når du oppretter en ny phishing-policy. La denne innstillingen **være På** for å få best resultat.|
|Legge til klarerte avsendere og domener|Her kan du legge til ditt eget domene eller andre klarerte domener.|
|Brukt på|Velg **Mottakerdomenet er**. Velg Velg under **Hvilken som** helst av **disse**. Velg **+ Legg til**. Merk av for navnet på domenet, for eksempel *contoso. <span> <span> com* i listen, og velg deretter **Legg til**. Velg **Ferdig**.|

## <a name="protect-against-malicious-attachments-and-files-with-safe-attachments"></a>Beskytt mot skadelige vedlegg og filer med klarerte vedlegg

Personer sender, mottar og deler vedlegg regelmessig, for eksempel dokumenter, presentasjoner, regneark og mer. Det er ikke alltid enkelt å se om et vedlegg er trygt eller skadelig bare ved å se på en e-postmelding. Microsoft Defender for Office 365 inneholder beskyttelse mot sikkert vedlegg, men denne beskyttelsen er ikke aktivert som standard. Vi anbefaler at du oppretter en ny regel for å begynne å bruke denne beskyttelsen. Denne beskyttelsen gjelder for filer i SharePoint, OneDrive og Microsoft Teams.

Hvis du vil opprette en policy for sikkert vedlegg, kan du enten [se denne korte videoen](../business-video/safe-attachments.md)eller utføre følgende trinn:

1. Gå til [https://protection.office.com](https://protection.office.com) , og logg på med administratorkontoen.

2. Velg Policy under Trusselbehandling i navigasjonsruten til venstre i &amp; sikkerhetssamsvarssenteret. 

3. Velg Klarerte vedlegg på **Policy-siden.**

4. Bruk denne beskyttelsen bredt på siden Klarerte vedlegg ved å merke av **for Aktiver ATP for SharePoint, OneDrive** og Microsoft Teams.

5. Velg **+** for å opprette en ny policy.

6. Bruk innstillingene i tabellen nedenfor.

7. Når du har gått gjennom innstillingene, velger **du Opprett denne policyen** eller **Lagre** etter behov.

|Innstilling eller alternativ|Anbefalt innstilling|
|---|---|
|Navn|Blokker gjeldende og fremtidige e-postmeldinger med oppdaget skadelig programvare.|
|Beskrivelse|Blokker gjeldende og fremtidige e-postmeldinger og vedlegg med oppdaget skadelig programvare.|
|Lagre vedlegg ukjent svar på skadelig programvare|Velg **Blokker – Blokker gjeldende og fremtidige e-postmeldinger og vedlegg med oppdaget skadelig programvare.**|
|Omdiriger vedlegg ved gjenkjenning|Aktiver omadressering (velg denne boksen) Angi administratorkontoen eller et postboksoppsett for karantene.          Bruk det merkede området ovenfor hvis skanning av skadelig programvare for vedlegg blir tidsberammet eller det oppstår feil (velg denne boksen).|
|Brukt på|Mottakerdomenet er . . . velg domenet ditt.|

Hvis du vil ha mer informasjon, kan du se Konfigurere [phishing-policyer i Microsoft Defender for Office 365](../security/office-365-security/set-up-anti-phishing-policies.md).

## <a name="protect-against-phishing-attacks-with-safe-links"></a>Beskytt mot phishing-angrep med klarerte koblinger

Hackere skjuler noen ganger skadelige nettsteder i koblinger i e-post eller andre filer. Klarerte koblinger, som er en del av Microsoft Defender for Office 365, kan bidra til å beskytte organisasjonen ved å sørge for bekreftelse av nettadresser (nettadresser) i e-postmeldinger og Office dokumenter. Beskyttelse defineres gjennom policyer for klarerte koblinger.

Vi anbefaler at du gjør følgende:

- Endre standardpolicyen for å øke beskyttelsen.

- Legg til en ny policy som er rettet mot alle mottakerne i domenet.

Hvis du vil konfigurere klarerte koblinger, kan du [se denne korte opplæringsvideoen](../business-video/safe-links.md)eller fullføre følgende trinn:

1. Gå til [https://protection.office.com](https://protection.office.com) , og logg på med administratorkontoen.

2. Velg Policy under Trusselbehandling i navigasjonsruten til venstre i &amp; sikkerhetssamsvarssenteret. 

3. Velg Klarerte koblinger på **Policy-siden.**

Slik endrer du standardpolicyen:

1. Velg Standardpolicy under **Policyer som gjelder for hele** organisasjonen på siden Klarerte koblinger. 

2. Under **Innstillinger gjelder for** innhold unntatt e-post velger du **Microsoft 365 Apps for enterprise, Office for iOS og Android**.

3. Velg **Lagre**.

Slik oppretter du en ny policy som er rettet mot alle mottakerne i domenet:

1. Velg for å opprette en ny policy under **Policyer** som gjelder for hele organisasjonen på siden Klarerte **+** koblinger.

2. Bruk innstillingene som er oppført i tabellen nedenfor.

3. Velg **Lagre**.

|Innstilling eller alternativ|Anbefalt innstilling|
|---|---|
|Navn|Policy for klarerte koblinger for alle mottakere i domenet|
|Velg handlingen for ukjente potensielt skadelige nettadresser i meldinger|Velg **På – nettadresser skrives på nytt** og kontrolleres mot en liste over kjente ondsinnede koblinger når brukeren klikker koblingen .|
|Bruke klarerte vedlegg til å skanne nedlastbart innhold|Velg denne boksen.|
|Brukt på|Mottakerdomenet er . . . velg domenet ditt.|

Hvis du vil ha mer informasjon, kan du [se Klarerte koblinger](../security/office-365-security/safe-links.md).

## <a name="go-to-intune-admin-center"></a>Gå til administrasjonssenteret for Intune

1. Logg på [Azure Portal](https://portal.azure.com/).

2. Velg **Alle tjenester,** og skriv *inn Intune* i **søkeboksen**.

3. Når resultatene vises, velger du starten ved siden av Microsoft Intune **for** å gjøre det til en favoritt og enkel å finne senere.

I tillegg til administrasjonssenteret kan du bruke Intune til å registrere og administrere organisasjonens enheter. Hvis du vil ha mer informasjon, kan du se Funksjoner etter [registreringsmetode for Windows](/intune/enrollment/enrollment-method-capab) enheter og Registreringsalternativer for enheter som administreres [av Intune](/intune/enrollment-options).
