---
title: Valider app innstillinger for databeskyttelse på Android eller iOS enheter
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: 'Learn how to validate the Microsoft 365 Business app protection settings in your Android or iOS devices.  '
ms.openlocfilehash: 300f59e81a93cc3dfc03fd1d98891be1ac4f7795
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983676"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a>Valider app innstillinger for databeskyttelse på Android eller iOS enheter

Følg instruksjonene i kategoriene for å validere app innstillinger for databeskyttelse på Android eller iOS enheter.
  
## <a name="androidtab"></a>[Android](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a>Kontroller at innstillingene for appbeskyttelse fungerer på brukerenheter

Når du har [angitt appkonfigurasjoner for Android-enheter](app-protection-settings-for-android-and-ios.md) for å beskytte appene, kan du følge disse trinnene for å validere at innstillingene du velger, fungerer. 
  
Først må du kontrollere at policyen gjelder for appen du skal validere.
  
1. Gå til [Policyer](https://portal.office.com) **** \> i Microsoft 365 Business **-administrasjonssenteret**.
    
2. Velg **Programpolicy for Android** for innstillingen du opprettet under konfigureringen, eller en annen policy du opprettet, og kontroller at den håndheves for for eksempel Outlook. 
    
    ![Shows all the apps for which this policy protects files.](media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a>Valider Krev en PIN-kode eller et fingeravtrykk for å få tilgang til Office-apper

Velg **Rediger** ved siden av **Tilgangskontroll for Office-dokumenter**, og utvid **Administrer hvordan brukere får tilgang til Office-filer på mobile enheter** i **Rediger policy**-ruten. Sørg for at **Krever en PIN eller et fingeravtrykk for å få tilgang til Office-apper** er satt til **På**.
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. Åpne Outlook I brukerens Android-enhet, og logg deg på med brukerens Microsoft 365 Business-legitimasjon.
    
2. Du vil også bli bedt om å angi en PIN-kode eller bruke et fingeravtrykk.
    
    ![Enter a PIN on your Android device to access Office apps.](media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a>Valider Tilbakestill PIN-kode etter et antall mislykkede forsøk

Velg **Rediger** ved siden av **Tilgangskontroll for Office-dokumenter**, og utvid **Administrer hvordan brukere får tilgang til Office-filer på mobile enheter** i **Rediger policy**-ruten. Sørg for at **Tilbakestill PIN-kode etter et antall mislykkede forsøk** er satt til et nummer - dette antallet er fem som standard. 
  
1. Åpne Outlook I brukerens Android-enhet, og logg deg på med brukerens Microsoft 365 Business-legitimasjon.
    
2. Skriv inn feil PIN-kode så mange ganger som angitt av policyen. Du får se en melding der det står **Antall PIN-kodeforsøk er oppnådd** for å tilbakestille PIN-koden. 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. Trykk på **tilbakestille PIN-kode**. Du blir bedt om å logge inn med brukerens Microsoft 365 Business-administratorlegitimasjon, og deretter kreves det at du angir en ny PIN-kode.
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a>Valider Tving brukere å lagre alle arbeidsfiler til OneDrive for Business

Velg **Rediger** ved siden av **Beskyttelse mot tapte eller stjålne enheter** i **Rediger policy**-ruten. Utvid **Beskytt arbeidsfiler når enheter går tapt eller stjålet**, og sørg for at **Tving brukere til å lagre alle arbeidsfiler til OneDrive for Business** er satt til **På**.
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. Åpne Outlook i brukerens Android-enhet, logg deg på med brukerens Microsoft 365 Business-legitimasjon, og skriv inn en PIN-kode om nødvendig.
    
2. Åpne en e-postmelding som inneholder et vedlegg, og trykk på Pil ned-ikonet ved siden av vedleggsinformasjonen.
    
    ![Tap the down arrow next to an attachment to try to save it.](media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    Du vil se **Kan ikke lagre til enheten** nederst på skjermen. 
    
    ![Warning text that indicates cannot save a file locally to an Android.](media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > Lagre på OneDrive for Business er for øyeblikket ikke aktivert for Android, slik at du bare ser at lagring lokalt er blokkert. 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a>Valider Krev at brukeren logger på på nytt hvis Office-apper har vært inaktive i et angitt tidsrom

Velg **Rediger** ved siden av **Tilgangskontroll for Office-dokumenter**, og utvid **Administrer hvordan brukere får tilgang til Office-filer på mobile enheter** i **Rediger policy**-ruten. Sørg for at **Krever at brukerne logger på igjen etter at Office-apper har vært inaktive i en periode** er satt til noen minutter - perioden er 30 minutter som standard. 
  
1. Åpne Outlook i brukerens Android-enhet, logg deg på med brukerens Microsoft 365 Business-legitimasjon, og skriv inn en PIN-kode om nødvendig.
    
2. Du bør nå se innboksen til Outlook. La Android-enheten være uvirksom og urørt i minst 30 minutter (eller en annen tidsperiode, men lengre enn det du spesifiserte i policyen). Enheten vil sannsynligvis tone ned.
    
3. Få tilgang på nytt til Outlook på Android-enheten.
    
4. Du vil bli bedt om å angi PIN-koden før du igjen får tilgang til Outlook.
    
### <a name="validate-protect-work-files-with-encryption"></a>Valider Beskytt arbeidsfiler med kryptering

Velg **Rediger** ved siden av **Beskyttelse mot tapte eller stjålne enheter** i **Rediger policy**-ruten. Utvid **Beskytt arbeidsfiler når enheter går tapt eller stjålet**, og sørg for at **Beskytt arbeidsfiler med kryptering** er satt til **På** og **Tvinge brukere å lagre alle arbeidsfiler til OneDrive for Business** er satt til **Av**.
  
1. Åpne Outlook i brukerens Android-enhet, logg deg på med brukerens Microsoft 365 Business-legitimasjon, og skriv inn en PIN-kode om nødvendig.
    
2. Åpne en e-postmelding som inneholder noen bildefiler som vedlegg.
    
3. Trykk på Pil ned-ikonet ved siden av vedleggsinformasjonen for å lagre den.
    
    ![Tap the down arrow to save the figure file to the Android device.](media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. Du kan bli bedt om å gi Outlook tilgang til bildene, medier og filer på enheten. Trykk på **Tillat**.
    
5. Nederst på skjermen kan du velge å **Lagre til enhet** og deretter åpne **Galleri** -appen. 
    
6. Du bør nå se et kryptert bilde (eller flere hvis du har lagret flere bildefilvedlegg) i listen. Bildet kan vises på bildelisten som en grå firkant med et hvitt utropstegn inne i en hvit sirkel midt på den grå firkanten.
    
    ![An encrypted image file in the Gallery app.](media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="iostab"></a>[iOS](#tab/)
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a>Kontroller at innstillingene for appbeskyttelse fungerer på brukerenheter

Når du har [angitt appkonfigurasjoner for iOS-enheter](app-protection-settings-for-android-and-ios.md) for å beskytte apper, kan du følge disse trinnene for å validere at innstillingene du velger, fungerer. 
  
Først må du kontrollere at policyen gjelder for appen du skal validere.
  
1. Gå til [Policyer](https://portal.office.com) **** \> i Microsoft 365 Business **-administrasjonssenteret**.
    
2. Velg **Programpolicyer for iOS** for innstillingene du opprettet under konfigureringen, eller en annen policy du opprettet, og kontroller at den håndheves for for eksempel Outlook. 
    
    ![Shows all the apps for which this policy protects files.](media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a>Valider Krev en PIN-kode å få tilgang til Office-apper

Velg **Rediger** ved siden av **Tilgangskontroll for Office-dokumenter**, og utvid **Administrer hvordan brukere får tilgang til Office-filer på mobile enheter** i **Rediger policy**-ruten. Sørg for at **Krever en PIN eller et fingeravtrykk for å få tilgang til Office-apper** er satt til **På**.
  
![Make sure that the Require a PIN or fingerprint to acces Office apps is set to On.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. Åpne Outlook i brukerens iOS-enhet, og logg deg på med brukerens Microsoft 365 Business-legitimasjon.
    
2. Du vil også bli bedt om å angi en PIN-kode eller bruke et fingeravtrykk.
    
    ![Enter a PIN on your IOS device to access Office apps.](media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a>Valider Tilbakestill PIN-kode etter et antall mislykkede forsøk

Velg **Rediger** ved siden av **Tilgangskontroll for Office-dokumenter**, og utvid **Administrer hvordan brukere får tilgang til Office-filer på mobile enheter** i **Rediger policy**-ruten. Sørg for at **Tilbakestill PIN-kode etter et antall mislykkede forsøk** er satt til et nummer - dette antallet er fem som standard. 
  
1. Åpne Outlook i brukerens iOS-enhet, og logg deg på med brukerens Microsoft 365 Business-legitimasjon.
    
2. Skriv inn feil PIN-kode så mange ganger som angitt av policyen. Du får se en melding der det står **Antall PIN-kodeforsøk er oppnådd** for å tilbakestille PIN-koden. 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. Trykk på **OK**. Du blir bedt om å logge inn med brukerens Microsoft 365 Business-administratorlegitimasjon, og deretter kreves det at du angir en ny PIN-kode.
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a>Valider Tving brukere å lagre alle arbeidsfiler til OneDrive for Business

Velg **Rediger** ved siden av **Beskyttelse mot tapte eller stjålne enheter** i **Rediger policy**-ruten. Utvid **Beskytt arbeidsfiler når enheter går tapt eller stjålet**, og sørg for at **Tving brukere til å lagre alle arbeidsfiler til OneDrive for Business** er satt til **På**.
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. Åpne Outlook i brukerens iOS-enhet, logg deg på med brukerens Microsoft 365 Business-legitimasjon, og skriv inn en PIN-kode om nødvendig.
    
2. Åpne en e-postmelding som inneholder et vedlegg, åpne vedlegget, og velg **Lagre** nederst på skjermen. 
    
    ![Tap the Save option after you open an attachment to try to save it.](media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. Du bør nå bare se alternativet for OneDrive for Business. Hvis ikke kan du trykke på **Legg til konto** og velge **OneDrive for Business** fra **Legg til lagringskonto**-skjermen. Angi sluttbrukerens Microsoft 365 Business for å logge på når du blir bedt om det. 
    
    Trykk på **Lagre**, og velg **OneDrive for Business**.
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a>Valider Krev at brukeren logger på på nytt hvis Office-apper har vært inaktive i et angitt tidsrom

Velg **Rediger** ved siden av **Tilgangskontroll for Office-dokumenter**, og utvid **Administrer hvordan brukere får tilgang til Office-filer på mobile enheter** i **Rediger policy**-ruten. Sørg for at **Krever at brukerne logger på igjen etter at Office-apper har vært inaktive i en periode** er satt til noen minutter - perioden er 30 minutter som standard. 
  
1. Åpne Outlook i brukerens iOS-enhet, logg deg på med brukerens Microsoft 365 Business-legitimasjon, og skriv inn en PIN-kode om nødvendig.
    
2. Du bør nå se innboksen til Outlook. La iOS-enheten være uberørt i minst 30 minutter (eller en annen tidsperiode, men lengre enn det du spesifiserte i policyen). Enheten vil sannsynligvis tone ned.
    
3. Få tilgang på nytt til Outlook på iOS-enheten.
    
4. Du vil bli bedt om å angi PIN-koden før du igjen får tilgang til Outlook.
    
### <a name="validate-protect-work-files-with-encryption"></a>Valider Beskytt arbeidsfiler med kryptering

Velg **Rediger** ved siden av **Beskyttelse mot tapte eller stjålne enheter** i **Rediger policy**-ruten. Utvid **Beskytt arbeidsfiler når enheter går tapt eller stjålet**, og sørg for at **Beskytt arbeidsfiler med kryptering** er satt til **På** og **Tvinge brukere å lagre alle arbeidsfiler til OneDrive for Business** er satt til **Av**.
  
1. Åpne Outlook i brukerens iOS-enhet, logg deg på med brukerens Microsoft 365 Business-legitimasjon, og skriv inn en PIN-kode om nødvendig.
    
2. Åpne en e-postmelding som inneholder noen bildefiler som vedlegg.
    
3. Trykk på vedlegget, og trykk deretter på **Lagre**-alternativet under vedlegget. 
    
4. Åpne **Bilde**-appen på startskjermen. Du bør nå se et kryptert bilde (eller flere hvis du har lagret flere bildefilvedlegg) som er lagret, men kryptert. 
    
---

