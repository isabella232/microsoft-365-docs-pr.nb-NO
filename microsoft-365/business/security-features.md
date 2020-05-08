---
title: Microsoft 365 Business Premium-sikkerhets- og samsvarsfunksjoner
f1.keywords:
- NOCSH
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
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Finn ut mer om sikkerhetsfunksjonene som følger med Microsoft 365 Business Premium, for å beskytte dataene dine på PC-er, telefoner og nettbrett.
ms.openlocfilehash: f6aef84afc76217161dee6b68d626128e0cc15b2
ms.sourcegitcommit: 46644f9778bc70ab6d62783e0a1e60ba2eccc27f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/08/2020
ms.locfileid: "44165761"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Microsoft 365 Business Premium-sikkerhets- og samsvarsfunksjoner

Microsoft 365 Business Premium tilbyr forenklede sikkerhetsfunksjoner for å beskytte dataene dine på PC-er, telefoner og nettbrett.
    
## <a name="microsoft-365-admin-center-security-features"></a>Sikkerhetsfunksjoner for administrasjonssenteret for Microsoft 365

[![Etikett for å gi deg beskjed om at administrasjonssenteret endres. Du finner mer informasjon på aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Du kan administrere mange av sikkerhetsfunksjonene for Microsoft 365 Business Premium i administrasjonssenteret, noe som gir deg en forenklet måte å aktivere eller deaktivere disse funksjonene på. I administrasjonssenteret kan du gjøre følgende:
  
- [Angi innstillinger for programbehandling for Android- eller iOS-enheter](app-protection-settings-for-android-and-ios.md) . 
    
    Disse innstillingene inkluderer sletting av filer fra en inaktiv enhet etter en bestemt periode, kryptering av arbeidsfiler, som krever at brukere angir en PIN-kode og så videre.
    
- [Angi innstillinger for programbeskyttelse for Windows 10-enheter](protection-settings-for-windows-10-devices.md) . 
    
    Disse innstillingene kan brukes på firmadata på både bedriftseide eller personlig eide enheter.
    
- [Angi innstillinger for enhetsbeskyttelse for Windows 10-enheter](protection-settings-for-windows-10-pcs.md) . 
    
    Du kan aktivere [BitLocker-kryptering](https://go.microsoft.com/fwlink/p/?linkid=871405) for å beskytte data i tilfelle en enhet går tapt eller blir stjålet, og aktivere [Windows Exploit Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) for å gi avansert beskyttelse mot løsepengevirus. 
    
- [Fjerne firmadata fra enheter](remove-company-data.md)
    
    Du kan slette firmadata eksternt hvis en enhet går tapt, stjålet eller en ansatt forlater firmaet.
    
- [Tilbakestill Windows 10-enheter til fabrikkinnstillingene](reset-devices-to-factory-settings.md) . 
    
    Du kan tilbakestille alle Windows 10-enheter som har innstillinger for enhetsbeskyttelse brukt på dem.
    
## <a name="additional-security-features"></a>Ekstra sikkerhetsfunksjoner 

Avanserte funksjoner i Microsoft 365 Business Premium er tilgjengelige for å hjelpe deg med å beskytte bedriften mot cybertrusler og beskytte sensitiv informasjon.
  
- **[Avansert trusselbeskyttelse for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)**
    
    Avansert trusselbeskyttelse (ATP) bidrar til å beskytte bedriften mot sofistikerte phishing- og ransomware-angrep som er utformet for å kompromittere ansattes eller kundeinformasjon. Funksjoner inkluderer:
    
  - Sofistikert vedleggsskanning og AI-drevet analyse for å oppdage og forkaste farlige meldinger.
    
  - Automatiske kontroller av koblinger i e-post for å vurdere om de er en del av et phishing-skjema. Dette gjør deg trygg fra å få tilgang til usikre nettsteder.

- **[De fullstendige funksjonene til Intune i Azure-portalen](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Når du får tilgang til administrasjonssenteret for Intune i Azure-portalen, kan du konfigurere flere sikkerhetsfunksjoner, for eksempel administrasjon av MacOS-enheter, iPhone og Android-enheter, sammen med avansert enhetsadministrasjon for Windows, som ikke er tilgjengelige via administrasjonssenteret for Microsoft 365.
- **Samme [betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) som Azure AD Premium P1-plan**


    Betinget tilgang kan bidra til å beskytte organisasjonen mot påloggingsrisiko, tilgangsforsøk fra et uventet nettverk eller en nasjonal enhet, tilgangsforsøk fra risikable enhetstyper og så videre. Policyer for betinget tilgang håndheves etter at den første godkjenningen er fullført, og den bruker signaler fra den første godkjenningshendelsen til å avgjøre om tilgangsforsøket skal godkjennes, nektes eller om det kreves mer bevis (for eksempel en annen form for identifikasjon).

    De betingede tilgangsfunksjonene som er inkludert, er:

    - Tilgang basert på brukernavn, gruppe og rolle
    - Tilgang [basert på en app](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Tilgang basert på plassering;](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration)  bare gi tilgang fra klarerte IP-områder eller bestemte land 
    - Krev MFA for tilgang
    - Blokkere tilgang til apper som bruker [eldre godkjenning](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Krev apper tp bruk [Intune app beskyttelse](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Tilpasset godkjenning, for eksempel MFA med tredjepartsleverandører, for eksempel DUO.
   
    Andre funksjoner:
    - [Selvbetjent tilbakestilling av passord](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) for hybrid Azure AD
    
## <a name="compliance-features"></a>Samsvarsfunksjoner

Microsoft 365 Business Premium-abonnementet inneholder funksjoner som hjelper deg med å opprettholde samsvars- og forskriftsstandarder.

- **[Oversikt over policyer for hindring av tap](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies)** av data (DLP). 
    
    Du kan konfigurere DLP til automatisk å oppdage sensitiv informasjon, for eksempel kredittkortnumre, personnummer og så videre, for å forhindre utilsiktet deling utenfor firmaet.
    
- **[Exchange Online Archiving](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online Archiving-lisens gjør det enkelt å arkivere meldinger med kontinuerlig sikkerhetskopiering av data. Den lagrer alle en brukers e-post, inkludert slettede elementer, i tilfelle de er nødvendig senere for oppdagelse eller gjenoppretting. I tillegg kan du bruke forskjellige oppbevaringspolicyer til å beholde e-postdata for rettstvister, eDiscovery eller for å oppfylle samsvarskravene.
    
- **[Følsomhetsetiketter](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Microsoft 365 Business Premium inneholder alle funksjonene i [Azure Information Protection Plan 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Med denne planen kan du opprette **følsomhetsetiketter** som lar deg kontrollere tilgangen til sensitiv informasjon i e-post og dokumenter, med kontroller som "Ikke videresend" og "Ikke kopier." Du kan også klassifisere sensitiv informasjon som "Konfidensielt" og angi hvordan klassifisert informasjon kan deles utenfor og i virksomheten. Kryptering i bedriftsklasse er enkel å bruke på e-post og dokumenter for å holde informasjonen din privat. Du kan også installere Azure Information Protection-klienttillegget for Office-apper. Hvis du vil ha mer informasjon, kan du se [Unified Labeling-klient for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). For følsomhetsetiketter installerer du **AzInfoProtection_UL.exe**.

Du kan administrere disse &amp; funksjonene i sikkerhetssamsvarssenteret og administrasjonssenteret for Intune. Over tid legges de forenklede kontrollene til administrasjonssenteret for Microsoft 365.
  
    
## <a name="faq"></a>Vanlige spørsmål

 ### <a name="are-these-security-features-available-in-all-markets"></a>Er disse sikkerhetsfunksjonene tilgjengelige i alle markeder?
  
Ja, disse funksjonene er tilgjengelige i alle markeder der Microsoft 365 Business Premium selges.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Hvordan finner jeg &amp; sikkerhetssamsvarssenteret?
  
1. [Logg på Microsoft 365 Business Premium](https://portal.microsoft.com/) ved hjelp av administratorlegitimasjonen. 
    
2. Finn **administrasjonssentre** i venstre navigasjonsenhet og utvid den. 
    
    ![Velg Administrasjonssentre i venstre navigasjonsenhet i administrasjonssenteret for Microsoft 365.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Velg ** &amp; Sikkerhetssamsvar** for &amp; å gå til Sikkerhetssamsvarssenter.
