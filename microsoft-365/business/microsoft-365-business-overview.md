---
title: Oversikt Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 9/20/2018
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Lær hvordan du konfigurerer Microsoft 365 Business.
ms.openlocfilehash: afc39ce57e63ad039780ad33e60fa81d8e8eec7a
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/07/2019
ms.locfileid: "38031469"
---
# <a name="overview-of-microsoft-365-business"></a>Oversikt over Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>Hva er Microsoft 365 Business

Microsoft 365 Business er et omfattende sett med forretningsproduktivitet- og samarbeidsverktøy, for eksempel Outlook, Word, Excel og andre Office-produkter som alltid er oppdatert. Du kan beskytte arbeidsfiler på alle iOS-, Android- og Windows 10-enheter med sikkerhet på foretaksnivå som er enkel å administrere.
  
Microsoft 365 Business er beregnet for opptil 300 lisenser. Hvis du trenger flere lisenser, kan du se dokumentasjonen for [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) for å få mer informasjon.

Se [Microsoft 365 beskrivelse av forretnings tjeneste](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description) for hele listen over funksjoner.
  
## <a name="small-business-security-needs"></a>Sikkerhetsbehov for små bedrifter

Bedriftsdataene dine kan bli kompromittert på mange måter. Du og brukerne kan kompromittere organisasjonens sikkerhet når du logger på med kompromittert legitimasjon eller viser organisasjonsdata på forskjellige enheter og programmer. Mer spesifikt er organisasjonen i faresonen for:

1. Kompromittert eller svak påloggingslegitimasjon.
2. Kompromittert enhet med en svak PIN, eller en brukereid enhet.
3. Brukere som kan kopiere/lime inn/lagre organisasjonens data til personlige apper.
4. Brukernes hvem installere og bruk 3<sup>Rd</sup> parti apps med svak garanti.
5. Email sårbarheter inkludert deling av sensitive data, phishing-forsøk, malware, etc.
6. Når folk som ikke bør, kan få tilgang til dokumenter med sensitiv informasjon.

Microsoft 365 Business bidrar til å beskytte dataene dine i hver av disse tilfellene. Sikkerhetsfunksjonene som beskytter forretningsdataene, er beskrevet i illustrasjonen nedenfor.

![En figur som viser hvordan M365B beskytter virksomheten din.](media/m365businessvalueadd.png)

## <a name="how-your-data-and-devices-are-protected"></a>Slik beskyttes dataene og enhetene dine

Microsoft 365 Business bidrar til å **forsvare trusler** ved å:

Skanne koblinger i e-post og dokumenter i sanntid for å blokkere usikre nettsteder (ATP safe Links).

- Utføre avansert analyse av e-postvedlegg i et sandkassemiljø for å oppdage nylig utviklet skadelig programvare (ATP-sikre vedlegg). 

- Aktivering av anti-phishing-policyer som bruker maskinlæringsmodeller og gjenkjenning av representasjon for å gi beskyttelse mot avanserte angrep (ATP anti-phishing Intelligence). 

- Sette opp avanserte policyer som deaktiverer tilgang fra ikke-klarerte plasseringer eller omgå multifaktor godkjenning fra klarerte steder som kontornettverk (Azure MFA inkludert pålitelige IP-adresser og betinget tilgang). 

- Håndheve beskyttelse mot skadelig programvare på tvers av alle firmaets Windows 10-enheter og beskytte filer i viktige system mapper fra endringer som er gjort av ransomware (Windows Defender)

**Forretningsdataene dine er beskyttet** av:

- Ved hjelp av automatisk gjenkjenning for å hindre sensitiv informasjon som personnummer eller kredittkort fra lekker utenfor bedriften (hindring av tap av data). 

- Kryptere sensitive e-postmeldinger slik at du kan kommunisere sikkert med kunder eller andre personer utenfor bedriften, slik at bare den tiltenkte mottakeren kan lese meldingen (Office 365 meldingskryptering).

- Kontrollere hvem som har tilgang til firmainformasjon ved å bruke begrensninger som ikke **Kopier** og ikke **Videresend** til e-post og dokumenter (Azure Information Protection, plan 1).

- Aktivering av ubegrenset skybasert arkivering, slik at du kan beholde alle e-post fra bedriften din, inkludert postboksene til tidligere ansatte (Exchange Online arkivering).

**Enhetene dine sikres** ved å:

- Kontrollere hvilke enheter og brukere som har tilgang til Office 365-dataene dine. med alternativer for å blokkere brukere fra å logge på fra hjemme-datamaskiner, apper som ikke er godkjent, eller utenfor arbeidstiden (betinget tilgang).

- Bruk av sikkerhetspolicyer for å beskytte forretningsdata på iOS-og Android-enheter.  Du kan for eksempel kreve at brukere skal oppgi en PIN-kode eller et fingeravtrykk for å få tilgang til forretningsdata, og kryptere data på mobilenheter (app-beskyttelse for Office-Mobilapper).

- Holde forretningsdokumenter, e-post og andre data i godkjente Office-Mobilapper og hindre at ansatte lagrer disse til uautoriserte apper og plasseringer (app beskyttelse for Office Mobile Apps).

- Fjernsletting av forretningsdata fra tapte eller stjålne enheter uten å påvirke personlig informasjon (selektiv tømming av Intune).

- Bruke forenklede kontroller for å administrere policyer for alle Windows 10-PCer i firmaet, håndheve BitLocker-kryptering og automatisk installere kritiske Windows-oppdateringer (håndheve Windows Update-policyer).

Hvis du vil se den fullstendige listen over sikkerhetsfunksjoner, kan du se [sikkerhetsfunksjoner for Microsoft 365 Business](security-features.md). Når du har [konfigurert Microsoft 365 Business](set-up.md), kan du se [konfigurere avanserte sikkerhetspolicyer](set-up-advanced-security.md) for å komme i gang med sikkerhetsfunksjonene som ikke er inkludert som en del av det guidede oppsettet. Les også [topp 10 måter å sikre Office 365 og Microsoft 365 forretningsplaner](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for en god oversikt over hvordan du setter opp beskyttelse mot Cyber kriminelle og hackere.

## <a name="get-microsoft-365-business"></a>Skaff deg Microsoft 365 Business

- Hvis du har en partner, vil de få Microsoft 365 Business: [Skaff deg Microsoft 365 Business fra Microsoft Partnersenter](get-microsoft-365-business.md#get-microsoft-365-business-from-microsoft-partner-center).

- Hvis du ikke har en partner og ønsker å få Microsoft 365 Business, kan du [kjøpe den her](https://www.microsoft.com/microsoft-365/business) og følg [registrerings](sign-up.md) instruksjonene.

- Du kan også gå over til en [Microsoft store](https://www.microsoft.com/store/locations/find-a-store?icid=en-us_UF_FAS) for å både kjøpe Microsoft 365 Business og få oppsett hjelp.
