---
title: Hvordan kan beskyttelsesfunksjoner i Microsoft 365 Business Premium tilordne til Intune-innstillinger
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
ms.date: 8/13/2018
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: aad21b1a-c775-469a-b89c-c5d1d59d27db
description: Lær hvordan beskyttelsesfunksjoner i Microsoft 365 Business Premium tilordnes Intune-innstillinger. Abonnementet gir deg en lisens til å endre Intune-innstillinger.
ms.openlocfilehash: 844b83bca9483f72fd322d666803c42b90fee41d3e0047ea93b4b6b07717b0dd
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53852735"
---
# <a name="how-do-protection-features-in-microsoft-365-business-premium-map-to-intune-settings"></a>Hvordan kan beskyttelsesfunksjoner i Microsoft 365 Business Premium tilordne til Intune-innstillinger

## <a name="android-and-ios-application-protection-settings"></a>Innstillinger for programbeskyttelse for Android og iOS

Tabellen nedenfor inneholder detaljert informasjon om hvordan policyinnstillingene for Android- og iOS-programmer tilordnes til Intune-innstillinger.
  
Hvis du vil finne Intune-innstillingen, logger du på med Microsoft 365 Business Premium administratorlegitimasjon og går til **Administrasjonssentre** og **deretter Intune**.
  
 > [!IMPORTANT]
 > 
 > Et Microsoft 365 Business Premium gir deg en lisens til å endre alle Intune-innstillingene. Se [Innføring i Intune for å komme i gang.](/intune/introduction-intune)
  
Velg policynavnet du vil &mdash; bruke, for eksempel Programpolicy for &mdash; Android, og velg deretter **Policyinnstillinger**.
  
Under **Beskytt arbeidsfiler når enheter er tapt eller stjålne**
  
|**Policyinnstilling for Android- eller iOS-programmer**|**Intune-innstilling(er)**|
|:-----|:-----|
|Slett arbeidsfiler fra en inaktiv enhet etter  <br/> |Intervall (antall dager) som angir når appdata fjernes i frakoblet modus  <br/> |
|Tving brukere til å lagre arbeidsfiler til OneDrive for Business  <br/> Vær oppmerksom på at bare OneDrive for Business er tillatt  <br/> |Velg hvilke lagringstjenester bedriftsdata kan lagres til  <br/> |
|||
   
Under **Administrere hvordan brukere får tilgang til Office-filer på mobile enheter**
  
|**Policyinnstilling for Android- eller iOS-programmer**|**Intune-innstilling(er)**|
|:-----|:-----|
|Slett arbeidsfiler fra en inaktiv enhet etter  <br/> |Intervall (antall dager) som angir når appdata fjernes i frakoblet modus  <br/> |
|Tving brukere til å lagre arbeidsfiler til OneDrive for Business  <br/> Vær oppmerksom på at bare OneDrive for Business er tillatt  <br/> |Velg hvilke lagringstjenester bedriftsdata kan lagres til  <br/> |
|Kryptere arbeidsfiler  <br/> |Kryptere appdata  <br/> |
|Under **Administrere hvordan brukere får tilgang til Office-filer på mobile enheter** <br/> ||
|Kreve en PIN-kode eller et fingeravtrykk for å få tilgang til Office-apper  <br/> | Kreve PIN-kode for å få tilgang til  <br/>  Dette angir også:  <br/> **Tillat enkel PIN-kode** til **Ja** <br/> **Lengde for PIN-kode** til 4  <br/> **Tillat fingeravtrykk i stedet for PIN** til **Ja** <br/> **Deaktiver PIN-koden for appen når PIN-kode for enheten er angitt** til **Nei** <br/> |
|Tilbakestill PIN-kode når påloggingen mislykkes så mange ganger (dette er deaktivert hvis PIN-kode ikke er nødvendig)  <br/> |Antall forsøk før tilbakestilling av PIN-kode  <br/> |
|Krev at brukere logger på på nytt Office har vært inaktive for (dette er deaktivert hvis PIN-kode ikke er nødvendig)  <br/> | Kontroller tilgangskravene etter (minutter)  <br/>  Dette angir også:  <br/> **Tidsavbrudd** er angitt til minutter  <br/>  Dette er samme antall minutter som du angir i Microsoft 365 Business.  <br/> **Frakoblet løpeperiode** er satt til 720 minutter som standard  <br/> |
|Avslå tilgang til arbeidsfiler på enheter som er jailbreaket eller rootet  <br/> |Blokker administrerte apper fra å kjøre på enheter som er jailbreaket eller rootet  <br/> |
|Tillat at brukere kan kopiere innhold fra Office-apper til personlige apper  <br/> | Begrense klipp ut, kopier og lim inn med andre apper  <br/>  Hvis alternativet Microsoft 365 Business Premium er satt til **På**, er disse tre alternativene også satt til **Alle apper** i Intune:  <br/> **Tillat at appen kan overføre data til andre apper** <br/> **Tillat at appen kan motta data fra andre apper** <br/> **Begrens klipping, kopiering og liming med andre apper** <br/>  Hvis alternativet Microsoft 365 Business er satt til **På**, er alle Intune-alternativene satt til:  <br/> **Tillat at appen kan overføre data til andre apper** er satt til **Policyadministrerte apper** <br/> **Tillat at appen kan motta data fra andre apper** er satt til **Alle apper** <br/> **Begrens klipping, kopiering og liming med andre apper** er satt til **Policyadministrerte apper med Innliming** <br/> |
|||
   
