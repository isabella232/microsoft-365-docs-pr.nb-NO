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
ms.openlocfilehash: 92dce1e8761e53b85df85f2a84f30ab307f63e6d
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925067"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="c5c4f-103">Angi innstillinger for appbeskyttelse, for Android- eller iOS-enheter</span><span class="sxs-lookup"><span data-stu-id="c5c4f-103">Set app protection settings for Android or iOS devices</span></span>

<span data-ttu-id="c5c4f-104">Denne artikkelen gjelder for Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="create-an-app-management-policy"></a><span data-ttu-id="c5c4f-105">Opprette en policy for appbehandling</span><span class="sxs-lookup"><span data-stu-id="c5c4f-105">Create an app management policy</span></span>

1. <span data-ttu-id="c5c4f-106">Gå til administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="c5c4f-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
    
2. <span data-ttu-id="c5c4f-107">Velg Legg til  enheter policyer i det venstre \>  \> **navigasjonsfeltet.**</span><span class="sxs-lookup"><span data-stu-id="c5c4f-107">In the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
  
3. <span data-ttu-id="c5c4f-108">Angi et unikt navn for denne policyen på **Legg til policy**-ruten.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-108">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="c5c4f-109">Velg **Programbehandling** **for Android** eller **Programbehandling for iOS** under Policytype , avhengig av hvilket sett med policyer du vil opprette.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-109">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS**, depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="c5c4f-110">Utvid **Beskytt arbeidsfiler når enheter går tapt eller blir** stjålet og Administrer hvordan brukere får tilgang til **Office-filer på mobile enheter.**</span><span class="sxs-lookup"><span data-stu-id="c5c4f-110">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices**.</span></span> <span data-ttu-id="c5c4f-111">Konfigurer innstillingene slik du ønsker.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-111">Configure the settings how you would like.</span></span> <span data-ttu-id="c5c4f-112">**Administrer hvordan brukere får tilgang til Office-filer** på mobile enheter  er Av **som** standard, men vi anbefaler at du slår den på og godtar standardverdiene.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-112">**Manage how users access Office files on mobile devices** is **Off** by default, but we recommend that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="c5c4f-113">Hvis du vil ha mer informasjon, kan [du se Tilgjengelige innstillinger](#available-settings).</span><span class="sxs-lookup"><span data-stu-id="c5c4f-113">For more information, see [Available settings](#available-settings).</span></span> 
    
    <span data-ttu-id="c5c4f-114">Du kan til enhver tid bruke **Tilbakestill standardinnstillinger**-koblingen for å gå tilbake til standardinnstillingen.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-114">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](../media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="c5c4f-116">Bestem deretter **Hvem får disse innstillingene?**</span><span class="sxs-lookup"><span data-stu-id="c5c4f-116">Next decide **Who will get these settings?**</span></span> <span data-ttu-id="c5c4f-117">Hvis du ikke vil bruke standard sikkerhetsgruppe **for** alle brukere, velger du Endre **,** velger sikkerhetsgruppene som får disse innstillingene \> **Velg**.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-117">If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups that get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="c5c4f-118">Velg til slutt **Ferdig** for å lagre policyen og tilordne den til enhetene.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-118">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="c5c4f-119">Endre en policy for appbehandling</span><span class="sxs-lookup"><span data-stu-id="c5c4f-119">Edit an app management policy</span></span>

1. <span data-ttu-id="c5c4f-120">Velg Rediger **policy** på **Policyer-kortet.**</span><span class="sxs-lookup"><span data-stu-id="c5c4f-120">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="c5c4f-121">Velg policyen du vil endre, på **Rediger policy**-ruten</span><span class="sxs-lookup"><span data-stu-id="c5c4f-121">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="c5c4f-122">Velg **Rediger** ved siden av hver innstilling for å endre verdiene i policyen.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-122">Choose **Edit** next to each setting to change the values in the policy.</span></span> <span data-ttu-id="c5c4f-123">Når du endrer en verdi, lagres den automatisk i policyen.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-123">When you change a value, it's automatically saved in the policy.</span></span>
    
4. <span data-ttu-id="c5c4f-124">Når du er ferdig, lukker du **Rediger policy-ruten.**</span><span class="sxs-lookup"><span data-stu-id="c5c4f-124">When you're finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="c5c4f-125">Slette en policy for appbehandling</span><span class="sxs-lookup"><span data-stu-id="c5c4f-125">Delete an app management policy</span></span>

1. <span data-ttu-id="c5c4f-126">Velg en **policy** på Policyer-siden, og velg deretter **Slett**.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-126">On the **Policies** page, choose a policy and then **Delete**.</span></span>
    
2. <span data-ttu-id="c5c4f-127">Velg **Bekreft i** Slett policy-ruten **for** å slette policyen eller policyene du valgte.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-127">On the **Delete policy** pane, choose **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="c5c4f-128">Tilgjengelige innstillinger</span><span class="sxs-lookup"><span data-stu-id="c5c4f-128">Available settings</span></span>

<span data-ttu-id="c5c4f-129">Tabellene nedenfor gir detaljert informasjon om innstillinger som er tilgjengelige for å beskytte arbeidsfiler på enheter og innstillingene som styrer hvordan brukere får tilgang til Office-filer fra sine mobile enheter.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-129">The following tables give detailed information about settings available to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="c5c4f-130">Hvis du vil ha mer informasjon, kan du se [Hvordan fungerer beskyttelsesfunksjoner i Microsoft 365 Business Premium-kart til Intune-innstillinger](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="c5c4f-130">For more information, see [How do protection features in Microsoft 365 Business Premium map to Intune settings](map-protection-features-to-intune-settings.md).</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="c5c4f-131">Innstillinger som beskytter arbeidsfiler</span><span class="sxs-lookup"><span data-stu-id="c5c4f-131">Settings that protect work files</span></span>

<span data-ttu-id="c5c4f-132">Følgende innstillinger er tilgjengelig for å beskytte arbeidsfiler hvis en brukers enhet mistes eller blir stjålet:</span><span class="sxs-lookup"><span data-stu-id="c5c4f-132">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>


|<span data-ttu-id="c5c4f-133">Innstilling</span><span class="sxs-lookup"><span data-stu-id="c5c4f-133">Setting</span></span>  <br/> |<span data-ttu-id="c5c4f-134">Beskrivelse</span><span class="sxs-lookup"><span data-stu-id="c5c4f-134">Description</span></span>  <br/> |
|:-----|:-----|
|<span data-ttu-id="c5c4f-135">Slette arbeidsfiler fra en inaktiv enhet etter et visst antall dager</span><span class="sxs-lookup"><span data-stu-id="c5c4f-135">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="c5c4f-136">Hvis en enhet ikke brukes for antall dager du angir her, slettes alle arbeidsfiler som er lagret på enheten, automatisk.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-136">If a device isn't used for the number of days that you specify here, any work files stored on the device will be deleted automatically.</span></span>  <br/> |
|<span data-ttu-id="c5c4f-137">Tvinge brukere til å lagre alle arbeidsfiler til OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="c5c4f-137">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="c5c4f-138">Hvis denne innstillingen er **På**, er den eneste tilgjengelige lagringsplasseringsplasseringen for arbeidsfiler OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-138">If this setting is **On**, the only available save location for work files is OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="c5c4f-139">Kryptere arbeidsfiler</span><span class="sxs-lookup"><span data-stu-id="c5c4f-139">Encrypt work files</span></span>  <br/> |<span data-ttu-id="c5c4f-140">Behold denne innstillingen **På** slik at arbeidsfiler er beskyttet ved hjelp av kryptering.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-140">Keep this setting **On** so that work files are protected by encryption.</span></span> <span data-ttu-id="c5c4f-141">Selv om enheten er mistet eller stjålet, kan ingen lese firmadataene dine.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-141">Even if the device is lost or stolen, no one can read your company data.</span></span>  <br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="c5c4f-142">Innstillinger som kontrollerer hvordan brukere får tilgang til Office-filer på mobile enheter</span><span class="sxs-lookup"><span data-stu-id="c5c4f-142">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="c5c4f-143">Følgende innstillinger er tilgjengelig for å styre hvordan brukere får tilgang til Office-arbeidsfiler:</span><span class="sxs-lookup"><span data-stu-id="c5c4f-143">The following settings are available to manage how users access Office work files:</span></span>


|<span data-ttu-id="c5c4f-144">Innstilling</span><span class="sxs-lookup"><span data-stu-id="c5c4f-144">Setting</span></span>  <br/> |<span data-ttu-id="c5c4f-145">Beskrivelse</span><span class="sxs-lookup"><span data-stu-id="c5c4f-145">Description</span></span>  <br/> |
|:-----|:-----|
|<span data-ttu-id="c5c4f-146">Kreve en PIN-kode eller et fingeravtrykk for å få tilgang til Office-apper</span><span class="sxs-lookup"><span data-stu-id="c5c4f-146">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="c5c4f-147">Hvis denne  innstillingen er På-brukere, må de oppgi en annen form for godkjenning, i tillegg til brukernavn og passord, før de kan bruke Office-apper på sine mobile enheter.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-147">If this setting is **On** users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile devices.</span></span><br/> |
|<span data-ttu-id="c5c4f-148">Tilbakestille PIN-kode når påloggingen mislykkes et visst antall ganger</span><span class="sxs-lookup"><span data-stu-id="c5c4f-148">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="c5c4f-149">Hvis du vil forhindre at en uautorisert bruker tilfeldig gjetter en PIN-kode, tilbakestilles PIN-koden etter det antallet feiloppføringer du angir.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-149">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="c5c4f-150">Kreve at brukere logger seg på igjen etter at Office-apper har vært inaktive i</span><span class="sxs-lookup"><span data-stu-id="c5c4f-150">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="c5c4f-151">Denne innstillingen bestemmer hvor lenge en bruker kan være inaktiv før de blir bedt om å logge på igjen.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-151">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="c5c4f-152">Avslå tilgang til arbeidsfiler på enheter der programvarebegrensningene er fjernet, eller enheter som har blitt utsatt for utiltenkt rottilgang</span><span class="sxs-lookup"><span data-stu-id="c5c4f-152">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="c5c4f-p105">Smarte brukere har kanskje en enhet der programvarebegrensningene er fjernet, eller en enhet som har blitt utsatt for utiltenkt rottilgang. Dette betyr at brukeren kan endre operativsystemet, noe som kan gjøre enheten mer utsatt for skadelig programvare. Disse enhetene blokkeres når denne innstillingen er **På**.  </span><span class="sxs-lookup"><span data-stu-id="c5c4f-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="c5c4f-156">Ikke tillat brukere å kopiere innhold fra Office-apper til personlige apper</span><span class="sxs-lookup"><span data-stu-id="c5c4f-156">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="c5c4f-157">Vi tillater dette som standard, men hvis innstillingen er satt til **På**, vil brukeren kunne kopiere informasjon fra en arbeidsfil til en personlig fil.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-157">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="c5c4f-158">Hvis innstillingen er **Av**, kan ikke brukeren kopiere informasjon fra en jobbkonto til en personlig app eller personlig konto.</span><span class="sxs-lookup"><span data-stu-id="c5c4f-158">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
