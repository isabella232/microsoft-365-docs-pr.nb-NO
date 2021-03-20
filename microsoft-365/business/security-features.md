---
title: Sikkerhets- og samsvarsfunksjoner for Microsoft 365 Business Premium
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Lær om sikkerhetsfunksjonene som følger med Microsoft 365 Business Premium for å beskytte dataene dine på PC-er, telefoner og nettbrett.
ms.openlocfilehash: 74a22b654e60e4a980e397598117bb4c435e833b
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912554"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Sikkerhets- og samsvarsfunksjoner for Microsoft 365 Business Premium

Microsoft 365 Business Premium tilbyr forenklede sikkerhetsfunksjoner for å beskytte dataene dine på PC-er, telefoner og nettbrett.
    
## <a name="microsoft-365-admin-center-security-features"></a>Sikkerhetsfunksjoner i administrasjonssenteret for Microsoft 365

Du kan administrere mange av sikkerhetsfunksjonene for Microsoft 365 Business Premium i administrasjonssenteret, noe som gir deg en forenklet måte å aktivere eller deaktivere disse funksjonene på. I administrasjonssenteret kan du gjøre følgende:
  
- [Angi innstillinger for programbehandling for Android- eller iOS-enheter](app-protection-settings-for-android-and-ios.md) . 
    
    Disse innstillingene omfatter å slette filer fra en inaktiv enhet etter en angitt periode, kryptere arbeidsfiler, kreve at brukerne angir en PIN-kode og så videre.
    
- [Angi innstillinger for programbeskyttelse for Windows 10-enheter](protection-settings-for-windows-10-devices.md) . 
    
    Disse innstillingene kan brukes på firmadata på både firmaeide eller personlig eide enheter.
    
- [Angi innstillinger for enhetsbeskyttelse for Windows 10-enheter](protection-settings-for-windows-10-pcs.md) . 
    
    Du kan aktivere [BitLocker-kryptering](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions) for å beskytte data i tilfelle en enhet blir mistet eller stjålet, og aktivere [Windows Exploit Guard](/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) for å gi avansert beskyttelse mot løsepengevirus. 
    
- [Fjerne firmadata fra enheter](remove-company-data.md)
    
    Du kan slette firmadata eksternt hvis en enhet går tapt, stjålet eller en ansatt forlater firmaet.
    
- [Tilbakestill Windows 10-enheter til fabrikkinnstillingene.](reset-devices-to-factory-settings.md) 
    
    Du kan tilbakestille alle Windows 10-enheter som har aktivert innstillinger for enhetsbeskyttelse.
    
## <a name="additional-security-features"></a>Ekstra sikkerhetsfunksjoner 

Avanserte funksjoner i Microsoft 365 Business Premium er tilgjengelige for å hjelpe deg med å beskytte bedriften mot cybertrusler og beskytte sensitiv informasjon.
  
- **[Microsoft Defender for Office 365](../security/office-365-security/office-365-atp.md)**
    
    Microsoft Defender for Office 365 bidrar til å beskytte bedriften mot avanserte phishing- og løsepengevirusangrep som er utformet for å kompromittere informasjon om ansatte eller kunder. Funksjonene omfatter:
    
  - Avansert skanning av vedlegg og AI-drevet analyse for å oppdage og forkaste farlige meldinger.
    
  - Automatiske kontroller av koblinger i e-post for å vurdere om de er en del av et phishing-forsøk. Dette holder deg trygg fra å få tilgang til usikre nettsteder.

- **[De fullstendige funksjonene til Intune i Azure-portalen](/mem/intune/fundamentals/what-is-intune)**
    
    Når du har tilgang til Administrasjonssenter for Intune i Azure-portalen, kan du konfigurere flere sikkerhetsfunksjoner, for eksempel administrasjon av MacOS-enheter, iPhone og Android-enheter, sammen med avansert enhetsbehandling for Windows, som ikke er tilgjengelig via administrasjonssenteret for Microsoft 365.
