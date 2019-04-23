---
title: Angi innstillinger for programbeskyttelse for Windows 10-enheter
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Lær hvordan du oppretter en policy for informasjonsbehandling av app og beskytte arbeidsfiler på Windows 10 enheter.
ms.openlocfilehash: 289c6a74f6ccb53f6a833612a7b4a5bcddd3ea56
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32278188"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="f1db8-103">Angi innstillinger for programbeskyttelse for Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="f1db8-103">Set application protection settings for Windows 10 devices</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="f1db8-104">Opprette en policy for appbehandling for Windows 10</span><span class="sxs-lookup"><span data-stu-id="f1db8-104">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="f1db8-105">Hvis brukerne har personlige Windows 10-enheter der de utfører arbeidsoppgaver, kan du beskytte dataene dine på disse enhetene i tillegg.</span><span class="sxs-lookup"><span data-stu-id="f1db8-105">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="f1db8-106">Logg på [administrasjonssenteret](https://go.microsoft.com/fwlink/p/?linkid=837890) med global admin-legitimasjon.</span><span class="sxs-lookup"><span data-stu-id="f1db8-106">Sign in to [admin center](https://go.microsoft.com/fwlink/p/?linkid=837890) with global admin credentials.</span></span> <span data-ttu-id="f1db8-107">Velg **Administrasjon**-flisen for å gå til administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="f1db8-107">Choose the **Admin** tile to go to the admin center.</span></span> 
    
2. <span data-ttu-id="f1db8-108">Velg **enheter** på venstre nav, \> **policyer** \> **Legg til**.</span><span class="sxs-lookup"><span data-stu-id="f1db8-108">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>

3. <span data-ttu-id="f1db8-109">Angi et unikt navn for denne policyen i **Legg til Policy**-ruten.</span><span class="sxs-lookup"><span data-stu-id="f1db8-109">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
    
4. <span data-ttu-id="f1db8-110">Velg **Programbehandling for Windows 10** under **Policytype**.</span><span class="sxs-lookup"><span data-stu-id="f1db8-110">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
    
5. <span data-ttu-id="f1db8-111">Under \*\* Device type \*\*, choose either **Personal** or **Company Owned**.</span><span class="sxs-lookup"><span data-stu-id="f1db8-111">Under \*\* Device type \*\*, choose either **Personal** or **Company Owned**.</span></span>
    
6. <span data-ttu-id="f1db8-112">**Krypter arbeidsfiler** aktiveres automatisk.</span><span class="sxs-lookup"><span data-stu-id="f1db8-112">The **Encrypt work files** is turned on automatically.</span></span> 
    
7. <span data-ttu-id="f1db8-113">Sett **Forhindre brukere fra å kopiere bedriftsdata til personlige filer, og tvinge dem til å lagre arbeidsfiler til OneDrive for Business** til **På** hvis du ikke vil at brukerne skal lagre arbeidsfiler på PCen.</span><span class="sxs-lookup"><span data-stu-id="f1db8-113">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
    
