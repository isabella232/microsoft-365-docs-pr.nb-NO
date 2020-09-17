---
title: Øke trussel beskyttelse for Microsoft 365 for bedrifter
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
description: Konfigurer Office 365 Advanced Threat Protection og Beskytt sensitive data mot phishing, skadelig program vare og andre trusler.
ms.openlocfilehash: d56a5371bc5fc4da22f4625024769cc0325a25ca
ms.sourcegitcommit: dffb9b72acd2e0bd286ff7e79c251e7ec6e8ecae
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/17/2020
ms.locfileid: "47948592"
---
# <a name="increase-threat-protection"></a>Øke beskyttelse mot trussel

Denne artikkelen hjelper deg med å øke beskyttelsen i Microsoft 365-abonnementet for å beskytte mot phishing, skadelig program vare og andre trusler. Disse anbefalingene er riktige for organisasjoner med økt behov for sikkerhet, for eksempel politi kontorer og helse vesen Clinics.

Før du begynner, må du kontrollere Office 365-den sikre poeng summen. Sikker poengsum i Office 365 analyserer organisasjonens sikkerhet basert på vanlige aktiviteter og sikkerhets innstillinger, og tilordner en poengsum. Begynn med å notere den gjeldende poeng summen. Hvis du vil øke poengsum, kan du fullføre handlingene som anbefales i denne artikkelen. Målet er ikke å oppnå maksimal poeng sum, men for å være klar over muligheter til å beskytte miljøet som ikke har negativ innvirkning på produktivitet for brukerne dine.

