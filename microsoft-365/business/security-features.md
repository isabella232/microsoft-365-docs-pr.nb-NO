---
title: Microsoft 365 Business Premium-funksjoner for sikkerhet og samsvar
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
description: Lær om sikkerhets funksjonene som følger med Microsoft 365 Business Premium, for å beskytte dataene på PC-er, telefoner og nett brett.
ms.openlocfilehash: b7fdd3d7fa25c23ee49ae82aa037588d8fba61a1
ms.sourcegitcommit: 83a40facd66e14343ad3ab72591cab9c41ce6ac0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/13/2021
ms.locfileid: "49840393"
---
# <a name="microsoft-365-business-premium-security-and-compliance-features"></a>Microsoft 365 Business Premium-funksjoner for sikkerhet og samsvar

Microsoft 365 Business Premium tilbyr forenklet sikkerhets funksjoner for å beskytte dataene dine på PC-er, telefoner og nett brett.
    
## <a name="microsoft-365-admin-center-security-features"></a>Sikkerhets funksjoner i administrasjons senteret for Microsoft 365

Du kan administrere mange av sikkerhets funksjonene i Microsoft 365 Business Premium i administrasjons senteret, noe som gir deg en enkel måte å aktivere eller deaktivere disse funksjonene på. I administrasjons senteret kan du gjøre følgende:
  
- [Angi innstillinger for program behandling for Android-eller IOS-enheter](app-protection-settings-for-android-and-ios.md) . 
    
    Disse innstillingene omfatter sletting av filer fra en inaktiv enhet etter en angitt periode, kryptering av arbeids filer, som krever at brukere angir en PIN-kode og så videre.
    
- [Angi innstillinger for program beskyttelse for Windows 10-enheter](protection-settings-for-windows-10-devices.md) . 
    
    Disse innstillingene kan brukes på firma data på både firmaeide eller andre eide enheter.
    
- [Angi innstillinger for enhets beskyttelse for Windows 10-enheter](protection-settings-for-windows-10-pcs.md) . 
    
    Du kan aktivere [BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) -kryptering for å beskytte data i tilfelle en enhet mistes eller blir stjålet, og aktivere [Windows Exploit Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/enable-exploit-protection) for å gi avansert beskyttelse mot løse penge virus. 
    
- [Fjerne firmadata fra enheter](remove-company-data.md)
    
    Du kan slette firma data eksternt hvis en enhet går tapt, blir stjålet eller en ansatt forlater firmaet ditt.
    
- [Tilbakestill Windows 10-enheter til fabrikk innstillingene](reset-devices-to-factory-settings.md) . 
    
    Du kan tilbakestille alle Windows 10-enheter som har innstillingene for enhets beskyttelse brukt på dem.
    
## <a name="additional-security-features"></a>Ekstra sikkerhetsfunksjoner 

Avanserte funksjoner i Microsoft 365 Business Premium er tilgjengelig for å hjelpe deg med å beskytte virksomheten din mot kyberterrorisme-trusler og beskytte sensitive opplysninger.
  
- **[Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)**
    
    Microsoft Defender for Office 365 bidrar til å beskytte virksomheten mot avanserte phishing-og løse penge angrep som er utformet for å gi informasjon om ansatte eller kunder. Funksjonene omfatter:
    
  - Avansert Vedleggs skanning og AI-drevet analyse for å oppdage og forkaste farlige meldinger.
    
  - Automatisk kontroll av koblinger i e-post for å vurdere om de er en del av et phishing-oppsett. Dette hindrer deg trygg på å få tilgang til usikre nett steder.

