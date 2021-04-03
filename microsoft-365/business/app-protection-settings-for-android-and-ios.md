---
title: Angi innstillinger for appbeskyttelse, for Android- eller iOS-enheter
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
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
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Lær hvordan du oppretter, redigerer eller sletter en policy for appbehandling og beskytter arbeidsfiler på Android- eller iOS-enheter.
ms.openlocfilehash: 2e157737990c7aca6e87a676e90f62f0d40ad372
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580298"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a>Angi innstillinger for appbeskyttelse, for Android- eller iOS-enheter

Denne artikkelen gjelder for Microsoft 365 Business Premium.

## <a name="create-an-app-management-policy"></a>Opprette en policy for appbehandling

1. Gå til administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
    
2. Velg Legg til  enheter policyer i det venstre \>  \> **navigasjonsfeltet.**
  
3. Angi et unikt navn for denne policyen på **Legg til policy**-ruten. 
    
4. Velg **Programbehandling** **for Android** eller **Programbehandling for iOS** under Policytype , avhengig av hvilket sett med policyer du vil opprette. 
    
5. Utvid **Beskytt arbeidsfiler når enheter går tapt eller blir** stjålet og Administrer hvordan brukere får tilgang til **Office-filer på mobile enheter.** Konfigurer innstillingene slik du ønsker. **Administrer hvordan brukere får tilgang til Office-filer** på mobile enheter  er Av **som** standard, men vi anbefaler at du slår den på og godtar standardverdiene. Hvis du vil ha mer informasjon, kan [du se Tilgjengelige innstillinger](#available-settings). 
    
    Du kan til enhver tid bruke **Tilbakestill standardinnstillinger**-koblingen for å gå tilbake til standardinnstillingen. 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. Bestem deretter **Hvem får disse innstillingene?** Hvis du ikke vil bruke standard sikkerhetsgruppe **for** alle brukere, velger du Endre **,** velger sikkerhetsgruppene som får disse innstillingene \> **Velg**.
    
7. Velg til slutt **Ferdig** for å lagre policyen og tilordne den til enhetene. 
    
## <a name="edit-an-app-management-policy"></a>Endre en policy for appbehandling

1. Velg Rediger **policy** på **Policyer-kortet.**
    
2. Velg policyen du vil endre, på **Rediger policy**-ruten 
    
3. Velg **Rediger** ved siden av hver innstilling for å endre verdiene i policyen. Når du endrer en verdi, lagres den automatisk i policyen.
    
4. Når du er ferdig, lukker du **Rediger policy-ruten.** 
    
## <a name="delete-an-app-management-policy"></a>Slette en policy for appbehandling

1. Velg en **policy** på Policyer-siden, og velg deretter **Slett**.
    
2. Velg **Bekreft i** Slett policy-ruten **for** å slette policyen eller policyene du valgte. 
    
## <a name="available-settings"></a>Tilgjengelige innstillinger

Tabellene nedenfor gir detaljert informasjon om innstillinger som er tilgjengelige for å beskytte arbeidsfiler på enheter og innstillingene som styrer hvordan brukere får tilgang til Office-filer fra sine mobile enheter.
  
 Hvis du vil ha mer informasjon, kan du se [Hvordan fungerer beskyttelsesfunksjoner i Microsoft 365 Business Premium-kart til Intune-innstillinger](map-protection-features-to-intune-settings.md). 
  
### <a name="settings-that-protect-work-files"></a>Innstillinger som beskytter arbeidsfiler

Følgende innstillinger er tilgjengelig for å beskytte arbeidsfiler hvis en brukers enhet mistes eller blir stjålet:
  
|||
|:-----|:-----|
|Innstilling  <br/> |Beskrivelse  <br/> |
|Slette arbeidsfiler fra en inaktiv enhet etter et visst antall dager  <br/> |Hvis en enhet ikke brukes for antall dager du angir her, slettes alle arbeidsfiler som er lagret på enheten, automatisk.  <br/> |
|Tvinge brukere til å lagre alle arbeidsfiler til OneDrive for Business  <br/> |Hvis denne innstillingen er **På**, er den eneste tilgjengelige lagringsplasseringsplasseringen for arbeidsfiler OneDrive for Business.  <br/> |
|Kryptere arbeidsfiler  <br/> |Behold denne innstillingen **På** slik at arbeidsfiler er beskyttet ved hjelp av kryptering. Selv om enheten er mistet eller stjålet, kan ingen lese firmadataene dine.  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a>Innstillinger som kontrollerer hvordan brukere får tilgang til Office-filer på mobile enheter

Følgende innstillinger er tilgjengelig for å styre hvordan brukere får tilgang til Office-arbeidsfiler:
  
|||
|:-----|:-----|
|Innstilling  <br/> |Beskrivelse  <br/> |
|Kreve en PIN-kode eller et fingeravtrykk for å få tilgang til Office-apper  <br/> |Hvis denne  innstillingen er På-brukere, må de oppgi en annen form for godkjenning, i tillegg til brukernavn og passord, før de kan bruke Office-apper på sine mobile enheter.<br/> |
|Tilbakestille PIN-kode når påloggingen mislykkes et visst antall ganger  <br/> |Hvis du vil forhindre at en uautorisert bruker tilfeldig gjetter en PIN-kode, tilbakestilles PIN-koden etter det antallet feiloppføringer du angir.  <br/> |
|Kreve at brukere logger seg på igjen etter at Office-apper har vært inaktive i  <br/> |Denne innstillingen bestemmer hvor lenge en bruker kan være inaktiv før de blir bedt om å logge på igjen.  <br/> |
|Avslå tilgang til arbeidsfiler på enheter der programvarebegrensningene er fjernet, eller enheter som har blitt utsatt for utiltenkt rottilgang  <br/> |Smarte brukere har kanskje en enhet der programvarebegrensningene er fjernet, eller en enhet som har blitt utsatt for utiltenkt rottilgang. Dette betyr at brukeren kan endre operativsystemet, noe som kan gjøre enheten mer utsatt for skadelig programvare. Disse enhetene blokkeres når denne innstillingen er **På**.  <br/> |
|Ikke tillat brukere å kopiere innhold fra Office-apper til personlige apper  <br/> |Vi tillater dette som standard, men hvis innstillingen er satt til **På**, vil brukeren kunne kopiere informasjon fra en arbeidsfil til en personlig fil. Hvis innstillingen er **Av**, kan ikke brukeren kopiere informasjon fra en jobbkonto til en personlig app eller personlig konto.  <br/> |
