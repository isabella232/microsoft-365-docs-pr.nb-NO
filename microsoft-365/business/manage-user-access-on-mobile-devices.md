---
title: Administrer hvordan brukere får tilgang til Office-dokumenter på mobile enheter
ms.author: sirkkuw
author: sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
f1_keywords:
- 'O365E_BCSSetup4OfficeMobile '
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Lær mer om beskyttelse av policyer som kan hjelpe sikker tilgang til Office-programmer fra mobile enheter.
ms.openlocfilehash: 75dbe79acccabd851c43259a165e79bfe3c509c0
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983186"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="bae2e-103">Administrer hvordan brukere får tilgang til Office-dokumenter på mobile enheter</span><span class="sxs-lookup"><span data-stu-id="bae2e-103">Manage how users access Office documents on mobile devices</span></span>

 <span data-ttu-id="bae2e-p101">Policyinnstillinger som kontrollerer hvordan brukere får tilgang til Office-filer fra de mobile enhetene, er **Av** som standard. Vi anbefaler at du godtar standardverdiene under konfigurasjonen for å opprette programpolicyer for Android, iOS og Windows 10 som gjelder for alle brukere. Du kan opprette flere policyer når konfigurasjonen er fullført.</span><span class="sxs-lookup"><span data-stu-id="bae2e-p101">Policy settings that control how users access Office files from their mobile devices are **Off** by default. We recommend you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users. You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="bae2e-107">Innstillinger som kontrollerer hvordan brukere får tilgang til Office-filer på mobile enheter</span><span class="sxs-lookup"><span data-stu-id="bae2e-107">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="bae2e-108">Følgende innstillinger er tilgjengelig for å styre hvordan brukere får tilgang til Office-arbeidsfiler:</span><span class="sxs-lookup"><span data-stu-id="bae2e-108">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="bae2e-109">Innstilling</span><span class="sxs-lookup"><span data-stu-id="bae2e-109">Setting</span></span>  <br/> |<span data-ttu-id="bae2e-110">Beskrivelse</span><span class="sxs-lookup"><span data-stu-id="bae2e-110">Description</span></span>  <br/> |
|<span data-ttu-id="bae2e-111">Kreve en PIN-kode eller et fingeravtrykk for å få tilgang til Office-apper</span><span class="sxs-lookup"><span data-stu-id="bae2e-111">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="bae2e-112">Hvis disse innstillingene er **På**, må brukere gi en annen form for godkjenning, i tillegg til brukernavn og passord, før de kan bruke Office-apper på mobilenheten.</span><span class="sxs-lookup"><span data-stu-id="bae2e-112">If this settings is **On** users have to provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="bae2e-113">Tilbakestille PIN-kode når påloggingen mislykkes et visst antall ganger</span><span class="sxs-lookup"><span data-stu-id="bae2e-113">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="bae2e-114">Hvis du vil forhindre at en uautorisert bruker tilfeldig gjetter en PIN-kode, tilbakestilles PIN-koden etter det antallet feiloppføringer du angir.</span><span class="sxs-lookup"><span data-stu-id="bae2e-114">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="bae2e-115">Kreve at brukere logger seg på igjen etter at Office-apper har vært inaktive i</span><span class="sxs-lookup"><span data-stu-id="bae2e-115">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="bae2e-116">Denne innstillingen bestemmer hvor lenge en bruker kan være inaktiv før de blir bedt om å logge seg på igjen.</span><span class="sxs-lookup"><span data-stu-id="bae2e-116">This setting determines how long a user can be idle before they are prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="bae2e-117">Avslå tilgang til arbeidsfiler på enheter der programvarebegrensningene er fjernet, eller enheter som har blitt utsatt for utiltenkt rottilgang</span><span class="sxs-lookup"><span data-stu-id="bae2e-117">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="bae2e-p102">Smarte brukere har kanskje en enhet der programvarebegrensningene er fjernet, eller en enhet som har blitt utsatt for utiltenkt rottilgang. Dette betyr at brukeren kan endre operativsystemet, noe som kan gjøre enheten mer utsatt for skadelig programvare. Disse enhetene blokkeres når denne innstillingen er **På**.  </span><span class="sxs-lookup"><span data-stu-id="bae2e-p102">Clever users may have a device that is jailbroken or rooted. This means that the user can modify the operating system, which can make the device more subject to malware. These devices are blocked when this setting is **On**.  </span></span><br/> |
|<span data-ttu-id="bae2e-121">Tillate brukere å kopiere innhold fra Office-apper til personlige apper</span><span class="sxs-lookup"><span data-stu-id="bae2e-121">Allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="bae2e-p103">Vi tillater ikke dette som standard, men hvis innstillingen er satt til **På**, vil brukeren kunne kopiere informasjon fra en arbeidsfil til en personlig fil. Hvis innstillingen er **Av**, kan ikke brukeren kopiere informasjon fra en jobbfil til en personlig app eller personlig konto.  </span><span class="sxs-lookup"><span data-stu-id="bae2e-p103">We allow this by default, but when the setting is **On**, the user can copy information in a work file to a personal file. If the setting is **Off**, the user can't copy information from a work file to a personal app or personal account.  </span></span><br/> |
   