- **Samme [betinget tilgang](/azure/active-directory/conditional-access/overview) som Azure AD Premium P1-plan**


    Betinget tilgang kan bidra til å beskytte organisasjonen mot påloggingsrisiko, tilgangsforsøk fra et uventet nettverk eller nasjonalt område, tilgangsforsøk fra risikofylte enhetstyper og så videre. Policyer for betinget tilgang håndheves etter at den første godkjenningen er fullført, og den bruker signaler fra den første godkjenningshendelsen til å avgjøre om den forsøkte tilgangen skal godkjennes, avslås eller om det kreves flere bevis (for eksempel en annen form for identifikasjon).

    Funksjonene for betinget tilgang som er inkludert, er:

    - Tilgang basert på brukernavn, gruppe og rolle
    - Access [basert på en app](/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Tilgang basert på plassering](/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  bare tillate tilgang fra klarerte IP-områder eller bestemte land 
    - Krev MFA for tilgang
    - Blokkere tilgang til apper som bruker [eldre godkjenning](/azure/active-directory/conditional-access/block-legacy-authentication)
    - Krev apper for å bruke [Intune-appbeskyttelse](/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Egendefinert godkjenning, for eksempel MFA med tredjepartsleverandører, for eksempel DUO.
   
    Andre funksjoner:
    - [Selvbetjent tilbakestilling av passord](/azure/active-directory/authentication/concept-sspr-customization) for hybrid Azure AD
    
## <a name="compliance-features"></a>Samsvarsfunksjoner

Microsoft 365 Business Premium-abonnementet inneholder funksjoner som hjelper deg med å opprettholde samsvar og forskriftsmessige standarder.

- **[Oversikt over policyer for hindring av tap av data](../compliance/data-loss-prevention-policies.md)** (DLP). 
    
    Du kan konfigurere DLP til automatisk å oppdage sensitiv informasjon, for eksempel kredittkortnumre, personnumre og så videre, for å hindre utilsiktet deling utenfor firmaet.
    
- **[Exchange Online Archiving](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online Archiving-lisens gjør det enkelt å arkivere meldinger med kontinuerlig sikkerhetskopiering av data. Den lagrer alle en brukers e-postmeldinger, inkludert slettede elementer, i tilfelle de er nødvendige senere for å oppdage eller gjenopprette. I tillegg kan du bruke ulike oppbevaringspolicyer til å bevare e-postdata for rettslige sperringer, eDiscovery eller for å oppfylle samsvarskravene.
    
- **[Følsomhetsetiketter](../compliance/sensitivity-labels.md)**

   Microsoft 365 Business Premium inneholder alle funksjonene i [Azure Information Protection Plan 1.](https://go.microsoft.com/fwlink/p/?linkid=871407) Med denne planen kan  du opprette følsomhetsetiketter som lar deg kontrollere tilgang til sensitiv informasjon i e-post og dokumenter, med kontroller som «Ikke videresend» og «Ikke kopier». Du kan også klassifisere sensitiv informasjon som Konfidensielt og angi hvordan klassifisert informasjon kan deles utenfor og i bedriften. Kryptering på bedriftsnivå er enkelt å bruke på e-post og dokumenter for å holde informasjonen privat. Du kan også installere Azure Information Protection-klient tillegget for Office-apper. Hvis du vil ha mer informasjon, kan du [se Azure Information Protection unified labeling client](/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). Installer følsomhetsetikettene for **AzInfoProtection_UL.exe**.

Du kan administrere disse funksjonene i &amp; sikkerhetssamsvarssenteret og administrasjonssenteret for Intune. Over tid legges de forenklede kontrollene til i administrasjonssenteret for Microsoft 365.
  
    
## <a name="faq"></a>Vanlige spørsmål

 ### <a name="are-these-security-features-available-in-all-markets"></a>Er disse sikkerhetsfunksjonene tilgjengelige i alle markeder?
  
Ja, disse funksjonene er tilgjengelige i alle markeder der Microsoft 365 Business Premium selges.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Hvordan finner jeg senteret for &amp; sikkerhetssamsvar?
  
1. [Logg på Microsoft 365 Business Premium ved](https://portal.microsoft.com/) hjelp av administratorlegitimasjonen. 
    
2. Finn **administrasjonssentre** i det venstre navigasjonsfeltet, og utvid det. 
    
    ![Velg Administrasjonssentre i det venstre navigasjonsfeltet i administrasjonssenteret for Microsoft 365.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Velg **&amp; Sikkerhetssamsvar** for å gå til &amp; sikkerhetssamsvarssenteret.