8. <span data-ttu-id="f1db8-114">Utvid **Administrer hvordan brukere får tilgang til Office-filer på enheter** \> konfigurer innstillingene slik du ønsker.</span><span class="sxs-lookup"><span data-stu-id="f1db8-114">Expand **Manage how users access Office files on devices** \> configure the settings how you would like.</span></span> <span data-ttu-id="f1db8-115">**Administrer hvordan brukere får tilgang til Office-enheter på mobile enheter** er slått **Av** som standard, men det anbefales at du slår den **På** og godtar standardverdiene.</span><span class="sxs-lookup"><span data-stu-id="f1db8-115">The **Manage how users access Office devices on mobile devices** is **Off** by default, but it is recommended that you turn it **On** and accept the default values.</span></span> <span data-ttu-id="f1db8-116">Hvis du vil ha mer informasjon, kan du se [tilgjengelige innstillinger](#available-settings).</span><span class="sxs-lookup"><span data-stu-id="f1db8-116">See [Available settings](#available-settings)for more information.</span></span> 
    
    <span data-ttu-id="f1db8-117">Du kan til enhver tid bruke **Tilbakestill standardinnstillinger**-koblingen for å gå tilbake til standardinnstillingen.</span><span class="sxs-lookup"><span data-stu-id="f1db8-117">You can always use the **Reset default settings** link to return to the default setting.</span></span> 
    
9. <span data-ttu-id="f1db8-118">Utvid **Gjenopprett data på Windows-enheter**, og det anbefales også at du slår den **På**.</span><span class="sxs-lookup"><span data-stu-id="f1db8-118">Expand **Recover data on Windows devices** and it is recommended that you turn it **On**.</span></span>
    
    <span data-ttu-id="f1db8-p103">Før du kan bla til plasseringen av Sertifikatet for datagjenopprettingsagent, må du først opprette ett. For nærmere instruksjoner kan du se [Opprett og bekreft et sertifikat for datagjenopprettingsagent for EFS (Encrypting File System)](https://go.microsoft.com/fwlink/p/?linkid=853700).</span><span class="sxs-lookup"><span data-stu-id="f1db8-p103">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one. For instructions see, [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](https://go.microsoft.com/fwlink/p/?linkid=853700).</span></span>
    
    <span data-ttu-id="f1db8-p104">Som standard blir arbeidsfiler kryptert ved hjelp av en hemmelig nøkkel som er lagret på enheten og knyttet til brukerens profil. Bare brukeren kan åpne og dekryptere filen. Men hvis en enhet mistes eller en bruker fjernes, kan en fil bli sittende fast i en kryptert tilstand. En administrator kan bruke sertifikatet for datagjenopprettingsagenten til å dekryptere filen.</span><span class="sxs-lookup"><span data-stu-id="f1db8-p104">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile. Only the user can open and decrypt the file. However, if a device is lost or a user is removed, a file can be stuck in an encrypted state. The Data Recovery Agent (DRA) certificate can be used by an admin to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="f1db8-p105">Utvid **Beskytt ekstra nettverk og skyplasseringer** hvis du vil legge til flere domener eller SharePoint Online-områder, for å sikre at filene i alle oppførte apper blir beskyttet. Hvis du trenger å angi mer enn ett element for hvert felt, kan du bruke semikolon (;) mellom elementene.</span><span class="sxs-lookup"><span data-stu-id="f1db8-p105">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps will be protected. If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span> 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="f1db8-p106">Bestem deretter **Hvem får disse innstillingene?** Hvis du ikke vil bruke den standard sikkerhetsgruppen **Alle brukere**, velger du **Endre** og deretter sikkerhetsgruppene som vil få disse innstillingene \> **Velg**.</span><span class="sxs-lookup"><span data-stu-id="f1db8-p106">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
    
12. <span data-ttu-id="f1db8-131">Velg til slutt **Legg til** for å lagre policyen og tilordne den til enhetene.</span><span class="sxs-lookup"><span data-stu-id="f1db8-131">Finally, choose **Add** to save the policy, and assign it to devices.</span></span> 
    
## <a name="available-settings"></a><span data-ttu-id="f1db8-132">Tilgjengelige innstillinger</span><span class="sxs-lookup"><span data-stu-id="f1db8-132">Available settings</span></span>

<span data-ttu-id="f1db8-133">De følgende innstillingene er tilgjengelige for å administrere hvordan brukere får tilgang til Office-arbeidsfiler.</span><span class="sxs-lookup"><span data-stu-id="f1db8-133">The following settings are available to manage how users access Office work files.</span></span>
  
<span data-ttu-id="f1db8-134">Hvis du vil ha mer informasjon, kan du se [Slik tilordnes beskyttelsesfunksjoner i Microsoft 365 Business til Intune-innstillinger](map-protection-features-to-intune-settings.md).</span><span class="sxs-lookup"><span data-stu-id="f1db8-134">For more information, see [How do protection features in Microsoft 365 Business map to Intune settings](map-protection-features-to-intune-settings.md).</span></span>
  
|<span data-ttu-id="f1db8-135">**Innstilling**</span><span class="sxs-lookup"><span data-stu-id="f1db8-135">**Setting**</span></span>|<span data-ttu-id="f1db8-136">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="f1db8-136">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f1db8-137">Kreve en PIN-kode eller et fingeravtrykk for å få tilgang til Office-apper</span><span class="sxs-lookup"><span data-stu-id="f1db8-137">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="f1db8-138">Hvis disse innstillingene er **På**, må brukere gi en annen form for godkjenning, i tillegg til brukernavn og passord, før de kan bruke Office-apper på mobilenheten.</span><span class="sxs-lookup"><span data-stu-id="f1db8-138">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="f1db8-139">Tilbakestille PIN-kode når påloggingen mislykkes et visst antall ganger</span><span class="sxs-lookup"><span data-stu-id="f1db8-139">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="f1db8-140">Hvis du vil forhindre at en uautorisert bruker tilfeldig gjetter en PIN-kode, tilbakestilles PIN-koden etter det antallet feiloppføringer du angir.</span><span class="sxs-lookup"><span data-stu-id="f1db8-140">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="f1db8-141">Kreve at brukere logger seg på igjen etter at Office-apper har vært inaktive i</span><span class="sxs-lookup"><span data-stu-id="f1db8-141">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="f1db8-142">Denne innstillingen bestemmer hvor lenge en bruker kan være inaktiv før de blir bedt om å logge seg på igjen.</span><span class="sxs-lookup"><span data-stu-id="f1db8-142">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
   

