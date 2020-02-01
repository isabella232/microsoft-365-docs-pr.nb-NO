---
title: Validere appbeskyttelsesinnstillinger på Android- eller iOS-enheter
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: f3433b6b-02f7-447f-9d62-306bf03638b0
description: Learn how to validate the Microsoft 365 Business app protection settings in your Android or iOS devices.
ms.openlocfilehash: 47ce137f785c595992886c756ad85b80957272fe
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594979"
---
# <a name="validate-app-protection-settings-on-android-or-ios-devices"></a><span data-ttu-id="27f34-103">Validere appbeskyttelsesinnstillinger på Android- eller iOS-enheter</span><span class="sxs-lookup"><span data-stu-id="27f34-103">Validate app protection settings on Android or iOS devices</span></span>

<span data-ttu-id="27f34-104">Følg instruksjonene i avsnittene nedenfor for å validere appbeskyttelsesinnstillinger på Android- eller iOS-enheter.</span><span class="sxs-lookup"><span data-stu-id="27f34-104">Follow the instructions in the following sections to validate app protection settings on Android or iOS devices.</span></span>
  
## <a name="android"></a><span data-ttu-id="27f34-105">Android</span><span class="sxs-lookup"><span data-stu-id="27f34-105">Android</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="27f34-106">Kontroller at innstillingene for appbeskyttelse fungerer på brukerenheter</span><span class="sxs-lookup"><span data-stu-id="27f34-106">Check that the app protection settings are working on user devices</span></span>

<span data-ttu-id="27f34-107">Når du har [angitt appkonfigurasjoner for Android-enheter](app-protection-settings-for-android-and-ios.md) for å beskytte appene, kan du følge disse trinnene for å validere at innstillingene du velger, fungerer.</span><span class="sxs-lookup"><span data-stu-id="27f34-107">After you [set app configurations for Android devices](app-protection-settings-for-android-and-ios.md) to protect the apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="27f34-108">Først må du kontrollere at policyen gjelder for appen der du skal validere den.</span><span class="sxs-lookup"><span data-stu-id="27f34-108">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="27f34-109">Gå til [Policyer](https://portal.office.com)\*\*\*\*\> i Microsoft 365 Business **-administrasjonssenteret**.</span><span class="sxs-lookup"><span data-stu-id="27f34-109">In the Microsoft 365 Business [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="27f34-110">Velg **Programpolicy for Android** for innstillingene du opprettet ved installasjonen, eller en annen policy du opprettet, og kontroller at den for eksempel håndheves for Outlook.</span><span class="sxs-lookup"><span data-stu-id="27f34-110">Choose **Application policy for Android** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook, for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/b3be3ddd-f683-4073-8d7a-9c639a636a2c.png)
  
### <a name="validate-require-a-pin-or-a-fingerprint-to-access-office-apps"></a><span data-ttu-id="27f34-112">Valider Krev en PIN-kode eller et fingeravtrykk for å få tilgang til Office-apper</span><span class="sxs-lookup"><span data-stu-id="27f34-112">Validate Require a PIN or a fingerprint to access Office apps</span></span>

<span data-ttu-id="27f34-113">Velg **Rediger** ved siden av **Tilgangskontroll for Office-dokumenter**, og utvid **Administrer hvordan brukere får tilgang til Office-filer på mobile enheter** i **Rediger policy**-ruten. Sørg for at **Krever en PIN eller et fingeravtrykk for å få tilgang til Office-apper** er satt til **På**.</span><span class="sxs-lookup"><span data-stu-id="27f34-113">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Kontroller at Krev en PIN-kode eller fingeravtrykk for å få tilgang til Office-apper er satt til På.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="27f34-115">Åpne Outlook I brukerens Android-enhet, og logg deg på med brukerens Microsoft 365 Business-legitimasjon.</span><span class="sxs-lookup"><span data-stu-id="27f34-115">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="27f34-116">Du blir også bedt om å angi en PIN-kode eller bruke et fingeravtrykk.</span><span class="sxs-lookup"><span data-stu-id="27f34-116">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your Android device to access Office apps.](media/9e8ecfee-8122-4a3a-8918-eece80344310.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="27f34-118">Valider Tilbakestill PIN-kode etter et antall mislykkede forsøk</span><span class="sxs-lookup"><span data-stu-id="27f34-118">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="27f34-119">I **redigeringspolicyruten** velger du **Rediger** ved siden av **tilgangskontroll for Office-dokumenter**, utvid Behandle hvordan brukere får tilgang til **Office-filer på mobile enheter,** og kontroller at **Tilbakestill PIN-kode etter antall mislykkede forsøk** er satt til et tall.</span><span class="sxs-lookup"><span data-stu-id="27f34-119">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="27f34-120">Dette er 5 som standard.</span><span class="sxs-lookup"><span data-stu-id="27f34-120">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="27f34-121">Åpne Outlook I brukerens Android-enhet, og logg deg på med brukerens Microsoft 365 Business-legitimasjon.</span><span class="sxs-lookup"><span data-stu-id="27f34-121">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="27f34-122">Skriv inn feil PIN-kode så mange ganger som angitt av policyen.</span><span class="sxs-lookup"><span data-stu-id="27f34-122">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="27f34-123">Du ser en melding som angir **PIN-forsøksgrense nådd** for å tilbakestille PIN-koden.</span><span class="sxs-lookup"><span data-stu-id="27f34-123">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fca6fcb4-bb5c-477f-af5e-5dc937e8b835.png)
  