## <a name="windows-10-app-protection-settings"></a>Innstillinger for appbeskyttelse i Windows 10

Tabellen nedenfor inneholder detaljert informasjon om hvordan policyinnstillingene for Windows 10-programmer tilordnes til Intune-innstillinger.
  
Hvis du vil finne Intune-innstillingen, logger du på med Microsoft 365 Business Premium administratorlegitimasjon og går til [Azure Portal](https://portal.azure.com). Velg **Flere tjenester**, og skriv inn Intune i **Filter**. Velg **Apppolicy for Intune App** \> **Protection**.
  
 > [!IMPORTANT]
 >
 >Et Microsoft 365 Business Premium gir deg en lisens til å endre bare Intune-innstillingene som tilordnes til innstillingene som er tilgjengelige i Microsoft 365 Business Premium. 
  
Hvis du vil utforske de tilgjengelige innstillingene, velger du policynavnet du vil bruke, og  deretter velger du **Generelt,** Oppgaver **,** Tillatte apper **,** Unntatt apper **,** Obligatoriske innstillinger eller Avanserte innstillinger fra venstre navigasjonsrute. 
  
|**Policyinnstilling for Windows 10-programmer**|**Intune-innstilling(er)**|
|:-----|:-----|
|Kryptere arbeidsfiler  <br/> |**Avanserte innstillinger** \> **Databeskyttelse**: **Tilbakekall krypteringstastene for avregistrering** og **Opphev tilgang til beskyttede data enheten registrerer til MDM** er begge satt til **På**.  <br/> |
|Forhindre at brukere kopierer bedriftsdata over til personlige filer.  <br/> |**Obligatorisk innstillinger** \> **Windows Information Protection-modus**. **På** i Microsoft 365 Business Premium til: **Skjul overstyringer**, **Av** i Microsoft 365 Business Premium tilordnes til: **Av**.  <br/> |
|Tilgangskontroll for Office-dokumenter  <br/> | Hvis dette er satt til **På** i Microsoft 365 Business Premium, deretter  <br/> **Avanserte innstillinger** \> **Tilgang**, **Bruk Windows Hello for bedrifter som en metode for å logge deg på Windows** er satt til **På**, med følgende tilleggsinnstillinger:  <br/> **Angi det minste antallet tegn som er nødvendig for PIN-koden** er satt til **4**.  <br/> **Konfigurasjon av bruken av store bokstaver i PIN-koden for Windows Hello for bedrifter** er satt til **Ikke tillat bruk av store bokstaver i PIN-koden**.  <br/> **Konfigurasjon av bruken av små bokstaver i PIN-koden for Windows Hello for bedrifter** er satt til **Ikke tillat bruk av små bokstaver i PIN-koden**.  <br/> **Konfigurasjon av bruken av spesialtegn i PIN-koden for Windows Hello for bedrifter** er satt til **Ikke tillat bruk av spesialtegn i PIN-koden**.  <br/> **Angi tidsperioden (i dager)** som en PIN-kode kan brukes før systemet krever at brukeren endrer, er satt til **0**.  <br/> **Angi antallet tidligere PIN-koder som kan knyttes til en brukerkonto som ikke kan brukes på nytt** er satt til **0**.  <br/> **Antall godkjenningsfeil som er tillatt før enheten tømmes** er satt til det samme som i Microsoft 365 Business (5 som standard).  <br/> **Maksimum tid (i minutter) tillatt når enheten blir inaktiv, som vil føre til at enheten blir beskyttet med PIN-kode eller passord** er satt til det samme som i Microsoft 365 Business.  <br/> |
|Aktivere gjenoppretting av beskyttet data  <br/> |**Avanserte innstillinger** \> **Databeskyttelse**: **Vis ikonet for beskyttelse av bedriftsdata** og **Bruk Azure RMS for VIA** er satt til **På**.  <br/> |
|Beskytte flere skyplasseringer for firma  <br/> |**Avanserte innstillinger** \> **Beskyttede domener** og **Ressurser i skyen** viser domener og SharePoint-områder.  <br/> |
|Filer som brukes av disse appene, er beskyttet  <br/> |Listen over beskyttede apper er oppført i **Tillatte apper**.  <br/> |
|||
   
## <a name="windows-10-device-protection-settings"></a>Innstillinger for enhetsbeskyttelse i Windows 10

Tabellen nedenfor inneholder detaljert informasjon om hvordan innstillinger for enhetskonfigurasjon for Windows 10 tilordnes Intune-innstillinger.
  
Hvis du vil finne Intune-innstillingen, logger du på med Microsoft 365 Business Premium administratorlegitimasjon og går til [Azure Portal](https://portal.azure.com), velger flere tjenester **og** skriver inn Intune i **Filter**, velger **Intune** \> **Device configuration** \> **Profiles**. Then select **Device policy for Windows 10** \> **Properties** \> **Settings**.
  
|**Innstilling for enhetspolicy for Windows 10**|**Intune-innstilling(er)**|
|:-----|:-----|
|Beskytt PC-er mot virus og andre trusler ved hjelp av Windows Defender Antivirus  <br/> |Tillate overvåking i sanntid = PÅ  <br/> Tillat Nettbasert beskyttelse = PÅ  <br/> Be brukerne om innsending av eksempler= Sende sikre eksempler automatisk (automatisk innsending av ikke-standard personlig identifiserbar informasjon)  <br/> |
|Beskytt PC-er fra nettbaserte trusler i Microsoft Edge  <br/> |**SmartScreen** i **Innstillinger for Microsoft Edge-nettleseren** er satt til **Obligatorisk**.  <br/> |
|Slå av skjermen på enheten når den har vært inaktiv i (minutter)  <br/> |Maksimalt antall minutter med inaktivitet før skjermen låses (minutter)  <br/> |
|Tillat brukere å laste ned apper fra Microsoft Store  <br/> |Egendefinert URI-policy  <br/> |
|Gi brukere tilgang til Cortana  <br/> |**Generelt** \> **Cortana** er satt til å **blokkere** i Intune når den er satt til **av** i Microsoft 365 Business Premium.  <br/> |
|Tillat brukere å motta Windows-tips og annonser fra Microsoft  <br/> |**Windows er** blokkert hvis dette er satt til **av** i Microsoft 365 Business Premium.  <br/> |
|Holde Windows 10-enheter oppdatert automatisk  <br/> | Denne innstillingen er **i Microsoft Intune** \> **tjenesteoppdateringer – Windows 10 Oppdateringsringer**, velg Oppdater **policy for Windows 10-enheter** og deretter  \> **Egenskaper Innstillinger**.  <br/>  Når Microsoft 365 Business Premium er satt til **På**, angis alle følgende innstillinger:  <br/> **Tjenestegren** er satt til **CB** (CBB når dette er deaktivert i Microsoft 365 Business Premium).  <br/> **Microsoft-produktoppdateringer** er satt til **Tillat**.  <br/> **Windows-drivere** er satt til **Tillat**.  <br/> **Virkemåte for automatisk oppdatering** er satt til **Installere automatisk på tidspunkt for vedlikehold** med:  <br/> **Etter arbeidstid** er satt til **06:00**.  <br/> **Aktivitetsperiode** er satt til **22:00**.  <br/> **Utsettelsesperiode (dager) for kvalitetsoppdatering** er satt til **0**.  <br/> **Utsettelsesperiode (dager) for funksjonsoppdatering** er satt til **0**.  <br/> **Delivery optimization download mode** is set to **HTTP blended with peering behind same NAT**.  <br/> |
|||
