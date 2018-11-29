---
title: Angi innstillinger for appbeskyttelse, for Android- eller iOS-enheter
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Lær hvordan du kan opprette, redigere, eller slette en policy for informasjonsbehandling av app og beskytte arbeidsfiler på Android eller iOS enheter.
ms.openlocfilehash: ed03227496120369b94bf2396974eebfd7798678
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983666"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Angi innstillinger for appbeskyttelse, for Android- eller iOS-enheter

## <a name="create-an-app-management-policy"></a>Opprette en policy for appbehandling

1. Logg deg på [Microsoft 365 Business](https://portal.office.com) med legitimasjon for globaladministrator. 
    
2. Velg **Legg til policy** på **Enhetspolicyer**-kortet i administratorportalen.
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. Angi et unikt navn for denne policyen på **Legg til policy**-ruten. 
    
4. Velg **Programbehandling for Android** eller **Programbehandling for iOS** under **Policytype**, avhengig av hvilke sett med policyer du vil opprette. 
    
5. Utvid **Beskytt arbeidsfiler når enheter går tapt eller blir stjålet** og **Behandle hvordan brukere får tilgang til Office-filer på mobilenheter** \> konfigurer innstillingene slik du ønsker. **Administrer hvordan brukere får tilgang til Office-filer på mobilenheter** er slått **Av** som standard, men det anbefales at du slår den **På** og godtar standardverdiene. Du kan se [Tilgjengelige innstillinger](app-protection-settings-for-android-and-ios.md#bkmk_availablesettings) for mer informasjon. 
    
    Du kan til enhver tid bruke **Tilbakestill standardinnstillinger**-koblingen for å gå tilbake til standardinnstillingen. 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Bestem deretter **Hvem får disse innstillingene?** Hvis du ikke vil bruke den standard sikkerhetsgruppen **Alle brukere**, velger du **Endre**, og velg så sikkerhetsgruppene som vil få disse innstillingene \> **Velg**.
    
7. Velg til slutt **Ferdig** for å lagre policyen og tilordne den til enhetene. 
    
## <a name="edit-an-app-management-policy"></a>Endre en policy for appbehandling

1. Velg **Rediger policy**på kortet **policyer** .
    
2. Velg policyen du vil endre, på **Rediger policy**-ruten 
    
3. Velg **Rediger** ved siden av hver innstilling for å endre verdiene i policyen. Når du endrer en verdi, lagres den automatisk i policyen 
    
4. Lukk **Rediger policy**-ruten når du er ferdig. 
    
## <a name="delete-an-app-management-policy"></a>Slette en policy for appbehandling

1. Velg **Slette policy** på **Policyer**-kortet.
    
2. Velg den policyen du ønsker å slette, på **Slett policy**-ruten \> **Velg**, deretter **Bekreft** for å slette policyen du valgte. 
    
## <a name="available-settings"></a>Tilgjengelige innstillinger

Tabellene nedenfor gir detaljert informasjon om de tilgjengelige innstillingene for å beskytte arbeidsfiler på enheter, samt innstillingene som kontrollerer hvordan brukere får tilgang til Office-filer fra de mobile enhetene.
  
 Se [Hvordan tilordnes beskyttelsesfunksjoner i Microsoft 365 Business til Intune-innstillinger](map-protection-features-to-intune-settings.md) for mer informasjon. 
  
### <a name="settings-that-protect-work-files"></a>Innstillinger som beskytter arbeidsfiler

Følgende innstillinger er tilgjengelig for å beskytte arbeidsfiler hvis en brukers enhet mistes eller stjeles:
  
|||
|:-----|:-----|
|Innstilling  <br/> |Beskrivelse  <br/> |
|Slette arbeidsfiler fra en inaktiv enhet etter et visst antall dager  <br/> |Hvis en enhet ikke er blitt brukt i løpet av det antallet dager som du spesifiserer her, vil eventuelle arbeidsfiler som er lagret på enheten automatisk bli slettet.  <br/> |
|Tvinge brukere til å lagre alle arbeidsfiler til OneDrive for Business  <br/> |Hvis denne innstillingen er **på**, vil den eneste tilgjengelige lagringsplasseringen for arbeidsfiler være OneDrive for Business.  <br/> |
|Kryptere arbeidsfiler  <br/> |Behold denne innstillingen **på** slik at arbeidsfiler er beskyttet ved hjelp av kryptering. Selv om enheten mistes eller stjeles, vil ingen kunne lese firmadataene.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Innstillinger som kontrollerer hvordan brukere får tilgang til Office-filer på mobile enheter

Følgende innstillinger er tilgjengelig for å styre hvordan brukere får tilgang til Office-arbeidsfiler:
  
|||
|:-----|:-----|
|Innstilling  <br/> |Beskrivelse  <br/> |
|Kreve en PIN-kode eller et fingeravtrykk for å få tilgang til Office-apper  <br/> |Hvis disse innstillingene er **På**, må brukere gi en annen form for godkjenning, i tillegg til brukernavn og passord, før de kan bruke Office-apper på mobilenheten.  <br/> |
|Tilbakestille PIN-kode når påloggingen mislykkes et visst antall ganger  <br/> |Hvis du vil forhindre at en uautorisert bruker tilfeldig gjetter en PIN-kode, tilbakestilles PIN-koden etter det antallet feiloppføringer du angir.  <br/> |
|Kreve at brukere logger seg på igjen etter at Office-apper har vært inaktive i  <br/> |Denne innstillingen bestemmer hvor lenge en bruker kan være inaktiv før de blir bedt om å logge seg på igjen.  <br/> |
|Avslå tilgang til å arbeidsfiler på enheter der programvarebegrensningene er fjernet, eller enheter som har blitt utsatt for utiltenkt rottilgang  <br/> |Smarte brukere har kanskje en enhet der programvarebegrensningene er fjernet, eller en enhet som har blitt utsatt for utiltenkt rottilgang. Dette betyr at brukeren kan endre operativsystemet, noe som kan gjøre enheten mer utsatt for skadelig programvare. Disse enhetene blokkeres når denne innstillingen er **På**.  <br/> |
|Tillate brukere å kopiere innhold fra Office-apper til personlige apper  <br/> |Vi tillater dette som standard, men hvis innstillingen er **aktivert**, brukeren kan kopiere informasjonen i en work-fil til en fil med personlige. Hvis innstillingen er **deaktivert**, vil brukeren ikke kunne kopiere informasjon fra en arbeidskonto til en personlig app eller personlig konto.<br/> |
   

  