3. <span data-ttu-id="27f34-125">Trykk på **tilbakestille PIN-kode**.</span><span class="sxs-lookup"><span data-stu-id="27f34-125">Press **Reset PIN**.</span></span> <span data-ttu-id="27f34-126">Du blir bedt om å logge på med brukerens Legitimasjon for Microsoft 365 Business, og deretter kreves for å angi en ny PIN-kode.</span><span class="sxs-lookup"><span data-stu-id="27f34-126">You'll be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="27f34-127">Valider Tving brukere å lagre alle arbeidsfiler til OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="27f34-127">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="27f34-128">Velg **Rediger** ved siden av **Beskyttelse mot tapte eller stjålne enheter** i **Rediger policy**-ruten. Utvid **Beskytt arbeidsfiler når enheter går tapt eller stjålet**, og sørg for at **Tving brukere til å lagre alle arbeidsfiler til OneDrive for Business** er satt til **På**.</span><span class="sxs-lookup"><span data-stu-id="27f34-128">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="27f34-130">Åpne Outlook i brukerens Android-enhet, logg deg på med brukerens Microsoft 365 Business-legitimasjon, og skriv inn en PIN-kode om nødvendig.</span><span class="sxs-lookup"><span data-stu-id="27f34-130">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="27f34-131">Åpne en e-postmelding som inneholder et vedlegg, og trykk på Pil ned-ikonet ved siden av vedleggsinformasjonen.</span><span class="sxs-lookup"><span data-stu-id="27f34-131">Open an email that contains an attachment and tap the down arrow icon next to the attachment's information.</span></span>
    
    ![Tap the down arrow next to an attachment to try to save it.](media/b22573bb-91ce-455f-84fa-8feb2846b117.png)
  
    <span data-ttu-id="27f34-133">Du ser **ikke kan lagre på enheten** nederst på skjermen.</span><span class="sxs-lookup"><span data-stu-id="27f34-133">You'll see **Cannot save to device** on the bottom of the screen.</span></span> 
    
    ![Warning text that indicates cannot save a file locally to an Android.](media/52ca3f3d-7ed0-4a52-9621-4872da6ea9c5.png)
  
    > [!NOTE]
    > <span data-ttu-id="27f34-135">Lagre på OneDrive for Business er for øyeblikket ikke aktivert for Android, slik at du bare ser at lagring lokalt er blokkert.</span><span class="sxs-lookup"><span data-stu-id="27f34-135">Saving to OneDrive for Business is not enabled for Android at this time, so you can only see that saving locally is blocked.</span></span> 
  
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="27f34-136">Valider Krev at brukeren logger på på nytt hvis Office-apper har vært inaktive i et angitt tidsrom</span><span class="sxs-lookup"><span data-stu-id="27f34-136">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="27f34-137">I **redigeringspolicyruten** velger du **Rediger** ved siden av **tilgangskontroll for Office-dokumenter**, utvid Behandle hvordan brukere får tilgang til **Office-filer på mobile enheter,** og kontroller at Det er satt til noen minutter å bruke brukere på nytt etter at **Office-apper er inaktive for,** er satt til et visst antall minutter.</span><span class="sxs-lookup"><span data-stu-id="27f34-137">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="27f34-138">Dette er 30 minutter som standard.</span><span class="sxs-lookup"><span data-stu-id="27f34-138">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="27f34-139">Åpne Outlook i brukerens Android-enhet, logg deg på med brukerens Microsoft 365 Business-legitimasjon, og skriv inn en PIN-kode om nødvendig.</span><span class="sxs-lookup"><span data-stu-id="27f34-139">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="27f34-p105">Du bør nå se innboksen til Outlook. La Android-enheten være uvirksom og urørt i minst 30 minutter (eller en annen tidsperiode, men lengre enn det du spesifiserte i policyen). Enheten vil sannsynligvis tone ned.</span><span class="sxs-lookup"><span data-stu-id="27f34-p105">You should now see Outlook's inbox. Let the Android device idle untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="27f34-143">Få tilgang til Outlook på Android-enheten på nytt.</span><span class="sxs-lookup"><span data-stu-id="27f34-143">Access Outlook on the Android device again.</span></span>
    
