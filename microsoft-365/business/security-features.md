---
title: Microsoft 365 forretningssikkerhet og samsvarsfunksjoner
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-security-compliance
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Finn ut mer om sikkerhetsfunksjonene som følger med Microsoft 365 Business.
ms.openlocfilehash: 0d1c35192bf82ac61e59356cda4d9fb29cb3d995
ms.sourcegitcommit: 4d5e4cb3fa3ab45ad15f103c720c77277b22fc23
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/22/2019
ms.locfileid: "37636776"
---
# <a name="microsoft-365-business-security-and-compliance-features"></a>Microsoft 365 forretningssikkerhet og samsvarsfunksjoner

Microsoft 365 Business tilbyr forenklede sikkerhetsfunksjoner som bidrar til å beskytte dataene dine på PC-er, telefoner og nettbrett.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Sikkerhetsfunksjoner for Microsoft 365 Business Administrasjonssenter

[![Label å fortelle deg at Administrasjonssenteret er i endring, og du kan finne mer informasjon på aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Du kan administrere mange av Microsoft 365 sikkerhetsfunksjoner for bedrifter i administrasjonssenteret, noe som gir deg en forenklet måte å aktivere eller deaktivere disse funksjonene på. I administrasjonssenteret kan du gjøre følgende:
  
  
- [Angi innstillinger for Programbehandling for Android-eller IOS-enheter](app-protection-settings-for-android-and-ios.md) . 
    
    Disse innstillingene inkluderer sletting av filer fra en inaktiv enhet etter en angitt periode, kryptering av arbeidsfiler, som krever at brukerne angir en PIN-kode osv.
    
- [Angi innstillinger for Applikasjonsbeskyttelse for Windows 10-enheter](protection-settings-for-windows-10-devices.md) . 
    
    Disse innstillingene kan brukes på firmadata på både firma eide og personlig eide enheter.
    
- [Angi innstillinger for enhetsbeskyttelse for Windows 10-enheter](protection-settings-for-windows-10-pcs.md) . 
    
    Du kan aktivere [BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) -kryptering for å beskytte data i tilfelle en enhet mistes eller blir stjålet, og aktiverer [Windows utnyttelse Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) for å gi avansert beskyttelse mot ransomware. 
    
- [Fjerne firmadata fra enheter](remove-company-data.md)
    
    Du kan slette firmadata eksternt hvis en enhet mistes, blir stjålet eller en ansatt forlater firmaet.
    
- [Tilbakestill Windows 10-enheter til fabrikkinnstillingene](reset-devices-to-factory-settings.md) . 
    
    Du kan tilbakestille alle Windows 10-enheter som har innstillinger for enhetsbeskyttelse.
    
## <a name="additional-security-features"></a>Ekstra sikkerhetsfunksjoner 

Avanserte funksjoner i Microsoft 365 Business er tilgjengelig for å hjelpe deg med å beskytte bedriften mot Cyber-trusler og beskytte sensitiv informasjon.
  
- **[Office 365 avansert trusselbeskyttelse](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Avansert trusselbeskyttelse (ATP) bidrar til å beskytte bedriften mot avanserte phishing-og ransomware-angrep som er utformet for å kompromittere ansattes eller kundeinformasjon. Funksjoner inkluderer:
    
  - Sofistikert skanning av vedlegg og AI-drevne analyser for å oppdage og forkaste farlige meldinger.
    
  - Automatiske kontroller av koblinger i e-post for å vurdere om de er en del av en phishing-ordning. Dette holder deg trygg fra å få tilgang til usikre nettsteder.

- **[Alle funksjonene i Intune i Azure-portalen](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Hvis du åpner administrasjonssenteret for Intune i Azure-portalen, kan du konfigurere flere sikkerhetsfunksjoner, for eksempel administrasjon av MacOS-enheter, iPhone og Android-enheter sammen med avansert Enhetsbehandling for Windows, som ikke er tilgjengelige via Microsoft 365 forretnings Administrasjonssenter.
- **Samme [betingede tilgang](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/overview) som Azure ad P1-plan**

    Betinget tilgang kan bidra til å beskytte organisasjonen mot påloggings risiko, få tilgang til forsøk fra et uventet nettverk eller nasjonale innstillinger, få tilgang til forsøk på å danne risikable enhetstyper og så videre. Policyer for betinget tilgang trer i kraft etter at den første godkjenningen er fullført, og den bruker signaler fra første godkjennings hendelse til å fastslå om forsøkt tilgang skal godkjennes, benekter eller f mer bevis (for eksempel andre form for identifikasjon) er Nødvendig.

    De betingede tilgangsfunksjonene som er inkludert, er:

    - Tilgang basert på brukernavn, gruppe og rolle
    - Tilgang [basert på en app](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Tilgang basert på plassering](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  bare tillate tilgang fra klarerte IP-områder eller bestemte land 
    - Krev MFA for tilgang
    - Blokkere tilgang til apper som bruker [eldre godkjenning](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Krev apper TP Bruk [beskyttelse for Intune](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access) -apper
    - Egendefinert godkjenning som MFA med tredjepartsleverandører, for eksempel DUO.
   
    Andre funksjoner:
    - [Selv](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) betjent tilbakestilling av passord for hybrid Azure ad
    
## <a name="compliance-features"></a>Funksjoner for overholdelse

Microsoft 365 Business-abonnementet inneholder funksjoner som hjelper deg med å opprettholde samsvar og forskriftsmessige standarder.

- **[Oversikt over policyer for hindring av datatap](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    Du kan konfigurere DLP slik at sensitiv informasjon registreres automatisk, for eksempel kredittkortnumre, personnumre osv., for å hindre utilsiktet deling utenfor firmaet.
    
- **[Exchange Online Archiving](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online arkiverings lisens gjør det enkelt å arkivere meldinger med kontinuerlig sikkerhetskopiering av data. Den lagrer alle e-postadressene til en bruker, inkludert slettede elementer, i tilfelle de er nødvendige senere for oppdagelse eller gjenoppretting. I tillegg kan du bruke forskjellige oppbevaringspolicyer for å beholde e-post data for rettslig sperringer, eDiscovery eller oppfylle krav til overholdelse.
    
- **[Følsomhetsetiketter](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Microsoft 365 Business inneholder alle funksjonene i [Azure Information Protection Plan 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Med denne planen kan du opprette **følsomhet etiketter**, som lar deg kontrollere tilgang til sensitiv informasjon i e-post og dokumenter med kontroller som "ikke Videresend" og "ikke kopier." Du kan også klassifisere sensitiv informasjon som "Konfidensielt" og angi hvordan gradert informasjon kan deles utenfor og inne i bedriften. Kryptering i foretaksklasse er enkelt å bruke på e-post og dokumenter for å holde informasjonen din privat. Du kan også installere klient tillegget Azure informasjonsbeskyttelse for Office-apper. Hvis du vil ha mer informasjon, kan du se [Azure Information Protection-klient for enhetlig merking](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). For følsomhet etiketter, installere **AzInfoProtection_UL. exe**.

Du kan administrere disse funksjonene i samsvarssenteret &amp; for sikkerhet og administrasjonssenteret for Intune. Over tid vil de forenklede kontrollene bli lagt til i Microsoft 365 Business administrasjonssenteret.
  
    
## <a name="faq"></a>Vanlige spørsmål

 ### <a name="are-these-security-features-available-in-all-markets"></a>Er disse sikkerhetsfunksjonene tilgjengelige i alle markeder?
  
Ja, disse funksjonene er tilgjengelige i alle markeder der Microsoft 365 Business selges.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Hvordan finner jeg sikkerhets &amp; samsvarssenteret?
  
1. [Logg på Microsoft 365 Business](https://portal.microsoft.com/) ved hjelp av administratorlegitimasjonen. 
    
2. Inne det igjen nav, finne **admin sentre** og utfolde den. 
    
    ![Velg administrasjonssentre i det venstre navigasjonsfeltet i administrasjonssenteret for Microsoft 365.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Velg **sikkerhets &amp; overholdelse** for å gå til &amp; sikkerhets samsvarssenteret.
