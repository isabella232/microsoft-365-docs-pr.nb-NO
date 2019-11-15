---
title: Oversikt over Microsoft 365 Business
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
description: Finn ut mer om Microsoft 365 Business.
ms.openlocfilehash: 03e16c336a2d6d3d8ffd5875ed7419bba3c7e378
ms.sourcegitcommit: 9a057e70637dcfe06d4f729a96c02be989cf9e25
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/14/2019
ms.locfileid: "38633403"
---
# <a name="overview-of-microsoft-365-business"></a>Oversikt over Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>Hva er Microsoft 365 Business

Microsoft 365 Business er en abonnementstjeneste som inkluderer Office 365 produktivitetsverktøy pluss avanserte funksjoner som bidrar til å beskytte bedriften mot cybertrusler, beskytte dataene og administrere enheter.
  
Microsoft 365 Business er ment for opptil 300 lisenser. Hvis du trenger flere lisenser, kan du se [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) -dokumentasjonen for mer informasjon.

Se [Microsoft 365 beskrivelse av forretnings tjeneste](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description) for hele listen over funksjoner.
  
## <a name="small-business-security-needs"></a>Sikkerhetsbehov for små bedrifter

Bedriftsdataene dine kan bli kompromittert på mange måter. Du og brukerne kan kompromittere organisasjonens sikkerhet når du logger på med kompromittert legitimasjon eller viser organisasjonsdata på forskjellige enheter og programmer. Mer spesifikt er organisasjonen i faresonen for:

- Kompromittert eller svak påloggingslegitimasjon.
- Kompromittert enhet med en svak PIN, eller en brukereid enhet.
- Brukere som kan kopiere/lime inn/lagre organisasjonens data til personlige apper.
- Brukere som installerer og bruker tredjepartsapper med svak sikkerhet.
- E-post sårbarheter, inkludert deling av sensitive data, phishing-forsøk, malware, og så videre.
- Når folk som ikke bør, kan få tilgang til dokumenter med sensitiv informasjon.

Microsoft 365 Business bidrar til å beskytte dataene dine i hver av disse tilfellene. Sikkerhetsfunksjonene som beskytter forretningsdataene, er beskrevet i illustrasjonen nedenfor.

![En figur som viser hvordan M365B beskytter virksomheten din.](media/m365businessvalueadd.png)

## <a name="how-your-data-and-devices-are-protected"></a>Slik beskyttes dataene og enhetene dine

Microsoft 365 Business bidrar til å **forsvare trusler** ved å:

- Skanne koblinger i e-postmeldinger og dokumenter i sanntid for å blokkere usikre nettsteder (ATP safe Links).

- Utføre avansert analyse av e-postvedlegg i et sandkassemiljø for å oppdage nylig utviklet skadelig programvare (ATP-sikre vedlegg). 

- Aktivering av anti-phishing-policyer som bruker maskinlæringsmodeller og gjenkjenning av representasjon for å gi beskyttelse mot avanserte angrep (ATP anti-phishing Intelligence). 

- Sette opp avanserte policyer som deaktiverer tilgang fra ikke-klarerte plasseringer eller omgå multifaktor godkjenning fra klarerte steder som kontornettverk (Azure MFA inkludert pålitelige IP-adresser og betinget tilgang). 

- Håndheve beskyttelse mot skadelig programvare på tvers av alle Windows 10-enhetene i organisasjonen og beskytte filer i viktige system mapper fra endringer som er gjort av ransomware (Windows Defender)

**Forretningsdataene dine er beskyttet** av:

- Ved hjelp av automatisk gjenkjenning for å hindre sensitiv informasjon som personnummer eller kredittkort fra lekker utenfor bedriften (hindring av tap av data). 

- Kryptere sensitive e-postmeldinger slik at du kan kommunisere sikkert med kunder eller andre personer utenfor organisasjonen. Dette sikrer at bare den tiltenkte mottakeren kan lese meldingen (Office 365 meldingskryptering).

- Kontrollere hvem som har tilgang til firmainformasjon ved å bruke begrensninger som ikke **Kopier** og ikke **Videresend** til e-post og dokumenter (Azure Information Protection, plan 1).

- Aktivering av ubegrenset skybasert arkivering, slik at du kan beholde alle organisasjonens e-post, inkludert postboksene til tidligere ansatte (Exchange Online arkivering).

**Enhetene dine sikres** ved å:

- Kontrollere hvilke enheter og brukere som kan få tilgang til Office 365-dataene dine, med alternativer for å blokkere brukere fra å logge på fra hjemme-datamaskiner, ikke-godkjente apper eller utenfor arbeidstiden (betinget tilgang).

- Bruk av sikkerhetspolicyer for å beskytte forretningsdata på iOS-og Android-enheter. Du kan for eksempel kreve at brukere skal oppgi en PIN-kode eller et fingeravtrykk for å få tilgang til forretningsdata, og kryptere data på mobilenheter (app-beskyttelse for Office-Mobilapper).

- Holde forretningsdokumenter, e-post og andre data i godkjente Office-Mobilapper og hindre at ansatte lagrer disse til uautoriserte apper og plasseringer (app beskyttelse for Office Mobile Apps).

- Fjernsletting av forretningsdata fra tapte eller stjålne enheter uten å påvirke personlig informasjon (selektiv tømming av Intune).

- Bruke forenklede kontroller for å administrere policyer for alle Windows 10-PCer i firmaet, håndheve BitLocker-kryptering og automatisk installere kritiske Windows-oppdateringer (håndheve Windows Update-policyer).

Hvis du vil se den fullstendige listen over sikkerhetsfunksjoner, kan du se [sikkerhetsfunksjoner for Microsoft 365 Business](security-features.md). Når du har [konfigurert Microsoft 365 Business](set-up.md), kan du se [konfigurere avanserte sikkerhetspolicyer](set-up-advanced-security.md) for å komme i gang med sikkerhetsfunksjonene som ikke er inkludert som en del av det guidede oppsettet. Les også [topp 10 måter å sikre Office 365 og Microsoft 365 forretningsplaner](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for en god oversikt over hvordan du setter opp beskyttelse mot Cyber kriminelle og hackere.

## <a name="get-microsoft-365-business"></a>Skaff deg Microsoft 365 Business

- Hvis du har en partner, vil de få Microsoft 365 Business: [få microsoft 365 Business fra Microsoft Partner Center](get-microsoft-365-business.md#get-microsoft-365-business-from-microsoft-partner-center).

- Hvis du ikke har en partner og ønsker å få Microsoft 365 Business, kan du [kjøpe den her](https://www.microsoft.com/microsoft-365/business) og følg [registrerings](sign-up.md) instruksjonene.

- Du kan også gå over til en [Microsoft store](https://www.microsoft.com/store/locations/find-a-store?icid=en-us_UF_FAS) for å både kjøpe Microsoft 365 Business og få oppsett hjelp.