4. <span data-ttu-id="27f34-144">Du blir bedt om å angi PIN-koden før du får tilgang til Outlook på nytt.</span><span class="sxs-lookup"><span data-stu-id="27f34-144">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="27f34-145">Valider Beskytt arbeidsfiler med kryptering</span><span class="sxs-lookup"><span data-stu-id="27f34-145">Validate Protect work files with encryption</span></span>

<span data-ttu-id="27f34-146">Velg **Rediger** ved siden av **Beskyttelse mot tapte eller stjålne enheter** i **Rediger policy**-ruten. Utvid **Beskytt arbeidsfiler når enheter går tapt eller stjålet**, og sørg for at **Beskytt arbeidsfiler med kryptering** er satt til **På** og **Tvinge brukere å lagre alle arbeidsfiler til OneDrive for Business** er satt til **Av**.</span><span class="sxs-lookup"><span data-stu-id="27f34-146">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="27f34-147">Åpne Outlook i brukerens Android-enhet, logg deg på med brukerens Microsoft 365 Business-legitimasjon, og skriv inn en PIN-kode om nødvendig.</span><span class="sxs-lookup"><span data-stu-id="27f34-147">In the user's Android device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="27f34-148">Åpne en e-post som inneholder noen bildefilvedlegg.</span><span class="sxs-lookup"><span data-stu-id="27f34-148">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="27f34-149">Trykk på Pil ned-ikonet ved siden av vedleggsinformasjonen for å lagre den.</span><span class="sxs-lookup"><span data-stu-id="27f34-149">Tap the down arrow icon next to the attachment's info to save it.</span></span>
    
    ![Tap the down arrow to save the figure file to the Android device.](media/08a9e21e-4022-45d5-acff-59cface651e7.png)
  
