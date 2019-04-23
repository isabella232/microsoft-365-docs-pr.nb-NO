---
title: Angi innstillinger for appbeskyttelse, for Android- eller iOS-enheter
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6f2b80b4-81c3-4714-a7bc-ae69313e8a33
description: Lær hvordan du kan opprette, redigere, eller slette en policy for informasjonsbehandling av app og beskytte arbeidsfiler på Android eller iOS enheter.
ms.openlocfilehash: e81ff8a4bd71dbbbf7ccc31249d450e03f4bd241
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277459"
---
# <a name="set-app-protection-settings-for-android-or-ios-devices"></a><span data-ttu-id="b03d1-103">Angi innstillinger for appbeskyttelse, for Android- eller iOS-enheter</span><span class="sxs-lookup"><span data-stu-id="b03d1-103">Set app protection settings for Android or iOS devices</span></span>

## <a name="create-an-app-management-policy"></a><span data-ttu-id="b03d1-104">Opprette en policy for appbehandling</span><span class="sxs-lookup"><span data-stu-id="b03d1-104">Create an app management policy</span></span>

1. <span data-ttu-id="b03d1-105">Logg på [administrasjonssenteret for Microsoft 365 Business](https://go.microsoft.com/fwlink/p/?linkid=837890) med global admin-legitimasjon.</span><span class="sxs-lookup"><span data-stu-id="b03d1-105">Sign in to [Microsoft 365 Business admin center ](https://go.microsoft.com/fwlink/p/?linkid=837890) with global admin credentials.</span></span> 
    
2. <span data-ttu-id="b03d1-106">Velg **enheter** i administrasjonssenteret, \> **policyer** \> **Legg til policyen**.</span><span class="sxs-lookup"><span data-stu-id="b03d1-106">In the admin center, choose **Devices** \> **Policies** \> **Add policy**.</span></span>
  
3. <span data-ttu-id="b03d1-107">Angi et unikt navn for denne policyen på **Legg til policy**-ruten.</span><span class="sxs-lookup"><span data-stu-id="b03d1-107">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="b03d1-108">Velg **Programbehandling for Android** eller **Programbehandling for iOS** under **Policytype**, avhengig av hvilke sett med policyer du vil opprette.</span><span class="sxs-lookup"><span data-stu-id="b03d1-108">Under **Policy type**, choose **Application Management for Android** or **Application Management for iOS** depending on which set of policies you want to create.</span></span> 
    
5. <span data-ttu-id="b03d1-109">Utvid **Beskytt arbeidsfiler når enheter går tapt eller blir stjålet** og **Behandle hvordan brukere får tilgang til Office-filer på mobilenheter** \> konfigurer innstillingene slik du ønsker.</span><span class="sxs-lookup"><span data-stu-id="b03d1-109">Expand **Protect work files when devices are lost or stolen** and **Manage how users access Office files on mobile devices** \> configure the settings how you would like.</span></span> <span data-ttu-id="b03d1-110">**Administrer hvordan brukere får tilgang til Office-filer på mobilenheter** er slått **Av** som standard, men det anbefales at du slår den **På** og godtar standardverdiene.</span><span class="sxs-lookup"><span data-stu-id="b03d1-110">The **Manage how users access Office files on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="b03d1-111">Hvis du vil ha mer informasjon, kan du se [tilgjengelige innstillinger](#available-settings) .</span><span class="sxs-lookup"><span data-stu-id="b03d1-111">See [Available settings](#available-settings)  for more information.</span></span> 
    
    <span data-ttu-id="b03d1-112">Du kan til enhver tid bruke **Tilbakestill standardinnstillinger**-koblingen for å gå tilbake til standardinnstillingen.</span><span class="sxs-lookup"><span data-stu-id="b03d1-112">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
    ![Screenshot of Create a policy with Application management for Android selected](media/eabbe06d-ac0a-4f3a-8630-68c808b1e662.png)
  
6. <span data-ttu-id="b03d1-p102">Bestem deretter **Hvem får disse innstillingene?** Hvis du ikke vil bruke den standard sikkerhetsgruppen **Alle brukere**, velger du **Endre**, og velg så sikkerhetsgruppene som vil få disse innstillingene \> **Velg**.</span><span class="sxs-lookup"><span data-stu-id="b03d1-p102">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
7. <span data-ttu-id="b03d1-116">Velg til slutt **Ferdig** for å lagre policyen og tilordne den til enhetene.</span><span class="sxs-lookup"><span data-stu-id="b03d1-116">Finally, choose **Done** to save the policy, and assign it to devices.</span></span> 
    
## <a name="edit-an-app-management-policy"></a><span data-ttu-id="b03d1-117">Endre en policy for appbehandling</span><span class="sxs-lookup"><span data-stu-id="b03d1-117">Edit an app management policy</span></span>

1. <span data-ttu-id="b03d1-118">Velg **Rediger policy**på kortet **policyer** .</span><span class="sxs-lookup"><span data-stu-id="b03d1-118">On the **Policies** card, choose **Edit policy**.</span></span>
    
2. <span data-ttu-id="b03d1-119">Velg policyen du vil endre, på **Rediger policy**-ruten</span><span class="sxs-lookup"><span data-stu-id="b03d1-119">On the **Edit policy** pane, choose the policy you want to change</span></span> 
    
3. <span data-ttu-id="b03d1-p103">Velg **Rediger** ved siden av hver innstilling for å endre verdiene i policyen. Når du endrer en verdi, lagres den automatisk i policyen</span><span class="sxs-lookup"><span data-stu-id="b03d1-p103">Choose **Edit** next to each setting to change the values in the policy. When you change a value, it is automatically saved into the policy</span></span> 
    
4. <span data-ttu-id="b03d1-122">Lukk **Rediger policy**-ruten når du er ferdig.</span><span class="sxs-lookup"><span data-stu-id="b03d1-122">When you are finished, close the **Edit policy** pane.</span></span> 
    
## <a name="delete-an-app-management-policy"></a><span data-ttu-id="b03d1-123">Slette en policy for appbehandling</span><span class="sxs-lookup"><span data-stu-id="b03d1-123">Delete an app management policy</span></span>

1. <span data-ttu-id="b03d1-124">Velg **Slette policy** på **Policyer**-kortet.</span><span class="sxs-lookup"><span data-stu-id="b03d1-124">On the **Policies** card, choose **Delete policy**.</span></span>
    
2. <span data-ttu-id="b03d1-125">Velg den policyen du ønsker å slette, på **Slett policy**-ruten \> **Velg**, deretter **Bekreft** for å slette policyen du valgte.</span><span class="sxs-lookup"><span data-stu-id="b03d1-125">On the **Delete policy** pane, choose the policies you want to delete \> **Select**, then **Confirm** to delete the policy or policies you chose.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="b03d1-126">Tilgjengelige innstillinger</span><span class="sxs-lookup"><span data-stu-id="b03d1-126">Available settings</span></span>

<span data-ttu-id="b03d1-127">Tabellene nedenfor gir detaljert informasjon om de tilgjengelige innstillingene for å beskytte arbeidsfiler på enheter, samt innstillingene som kontrollerer hvordan brukere får tilgang til Office-filer fra de mobile enhetene.</span><span class="sxs-lookup"><span data-stu-id="b03d1-127">The following tables give detailed information about the available settings to protect work files on devices and the settings that control how users access Office files from their mobile devices.</span></span>
  
 <span data-ttu-id="b03d1-128">Se [Hvordan tilordnes beskyttelsesfunksjoner i Microsoft 365 Business til Intune-innstillinger](map-protection-features-to-intune-settings.md) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="b03d1-128">See [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md) for more information.</span></span> 
  
### <a name="settings-that-protect-work-files"></a><span data-ttu-id="b03d1-129">Innstillinger som beskytter arbeidsfiler</span><span class="sxs-lookup"><span data-stu-id="b03d1-129">Settings that protect work files</span></span>

<span data-ttu-id="b03d1-130">Følgende innstillinger er tilgjengelig for å beskytte arbeidsfiler hvis en brukers enhet mistes eller blir stjålet:</span><span class="sxs-lookup"><span data-stu-id="b03d1-130">The following settings are available to protect work files if a user's device is lost or stolen:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="b03d1-131">Innstilling</span><span class="sxs-lookup"><span data-stu-id="b03d1-131">Setting</span></span>  <br/> |<span data-ttu-id="b03d1-132">Beskrivelse</span><span class="sxs-lookup"><span data-stu-id="b03d1-132">Description</span></span>  <br/> |
|<span data-ttu-id="b03d1-133">Slette arbeidsfiler fra en inaktiv enhet etter et visst antall dager</span><span class="sxs-lookup"><span data-stu-id="b03d1-133">Delete work files from an inactive device after this many days</span></span>  <br/> |<span data-ttu-id="b03d1-134">Hvis en enhet ikke er blitt brukt for det antallet dager som du spesifiserer her, vil eventuelle arbeidsfiler som er lagret på enheten, automatisk bli slettet.</span><span class="sxs-lookup"><span data-stu-id="b03d1-134">If a device is not used for the number of days that you specify here, any work files stored on the device will automatically be deleted.</span></span>  <br/> |
|<span data-ttu-id="b03d1-135">Tvinge brukere til å lagre alle arbeidsfiler til OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="b03d1-135">Force users to save all work files to OneDrive for Business</span></span>  <br/> |<span data-ttu-id="b03d1-136">Hvis denne innstillingen er **På**, vil den eneste tilgjengelige lagringsplasseringen for arbeidsfiler være OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="b03d1-136">If this setting is **On**, the only available save location for work files will be OneDrive for Business.</span></span>  <br/> |
|<span data-ttu-id="b03d1-137">Kryptere arbeidsfiler</span><span class="sxs-lookup"><span data-stu-id="b03d1-137">Encrypt work files</span></span>  <br/> |<span data-ttu-id="b03d1-p104">Behold denne innstillingen **På** slik at arbeidsfiler er beskyttet ved hjelp av kryptering. Selv om enheten mistes eller blir stjålet, vil ingen kunne lese firmadataene.  </span><span class="sxs-lookup"><span data-stu-id="b03d1-p104">Keep this setting **On** so that work files are protected by encryption. Even if the device is lost or stolen, no one will be able to read your company data.  </span></span><br/> |
   
### <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="b03d1-140">Innstillinger som kontrollerer hvordan brukere får tilgang til Office-filer på mobile enheter</span><span class="sxs-lookup"><span data-stu-id="b03d1-140">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="b03d1-141">Følgende innstillinger er tilgjengelig for å styre hvordan brukere får tilgang til Office-arbeidsfiler:</span><span class="sxs-lookup"><span data-stu-id="b03d1-141">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="b03d1-142">Innstilling</span><span class="sxs-lookup"><span data-stu-id="b03d1-142">Setting</span></span>  <br/> |<span data-ttu-id="b03d1-143">Beskrivelse</span><span class="sxs-lookup"><span data-stu-id="b03d1-143">Description</span></span>  <br/> |
|<span data-ttu-id="b03d1-144">Kreve en PIN-kode eller et fingeravtrykk for å få tilgang til Office-apper</span><span class="sxs-lookup"><span data-stu-id="b03d1-144">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="b03d1-145">Hvis disse innstillingene er **På**, må brukere gi en annen form for godkjenning, i tillegg til brukernavn og passord, før de kan bruke Office-apper på mobilenheten.</span><span class="sxs-lookup"><span data-stu-id="b03d1-145">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="b03d1-146">Tilbakestille PIN-kode når påloggingen mislykkes et visst antall ganger</span><span class="sxs-lookup"><span data-stu-id="b03d1-146">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="b03d1-147">Hvis du vil forhindre at en uautorisert bruker tilfeldig gjetter en PIN-kode, tilbakestilles PIN-koden etter det antallet feiloppføringer du angir.</span><span class="sxs-lookup"><span data-stu-id="b03d1-147">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="b03d1-148">Kreve at brukere logger seg på igjen etter at Office-apper har vært inaktive i</span><span class="sxs-lookup"><span data-stu-id="b03d1-148">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="b03d1-149">Denne innstillingen bestemmer hvor lenge en bruker kan være inaktiv før de blir bedt om å logge seg på igjen.</span><span class="sxs-lookup"><span data-stu-id="b03d1-149">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="b03d1-150">Avslå tilgang til arbeidsfiler på enheter der programvarebegrensningene er fjernet, eller enheter som har blitt utsatt for utiltenkt rottilgang</span><span class="sxs-lookup"><span data-stu-id="b03d1-150">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="b03d1-p105">Smarte brukere har kanskje en enhet der programvarebegrensningene er fjernet, eller en enhet som har blitt utsatt for utiltenkt rottilgang. Dette betyr at brukeren kan endre operativsystemet, noe som kan gjøre enheten mer utsatt for skadelig programvare. Disse enhetene blokkeres når denne innstillingen er **På**.  </span><span class="sxs-lookup"><span data-stu-id="b03d1-p105">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="b03d1-154">Tillate brukere å kopiere innhold fra Office-apper til personlige apper</span><span class="sxs-lookup"><span data-stu-id="b03d1-154">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="b03d1-155">Vi tillater dette som standard, men hvis innstillingen er satt til **På**, vil brukeren kunne kopiere informasjon fra en arbeidsfil til en personlig fil.</span><span class="sxs-lookup"><span data-stu-id="b03d1-155">We do allow this by default, but if the setting is **On**, the user could copy information in a work file to a personal file.</span></span> <span data-ttu-id="b03d1-156">Hvis innstillingen er **Av**, kan ikke brukeren kopiere informasjon fra en jobbkonto til en personlig app eller personlig konto.</span><span class="sxs-lookup"><span data-stu-id="b03d1-156">If the setting is **Off**, the user will be unable to copy information from a work account into a personal app or personal account.</span></span>  <br/> |
   

  