Hvis du vil ha mer informasjon, kan du se [Microsofts sikre poengsum](https://docs.microsoft.com/microsoft-365/security/mtp/microsoft-secure-score).

## <a name="raise-the-level-of-protection-against-malware-in-mail"></a>Øke beskyttelses nivået mot skadelig program vare i e-post

Office 365-eller Microsoft 365-miljøet ditt inkluderer beskyttelse mot skadelig program vare. Du kan øke denne beskyttelsen ved å blokkere vedlegg med filtyper som brukes ofte for skadelig program vare. Slik øker du beskyttelse mot skadelig program vare i e-post:

1. Gå til [https://protection.office.com](https://protection.office.com) og Logg på med legitimasjonen for administrator kontoen din.

2. &amp;Velg **policy** **Threat management** \> **anti-malware**under Threat Management i den venstre navigasjons ruten i sikkerhets samsvars senteret.

3. Dobbelt klikk standard policyen for å redigere denne policyen for hele firmaet.

4. Velg **Innstillinger**.

5. Velg **på**under **vanlige Vedleggs typer-filter**. Fil typene som blokkeres, vises i vinduet rett under denne kontrollen. Pass på at du legger til disse fil typene:

   `ade, adp, ani, bas, bat, chm, cmd, com, cpl, crt, hlp, ht, hta, inf, ins, isp, job, js, jse, lnk, mda, mdb, mde, mdz, msc, msi, msp, mst, pcd, reg, scr, sct, shs, url, vb, vbe, vbs, wsc, wsf, wsh, exe, pif`

   Hvis det er nødvendig, kan du legge til eller slette filtyper senere.

6. Velg **Lagre.**

Hvis du vil ha mer informasjon, kan du se [beskyttelse mot skadelig program vare i EoP](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-malware-protection).

## <a name="protect-against-ransomware"></a>Beskytte mot løse penge virus

Løse penge virus begrenser tilgang til data ved å kryptere filer eller låse data maskin skjermer. Den prøver deretter å extort penger fra Victims ved å spørre etter "Ransom", vanligvis i form av cryptocurrencies som Bitcoin, i Exchange for tilgang til data.

Hvis du vil beskytte mot løse penge virus, kan du opprette én eller flere regler for e-post for å blokkere filtyper som ofte brukes for løse penge virus (Du la til disse reglene i [øke beskyttelses nivået mot skadelig program vare i e-](#raise-the-level-of-protection-against-malware-in-mail) posttrinn.) Du kan også advare brukere som mottar vedleggene i e-post.

I tillegg til filene du har blokkert i forrige trinn, er det en god Fremgangs måte å opprette en regel for å advare brukere før du åpner Office-vedlegg som inneholder makroer. Løse penge virus kan skjules i makroer, så varsle brukere om ikke å åpne disse filene fra personer de ikke kjenner.

Slik oppretter du en e-posttransport regel:

1. Gå til administrasjons senteret <https://admin.microsoft.com> , og velg Exchange for **administrasjons sentre** \> **Exchange**.

2. Velg **regler**i kategorien **e-postflyt** .

3. Velg **+** , og velg deretter **Opprett en ny regel**.

4. Velg **flere alternativer** nederst i dialog boksen for å se hele settet med alternativer.

5. Bruk innstillingene i den følgende tabellen for regelen. Bruk standard verdiene for resten av innstillingene, med mindre du vil endre dem.

6. Velg **Lagre**.

|Innstilling|Advar brukere før vedlegg av Office-filer åpnes||
|---|---|---|
|Navn|Regel for anti-løse virus: Advar brukere|
|Bruk denne regelen hvis. . .|Et vedlegg. . . filtypen Sams varer. . .|
|Angi ord eller uttrykk|Legg til disse fil typene:  <br/> dotm, DOCM, XLSM, sltm, XLA, xlam, XLL, potm, PPAM, ppsm, sldm|
|Gjør følgende: . .|Varsle mottakeren med en melding|
|Gi meldings tekst|Ikke åpne disse fil typene fra personer du ikke kjenner, fordi de kan inneholde makroer med skadelig kode.|

Hvis du vil ha mer informasjon, kan du ta en titt på:

- [Løse feil: Slik reduserer du risikoen](https://www.microsoft.com/security/blog/2020/04/28/ransomware-groups-continue-to-target-healthcare-critical-services-heres-how-to-reduce-risk/)

- [Gjenopprette OneDrive](https://support.microsoft.com/office/fa231298-759d-41cf-bcd0-25ac53eb8a15.aspx)

## <a name="stop-auto-forwarding-for-email"></a>Stoppe automatisk videre sending for e-post

Hackere som får tilgang til en brukers post boks kan stjele e-post ved å sette post boksen til å vide res ende e-post automatisk. Dette kan skje selv uten en brukers tilstede status. Hvis du vil hindre at dette skjer, kan du konfigurere en regel for e-flyt.

Hvis du vil opprette en regel for e-posttransport, kan du enten se [denne korte videoen](https://support.microsoft.com/office/f9d693ba-5c78-47c0-b156-8e461e062aa7) eller følge disse trinnene:

1. Velg Exchange for **administrasjons sentre** i administrasjons senteret for Microsoft 365 \> **Exchange**.

2. Velg **regler**i kategorien **e-postflyt** .

3. Velg **+** , og velg deretter **Opprett en ny regel**.

4. Hvis du vil se alle alternativene, velger du **flere alternativer** nederst i dialog boksen.

5. Bruk innstillingene i tabellen nedenfor. Bruk standard verdiene for resten av innstillingene, med mindre du vil endre dem.

6. Velg **Lagre**.

|Innstilling|Advar brukere før vedlegg av Office-filer åpnes|
|---|---|
|Navn|Hindre automatisk videre sending av e-post til eksterne domener|
|Bruk denne regelen hvis...|Avsenderen. . . er eksternt/internt. . . I organisasjonen|
|Legg til betingelse|Meldings egenskapene. . . ta med meldings typen. . . Automatisk videre sending|
|Gjør følgende:|Blokker meldingen. . . Avvis meldingen og ta med en forklaring.|
|Gi meldings tekst|Automatisk videre sending av e-post utenfor denne organisasjonen er forhindret av sikkerhets hensyn.|


## <a name="protect-your-email-from-phishing-attacks"></a>Beskytte e-posten mot phishing-angrep

Hvis du har konfigurert ett eller flere egen definerte domener for Office 365-eller Microsoft 365-miljøet, kan du konfigurere målrettet beskyttelse mot svindel forsøk. ATP anti-phishing-beskyttelse, en del av Office 365 Advanced Threat Protection, kan bidra til å beskytte organisasjonen din mot ondsinnede angrep og andre phishing-angrep. Hvis du ikke har konfigurert et egen definert domene, trenger du ikke å gjøre dette.

Vi anbefaler at du kommer i gang med denne beskyttelsen ved å opprette en policy for å beskytte de viktigste brukerne og det egen definerte domenet.

Hvis du vil opprette en ATP-policy, kan du se  [denne korte opplærings videoen](https://support.microsoft.com/office/86c425e1-1686-430a-9151-f7176cce4f2c)eller fullføre følgende trinn:

1. Gå til [https://protection.office.com](https://protection.office.com).

2. &amp;Velg **policy**under **Threat Management**i den venstre navigasjons ruten i sikkerhets samsvars senteret.

3. Velg **ATP anti-phishing**på **policy** -siden.

4. Velg **+ Opprett**på siden **anti-phishing** . Det startes en vei viser som gjør det mulig å definere din anti-phishing-policy.

5. Angi navn, beskrivelse og innstillinger for policyen som anbefalt i tabellen nedenfor. Hvis du vil ha mer informasjon, kan du se [lære om alternativer for ATP-phishing-policy](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).

6. Når du har gått gjennom innstillingene, velger du **Opprett denne policyen** eller **Lagre**etter behov.

|Innstilling eller alternativ|Anbefalt innstilling|
|---|---|
|Navn|Domene og mest verdifulle kampanje ansatte|
|Beskrivelse|Pass på at de fleste viktige ansatte og domenet vårt ikke representeres.|
|Legge til brukere for å beskytte|Velg **+ Legg til en betingelse, mottakeren er**. Skriv inn bruker navn, eller skriv inn e-postadressen til kandidaten, kampanje sjefen og andre viktige medlemmer i ansatte. Du kan legge til opptil 20 interne og eksterne adresser du vil beskytte fra representasjon.|
|Legge til domener for å beskytte|Velg **+ Legg til en betingelse, mottaker domenet**. Skriv inn det egen definerte domenet som er knyttet til Microsoft 365-abonnementet, hvis du har definert et. Du kan angi mer enn ett domene.|
|Velg handlinger|Hvis e-post sendes av en representert bruker: Velg **Omadresser melding til en annen e-postadresse**, og skriv deretter inn e-postadressen til sikkerhets administratoren. for eksempel *anne <span> <span> @contoso. com*. Hvis e-post sendes av et representert domene: Velg **karantene melding**.|
|Post boks intelligens|Som standard velges post boks intelligens når du oppretter en ny anti-phishing-policy. La denne innstillingen være **på** for best mulig resultat.|
|Legge til klarerte avsendere og domener|Her kan du legge til ditt eget domene eller andre klarerte domener.|
|Brukt på|Velg **mottaker domenet**. Velg **Velg**under **noen av disse**. Velg **+ Legg til**. Merk av i boksen ved siden av navnet på domenet, for eksempel *contoso. <span> <span> com*, i listen, og velg deretter **Legg til**. Velg **ferdig**.|

## <a name="protect-against-malicious-attachments-and-files-with-atp-safe-attachments"></a>Beskytte mot skadelige vedlegg og filer med ATP safe vedlegg

Personer sender, mottar og deler ofte vedlegg, for eksempel dokumenter, presentasjoner, regne ark og mer. Det er ikke alltid enkelt å se om et vedlegg er sikkert eller skadelig ved å se på en e-postmelding. Office 365 Advanced Threat Protection inkluderer ATP sikker Vedleggs beskyttelse, men denne beskyttelsen er ikke aktivert som standard. Vi anbefaler at du oppretter en ny regel for å begynne å bruke denne beskyttelsen. Denne beskyttelsen utvides til filer i SharePoint, OneDrive og Microsoft Teams.

Hvis du vil opprette en policy for ATP safe-vedlegg, kan du enten se [denne korte videoen](https://support.microsoft.com/office/e7e68934-23dc-4b9c-b714-e82e27a8f8a5)eller fullføre følgende trinn:

1. Gå til [https://protection.office.com](https://protection.office.com) , og Logg på med administrator kontoen.

2. &amp;Velg **policy**under **Threat Management**i den venstre navigasjons ruten i sikkerhets samsvars senteret.

3. Velg **ATP safe vedlegg**på policy-siden.

4. På klarerte vedlegg-siden bruker du denne beskyttelsen ved å merke av for **Aktiver ATP for SharePoint, OneDrive og Microsoft Teams** .

5. Velg **+** for å opprette en ny policy.

6. Bruk innstillingene i tabellen nedenfor.

7. Når du har gått gjennom innstillingene, velger du **Opprett denne policyen** eller **Lagre**etter behov.

|Innstilling eller alternativ|Anbefalt innstilling|
|---|---|
|Navn|Blokker gjeldende og fremtidige e-postmeldinger med oppdaget skadelig program vare.|
|Beskrivelse|Blokker gjeldende og fremtidige e-postmeldinger og vedlegg med oppdaget skadelig program vare.|
|Lagre vedlegg ukjent svar på skadelig program vare|Velg **blokk – blokker gjeldende og fremtidige e-postmeldinger og vedlegg med oppdaget skadelig program vare**.|
|Omdirigere vedlegg ved gjenkjenning|Aktiver omdirigering (Velg denne boksen) Skriv inn administrator kontoen eller et post boks oppsett for karantene.          Bruk merkingen ovenfor hvis det oppstår feil søking av skadelig program vare eller feil (Velg denne boksen).|
|Brukt på|Mottaker domenet er. . . Velg domenet ditt.|

Hvis du vil ha mer informasjon, kan du se [konfigurere Office 365 ATP-policyer for anti-phishing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-anti-phishing-policies).

## <a name="protect-against-phishing-attacks-with-atp-safe-links"></a>Beskytte mot phishing-angrep med ATP safe-koblinger

Hackere skjuler noen ganger skadelige nett steder i koblinger i e-post eller andre filer. Office 365 ATP safe-koblinger (ATP safe-koblinger), en del av Office 365 Advanced Threat Protection, kan bidra til å beskytte organisasjonen ved å gi tid-til-Klikk-bekreftelse av Netta dresser (URL-adresser) i e-postmeldinger og Office-dokumenter. Beskyttelsen defineres gjennom policyer for ATP-klarerte koblinger.

Vi anbefaler at du gjør følgende:

- Endre standard policyen for å øke beskyttelsen.

- Legg til en ny policy som er rettet mot alle mottakerne i domenet ditt.

Hvis du vil konfigurere ATP safe-koblinger, kan du se [denne korte opplærings videoen](https://support.microsoft.com/office/61492713-53c2-47da-a6e7-fa97479e97fa)eller fullføre følgende trinn:

1. Gå til [https://protection.office.com](https://protection.office.com) , og Logg på med administrator kontoen.

2. &amp;Velg **policy**under **Threat Management**i den venstre navigasjons ruten i sikkerhets samsvars senteret.

3. Velg **ATP safe-koblinger**på policy-siden.

Slik endrer du standard policyen:

1. På siden sikre koblinger, under **policyer som gjelder for hele organisasjonen**, velger du **standard** policyen.

2. Velg **Microsoft 365-apper for Enterprise, Office for IOS og Android**under **innstillinger som gjelder for innhold bortsett fra e-post**.

3. Velg **Lagre**.

Slik oppretter du en ny policy som er rettet mot alle mottakerne i domenet:

1. På siden sikre koblinger, under **policyer som gjelder for hele organisasjonen**, velger **+** du for å opprette en ny policy.

2. Bruk innstillingene som er oppført i tabellen nedenfor.

3. Velg **Lagre**.

|Innstilling eller alternativ|Anbefalt innstilling|
|---|---|
|Navn|Policy for klarerte koblinger for alle mottakere i domenet|
|Velg handlingen for ukjente potensielt skadelige URL-adresser i meldinger|Velg **på-URL-adresser blir skrevet på nytt og kontrollert mot en liste over kjente skadelige koblinger når brukeren klikker koblingen**.|
|Bruke sikre vedlegg til å skanne nedlastbare innhold|Merk av for dette alternativet.|
|Brukt på|Mottaker domenet er. . . Velg domenet ditt.|

Hvis du vil ha mer informasjon, kan du se [Office 365 ATP-klarerte koblinger](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links).

## <a name="go-to-intune-admin-center"></a>Gå til administrasjons senter for Intune

1. Logg på [Azure-portalen](https://portal.azure.com/).

2. Velg **alle tjenester** , og skriv inn i *Intune* i **søke boksen**.

3. Når resultatene vises, velger du Start ved siden av **Microsoft Intune** for å gjøre det til en favoritt og enkelt å finne igjen senere.

I tillegg til administrasjons senteret kan du bruke Intune til å registrere og administrere organisasjonens enheter. Hvis du vil ha mer informasjon, kan du se [funksjoner etter registrerings metode for Windows-enheter](https://docs.microsoft.com/intune/enrollment/enrollment-method-capab) og [registrerings alternativer for enheter som administreres av Intune](https://docs.microsoft.com/intune/enrollment-options).