4. <span data-ttu-id="27f34-p106">Du kan bli bedt om å gi Outlook tilgang til bildene, medier og filer på enheten. Trykk på **Tillat**.</span><span class="sxs-lookup"><span data-stu-id="27f34-p106">You may be prompted to allow Outlook to access photos, media, and files on your device. Tap **Allow**.</span></span>
    
5. <span data-ttu-id="27f34-153">Nederst på skjermen kan du velge å **Lagre til enhet** og deretter åpne **Galleri** -appen.</span><span class="sxs-lookup"><span data-stu-id="27f34-153">At the bottom of the screen, choose to **Save to Device** and then open the **Gallery** app.</span></span> 
    
6. <span data-ttu-id="27f34-p107">Du bør nå se et kryptert bilde (eller flere hvis du har lagret flere bildefilvedlegg) i listen. Bildet kan vises på bildelisten som en grå firkant med et hvitt utropstegn inne i en hvit sirkel midt på den grå firkanten.</span><span class="sxs-lookup"><span data-stu-id="27f34-p107">You should see an encrypted photo (or more, if you saved multiple image file attachments) in the list. It may appear in the Pictures list as a gray square with a white exclamation point within a white circle in the center of the gray square.</span></span>
    
    ![An encrypted image file in the Gallery app.](media/25936414-bd7e-421d-824e-6e59b877722d.png)
  
## <a name="ios"></a><span data-ttu-id="27f34-157">Ios</span><span class="sxs-lookup"><span data-stu-id="27f34-157">iOS</span></span>
  
### <a name="check-that-the-app-protection-settings-are-working-on-user-devices"></a><span data-ttu-id="27f34-158">Kontroller at innstillingene for appbeskyttelse fungerer på brukerenheter</span><span class="sxs-lookup"><span data-stu-id="27f34-158">Check that the App protection settings are working on user devices</span></span>

<span data-ttu-id="27f34-159">Når du har [angitt appkonfigurasjoner for iOS-enheter](app-protection-settings-for-android-and-ios.md) for å beskytte apper, kan du følge disse trinnene for å validere at innstillingene du velger, fungerer.</span><span class="sxs-lookup"><span data-stu-id="27f34-159">After you [set app configurations for iOS devices](app-protection-settings-for-android-and-ios.md) to protect apps, you can follow these steps to validate that the settings you chose work.</span></span> 
  
<span data-ttu-id="27f34-160">Først må du kontrollere at policyen gjelder for appen der du skal validere den.</span><span class="sxs-lookup"><span data-stu-id="27f34-160">First, make sure that the policy applies to the app in which you're going to validate it.</span></span>
  