- **[Alle funksjonene i Intune i Azure-portalen](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Hvis du har tilgang til administrasjons senteret for Intune i Azure-portalen, kan du konfigurere flere sikkerhets funksjoner, for eksempel administrasjon av MacOS-enheter, iPhone og Android-enheter, sammen med avansert enhets behandling for Windows, som ikke er tilgjengelige via administrasjons senteret for Microsoft 365.
- **Samme [betingede tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) som Azure ad Premium P1-abonnement**


    Betinget tilgang kan bidra til å beskytte organisasjonen mot påloggings risiko, Access prøver fra et uventet nettverk eller en nasjonal innstilling, Access forsøker fra risikabelde enhets typer og så videre. Policyer for betinget tilgang håndheves etter at den første godkjenningen er fullført, og den bruker signaler fra den første godkjennings hendelsen til å avgjøre om den forsøkte tilgangen skal godkjennes, nektes eller om mer bevis (for eksempel en annen type identifikasjon) kreves.

    Funksjonene for betinget tilgang er inkludert:

    - Tilgang basert på bruker navn, gruppe og rolle
    - Tilgang [basert på en app](https://docs.microsoft.com/azure/active-directory/conditional-access/app-based-conditional-access) 
    - [Tilgang basert på plassering](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined#conditional-access-policies-for-combined-registration);  bare Tillat tilgang fra klarerte IP-områder eller bestemte land 
    - Krev MFA for tilgang
    - Blokkere tilgang til apper som bruker [eldre godkjenning](https://docs.microsoft.com/azure/active-directory/conditional-access/block-legacy-authentication)
    - Krev at apper bruker [Intune app Protection](https://docs.microsoft.com/azure/active-directory/conditional-access/app-protection-based-conditional-access)
    - Egen definert godkjenning som MFA med tredje parts leverandører, for eksempel DUO.
   
    Andre funksjoner:
    - [Selv betjent tilbakestilling av passord](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-customization) for hybrid Azure ad
    
## <a name="compliance-features"></a>Samsvars funksjoner

Microsoft 365 Business Premium-abonnementet inkluderer funksjoner som hjelper deg med å vedlikeholde samsvar og forskriftsmessige standarder.

- **[Oversikt over policyer for hindring av tap av data](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies)** (hindring). 
    
    Du kan konfigurere DLP for automatisk å oppdage sensitiv informasjon, for eksempel kreditt kort numre, trygde numre og så videre, for å hindre utilsiktet deling utenfor selskapet.
    
- **[Exchange Online Archiving](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Ved hjelp av Exchange Online arkiverings lisens kan meldinger enkelt arkiveres med kontinuerlige data sikkerhets kopiering. Det lagrer alle e-postmeldingene i en bruker, inkludert slettede elementer, i tilfelle de er nødvendige senere for oppdaging eller gjenoppretting. Du kan også bruke forskjellige oppbevarings policyer til å bevare e-postdata for rettslige sperringene, eDiscovery eller for å oppfylle kravene til samsvar.
    
- **[Følsomhetsetiketter](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)**

   Microsoft 365 Business Premium inkluderer alle funksjonene i [Azure Information Protection Plan 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Med denne planen kan du opprette **følsomme etiketter** som lar deg kontrollere tilgang til sensitiv informasjon i e-post og dokumenter, med kontroller som «ikke Videresend» og "Do not Copy." Du kan også klassifisere sensitiv informasjon som "Konfidensielt" og angi hvordan klassifiserings informasjon kan deles utenfor og innenfor virksomheten. Kryptering med bedrifts nivå er enkel å bruke på e-post og dokumenter for å holde informasjonen privat. Du kan også installere tillegget Azure Information Protection-klient for Office-apper. Hvis du vil ha mer informasjon, kan du se [Azure Information Protection Unified Labeling Client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history). Hvis du vil ha følsomme etiketter, kan du installere **AzInfoProtection_UL.exe**.

Du kan administrere disse funksjonene i sikkerhets &amp; samsvars senteret og administrasjons senteret for Intune. Over tid blir de forenklede kontrollene lagt til i administrasjons senteret for Microsoft 365.
  
    
## <a name="faq"></a>Vanlige spørsmål

 ### <a name="are-these-security-features-available-in-all-markets"></a>Er disse sikkerhets funksjonene tilgjengelige i alle markeder?
  
Ja, disse funksjonene er tilgjengelige i alle markeder der Microsoft 365 Business Premium selges.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Hvordan finner jeg sikkerhets &amp; samsvars senteret?
  
1. [Logg på Microsoft 365 Business Premium](https://portal.microsoft.com/) ved hjelp av administrator legitimasjonen din. 
    
2. I det venstre navigasjons feltet finner du **administrasjons sentre** og utvider det. 
    
    ![Velg administrasjons sentre i det venstre navigasjons senteret i Microsoft 365.](../media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Velg **sikkerhets &amp; samsvar** for å gå til sikkerhets &amp; samsvars senteret.