1. <span data-ttu-id="27f34-161">Gå til [Policyer](https://portal.office.com)\*\*\*\*\> i Microsoft 365 Business **-administrasjonssenteret**.</span><span class="sxs-lookup"><span data-stu-id="27f34-161">In the Microsoft 365 Business [admin center](https://portal.office.com), go to **Policies** \> **Edit policy**.</span></span>
    
2. <span data-ttu-id="27f34-162">Velg **Programpolicy for iOS** for innstillingene du opprettet ved installasjonen, eller en annen policy du opprettet, og kontroller at den håndheves for Outlook for eksempel.</span><span class="sxs-lookup"><span data-stu-id="27f34-162">Choose **Application policy for iOS** for the settings you created at setup, or another policy you created, and verify that it's enforced for Outlook for example.</span></span> 
    
    ![Shows all the apps for which this policy protects files.](media/842441b8-e7b1-4b86-9edd-d94d1f77b6f4.png)
  
### <a name="validate-require-a-pin-to-access-office-apps"></a><span data-ttu-id="27f34-164">Valider Krev en PIN-kode å få tilgang til Office-apper</span><span class="sxs-lookup"><span data-stu-id="27f34-164">Validate Require a PIN to access Office apps</span></span>

<span data-ttu-id="27f34-165">Velg **Rediger** ved siden av **Tilgangskontroll for Office-dokumenter**, og utvid **Administrer hvordan brukere får tilgang til Office-filer på mobile enheter** i **Rediger policy**-ruten. Sørg for at **Krever en PIN eller et fingeravtrykk for å få tilgang til Office-apper** er satt til **På**.</span><span class="sxs-lookup"><span data-stu-id="27f34-165">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require a PIN or fingerprint to access Office apps** is set to **On**.</span></span>
  
![Kontroller at Krev en PIN-kode eller fingeravtrykk for å få tilgang til Office-apper er satt til På.](media/f37eb5b2-7e26-49fb-9bd6-d955d196bacf.png)
  
1. <span data-ttu-id="27f34-167">Åpne Outlook i brukerens iOS-enhet, og logg deg på med brukerens Microsoft 365 Business-legitimasjon.</span><span class="sxs-lookup"><span data-stu-id="27f34-167">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="27f34-168">Du blir også bedt om å angi en PIN-kode eller bruke et fingeravtrykk.</span><span class="sxs-lookup"><span data-stu-id="27f34-168">You'll also be prompted to enter a PIN or use a fingerprint.</span></span>
    
    ![Enter a PIN on your IOS device to access Office apps.](media/06fc5cf3-9f19-4090-b23c-14bb59805b7a.png)
  
### <a name="validate-reset-pin-after-number-of-failed-attempts"></a><span data-ttu-id="27f34-170">Valider Tilbakestill PIN-kode etter et antall mislykkede forsøk</span><span class="sxs-lookup"><span data-stu-id="27f34-170">Validate Reset PIN after number of failed attempts</span></span>

<span data-ttu-id="27f34-171">I **redigeringspolicyruten** velger du **Rediger** ved siden av **tilgangskontroll for Office-dokumenter**, utvid Behandle hvordan brukere får tilgang til **Office-filer på mobile enheter,** og kontroller at **Tilbakestill PIN-kode etter antall mislykkede forsøk** er satt til et tall.</span><span class="sxs-lookup"><span data-stu-id="27f34-171">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Reset PIN after number of failed attempts** is set to some number.</span></span> <span data-ttu-id="27f34-172">Dette er 5 som standard.</span><span class="sxs-lookup"><span data-stu-id="27f34-172">This is 5 by default.</span></span> 
  
1. <span data-ttu-id="27f34-173">Åpne Outlook i brukerens iOS-enhet, og logg deg på med brukerens Microsoft 365 Business-legitimasjon.</span><span class="sxs-lookup"><span data-stu-id="27f34-173">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="27f34-174">Skriv inn feil PIN-kode så mange ganger som angitt av policyen.</span><span class="sxs-lookup"><span data-stu-id="27f34-174">Enter an incorrect PIN as many times as specified by the policy.</span></span> <span data-ttu-id="27f34-175">Du ser en melding som angir **PIN-forsøksgrense nådd** for å tilbakestille PIN-koden.</span><span class="sxs-lookup"><span data-stu-id="27f34-175">You'll see a prompt that states **PIN Attempt Limit Reached** to reset the PIN.</span></span> 
    
    ![After too many incorrect PIN attempts, you need to reset your PIN.](media/fab5c089-a4a5-4e8d-8c95-b8eed1dfa262.png)
  
3. <span data-ttu-id="27f34-177">Trykk på **OK**.</span><span class="sxs-lookup"><span data-stu-id="27f34-177">Press **OK**.</span></span> <span data-ttu-id="27f34-178">Du blir bedt om å logge på med brukerens Legitimasjon for Microsoft 365 Business, og deretter kreves for å angi en ny PIN-kode.</span><span class="sxs-lookup"><span data-stu-id="27f34-178">You'll be prompted to sign in with the user's Microsoft 365 Business credentials, and then required to set a new PIN.</span></span>
    
### <a name="validate-force-users-to-save-all-work-files-to-onedrive-for-business"></a><span data-ttu-id="27f34-179">Valider Tving brukere å lagre alle arbeidsfiler til OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="27f34-179">Validate Force users to save all work files to OneDrive for Business</span></span>

<span data-ttu-id="27f34-180">Velg **Rediger** ved siden av **Beskyttelse mot tapte eller stjålne enheter** i **Rediger policy**-ruten. Utvid **Beskytt arbeidsfiler når enheter går tapt eller stjålet**, og sørg for at **Tving brukere til å lagre alle arbeidsfiler til OneDrive for Business** er satt til **På**.</span><span class="sxs-lookup"><span data-stu-id="27f34-180">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Force users to save all work files to OneDrive for Business** is set to **On**.</span></span>
  
![Verify that Force users to save all work files to OneDrive for Business is set to On.](media/7140fa1d-966d-481c-829f-330c06abb5a5.png)
  
1. <span data-ttu-id="27f34-182">Åpne Outlook i brukerens iOS-enhet, logg deg på med brukerens Microsoft 365 Business-legitimasjon, og skriv inn en PIN-kode om nødvendig.</span><span class="sxs-lookup"><span data-stu-id="27f34-182">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="27f34-183">Åpne en e-postmelding som inneholder et vedlegg, åpne vedlegget, og velg **Lagre** nederst på skjermen.</span><span class="sxs-lookup"><span data-stu-id="27f34-183">Open an email that contains an attachment, open the attachment and choose **Save** on the bottom of the screen.</span></span> 
    
    ![Tap the Save option after you open an attachment to try to save it.](media/b419b070-1530-4f14-86a8-8d89933a2b25.png)
  
3. <span data-ttu-id="27f34-185">Du bør nå bare se alternativet for OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="27f34-185">You should only see an option for OneDrive for Business.</span></span> <span data-ttu-id="27f34-186">Hvis ikke, trykker du **Legg til konto** og velger **OneDrive for Business** fra skjermbildet Legg til **lagringskonto.**</span><span class="sxs-lookup"><span data-stu-id="27f34-186">If not, tap **Add Account** and select **OneDrive for Business** from the **Add Storage Account** screen.</span></span> <span data-ttu-id="27f34-187">Angi sluttbrukerens Microsoft 365 Business for å logge på når du blir bedt om det.</span><span class="sxs-lookup"><span data-stu-id="27f34-187">Provide the end user's Microsoft 365 Business to sign in when prompted.</span></span> 
    
    <span data-ttu-id="27f34-188">Trykk på **Lagre**, og velg **OneDrive for Business**.</span><span class="sxs-lookup"><span data-stu-id="27f34-188">Tap **Save** and select **OneDrive for Business**.</span></span>
    
### <a name="validate-require-user-to-sign-in-again-if-office-apps-have-been-idle-for-a-specified-time"></a><span data-ttu-id="27f34-189">Valider Krev at brukeren logger på på nytt hvis Office-apper har vært inaktive i et angitt tidsrom</span><span class="sxs-lookup"><span data-stu-id="27f34-189">Validate Require user to sign in again if Office apps have been idle for a specified time</span></span>

<span data-ttu-id="27f34-190">I **redigeringspolicyruten** velger du **Rediger** ved siden av **tilgangskontroll for Office-dokumenter**, utvid Behandle hvordan brukere får tilgang til **Office-filer på mobile enheter,** og kontroller at Det er satt til noen minutter å bruke brukere på nytt etter at **Office-apper er inaktive for,** er satt til et visst antall minutter.</span><span class="sxs-lookup"><span data-stu-id="27f34-190">In the **Edit policy** pane, choose **Edit** next to **Office documents access control**, expand **Manage how users access Office files on mobile devices**, and make sure that **Require users to sign in again after Office apps have been idle for** is set to some number of minutes.</span></span> <span data-ttu-id="27f34-191">Dette er 30 minutter som standard.</span><span class="sxs-lookup"><span data-stu-id="27f34-191">This is 30 minutes by default.</span></span> 
  
1. <span data-ttu-id="27f34-192">Åpne Outlook i brukerens iOS-enhet, logg deg på med brukerens Microsoft 365 Business-legitimasjon, og skriv inn en PIN-kode om nødvendig.</span><span class="sxs-lookup"><span data-stu-id="27f34-192">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="27f34-p113">Du bør nå se innboksen til Outlook. La iOS-enheten være uberørt i minst 30 minutter (eller en annen tidsperiode, men lengre enn det du spesifiserte i policyen). Enheten vil sannsynligvis tone ned.</span><span class="sxs-lookup"><span data-stu-id="27f34-p113">You should now see Outlook's inbox. Let the iOS device untouched for at least 30 minutes (or some other amount of time, longer than what you specified in the policy). The device will likely dim.</span></span>
    
3. <span data-ttu-id="27f34-196">Få tilgang til Outlook på iOS-enheten på nytt.</span><span class="sxs-lookup"><span data-stu-id="27f34-196">Access Outlook on the iOS device again.</span></span>
    
4. <span data-ttu-id="27f34-197">Du blir bedt om å angi PIN-koden før du får tilgang til Outlook på nytt.</span><span class="sxs-lookup"><span data-stu-id="27f34-197">You'll be prompted to enter your PIN before you can access Outlook again.</span></span>
    
### <a name="validate-protect-work-files-with-encryption"></a><span data-ttu-id="27f34-198">Valider Beskytt arbeidsfiler med kryptering</span><span class="sxs-lookup"><span data-stu-id="27f34-198">Validate Protect work files with encryption</span></span>

<span data-ttu-id="27f34-199">Velg **Rediger** ved siden av **Beskyttelse mot tapte eller stjålne enheter** i **Rediger policy**-ruten. Utvid **Beskytt arbeidsfiler når enheter går tapt eller stjålet**, og sørg for at **Beskytt arbeidsfiler med kryptering** er satt til **På** og **Tvinge brukere å lagre alle arbeidsfiler til OneDrive for Business** er satt til **Av**.</span><span class="sxs-lookup"><span data-stu-id="27f34-199">In the **Edit policy** pane, choose **Edit** next to **Protection against lost or stolen devices**, expand **Protect work files when devices are lost or stolen**, and make sure that **Protect work files with encryption** is set to **On**, and **Force users to save all work files to OneDrive for Business** is set to **Off**.</span></span>
  
1. <span data-ttu-id="27f34-200">Åpne Outlook i brukerens iOS-enhet, logg deg på med brukerens Microsoft 365 Business-legitimasjon, og skriv inn en PIN-kode om nødvendig.</span><span class="sxs-lookup"><span data-stu-id="27f34-200">In the user's iOS device, open Outlook and sign in with the user's Microsoft 365 Business credentials, and enter a PIN if requested.</span></span>
    
2. <span data-ttu-id="27f34-201">Åpne en e-post som inneholder noen bildefilvedlegg.</span><span class="sxs-lookup"><span data-stu-id="27f34-201">Open an email that contains a few image file attachments.</span></span>
    
3. <span data-ttu-id="27f34-202">Trykk på vedlegget, og trykk deretter på **Lagre**-alternativet under vedlegget.</span><span class="sxs-lookup"><span data-stu-id="27f34-202">Tap the attachment and then tap the **Save** option under it.</span></span> 
    
4. <span data-ttu-id="27f34-p114">Åpne **Bilde**-appen på startskjermen. Du bør nå se et kryptert bilde (eller flere hvis du har lagret flere bildefilvedlegg) som er lagret, men kryptert.</span><span class="sxs-lookup"><span data-stu-id="27f34-p114">Open **Photos** app from the home screen. You should see an encrypted photo (or more, if you saved multiple image file attachments) saved, but encrypted.</span></span> 
    
---

