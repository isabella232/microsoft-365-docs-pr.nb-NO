---
title: Administrer hvordan brukere får tilgang til Office-dokumenter på mobile enheter
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4OfficeMobile
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: aa31319c-9196-48c9-a90b-4057e0494c7a
description: Lær om beskyttelsespolicyer som lar deg administrere hvordan brukere får tilgang til Office-apper og arbeidsfiler fra mobile enheter.
ms.openlocfilehash: a48aa241c9e70cf087da3f1701e859dae7238024
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578391"
---
# <a name="manage-how-users-access-office-documents-on-mobile-devices"></a><span data-ttu-id="8b0ee-103">Administrer hvordan brukere får tilgang til Office-dokumenter på mobile enheter</span><span class="sxs-lookup"><span data-stu-id="8b0ee-103">Manage how users access Office documents on mobile devices</span></span>

<span data-ttu-id="8b0ee-104">Denne artikkelen gjelder for Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="8b0ee-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="8b0ee-105">Policyinnstillinger som kontrollerer hvordan brukere får tilgang til Office-filer fra de mobile enhetene, er **Av** som standard.</span><span class="sxs-lookup"><span data-stu-id="8b0ee-105">Policy settings that control how users access Office files from their mobile devices are **Off** by default.</span></span> <span data-ttu-id="8b0ee-106">Vi anbefaler at du godtar standardverdiene under konfigurasjonen for å opprette programpolicyer for Android, iOS og Windows 10 som gjelder for alle brukere.</span><span class="sxs-lookup"><span data-stu-id="8b0ee-106">We recommend that you accept the default values during setup to create application policies for Android, iOS, and Windows 10 that apply to all users.</span></span> <span data-ttu-id="8b0ee-107">Du kan opprette flere policyer når konfigurasjonen er fullført.</span><span class="sxs-lookup"><span data-stu-id="8b0ee-107">You can create more policies after setup completes.</span></span> 
  
## <a name="settings-that-control-how-users-access-office-files-on-mobile-devices"></a><span data-ttu-id="8b0ee-108">Innstillinger som kontrollerer hvordan brukere får tilgang til Office-filer på mobile enheter</span><span class="sxs-lookup"><span data-stu-id="8b0ee-108">Settings that control how users access Office files on mobile devices</span></span>

<span data-ttu-id="8b0ee-109">Følgende innstillinger er tilgjengelig for å styre hvordan brukere får tilgang til Office-arbeidsfiler:</span><span class="sxs-lookup"><span data-stu-id="8b0ee-109">The following settings are available to manage how users access Office work files:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="8b0ee-110">Innstilling</span><span class="sxs-lookup"><span data-stu-id="8b0ee-110">Setting</span></span>  <br/> |<span data-ttu-id="8b0ee-111">Beskrivelse</span><span class="sxs-lookup"><span data-stu-id="8b0ee-111">Description</span></span>  <br/> |
|<span data-ttu-id="8b0ee-112">Kreve en PIN-kode eller et fingeravtrykk for å få tilgang til Office-apper</span><span class="sxs-lookup"><span data-stu-id="8b0ee-112">Require a PIN or fingerprint to access Office apps</span></span>  <br/> |<span data-ttu-id="8b0ee-113">Hvis denne innstillingen er **På**, må brukere angi en annen form for godkjenning, i tillegg til brukernavn og passord, før de kan bruke Office-apper på mobilenheten.</span><span class="sxs-lookup"><span data-stu-id="8b0ee-113">If this setting is **On**, users must provide another form of authentication, in addition to their username and password, before they can use Office apps on their mobile device.</span></span>  <br/> |
|<span data-ttu-id="8b0ee-114">Tilbakestille PIN-kode når påloggingen mislykkes et visst antall ganger</span><span class="sxs-lookup"><span data-stu-id="8b0ee-114">Reset PIN when login fails this many times</span></span>  <br/> |<span data-ttu-id="8b0ee-115">Hvis du vil forhindre at en uautorisert bruker tilfeldig gjetter en PIN-kode, tilbakestilles PIN-koden etter det antallet feiloppføringer du angir.</span><span class="sxs-lookup"><span data-stu-id="8b0ee-115">To prevent an unauthorized user from randomly guessing a PIN, the PIN will reset after the number of wrong entries that you specify.</span></span>  <br/> |
|<span data-ttu-id="8b0ee-116">Kreve at brukere logger seg på igjen etter at Office-apper har vært inaktive i</span><span class="sxs-lookup"><span data-stu-id="8b0ee-116">Require users to sign in again after Office apps have been idle for</span></span>  <br/> |<span data-ttu-id="8b0ee-117">Denne innstillingen bestemmer hvor lenge en bruker kan være inaktiv før de blir bedt om å logge på igjen.</span><span class="sxs-lookup"><span data-stu-id="8b0ee-117">This setting determines how long a user can be idle before they're prompted to sign in again.</span></span>  <br/> |
|<span data-ttu-id="8b0ee-118">Avslå tilgang til arbeidsfiler på enheter der programvarebegrensningene er fjernet, eller enheter som har blitt utsatt for utiltenkt rottilgang</span><span class="sxs-lookup"><span data-stu-id="8b0ee-118">Deny access to work files on jailbroken or rooted devices</span></span>  <br/> |<span data-ttu-id="8b0ee-119">Smarte brukere har kanskje en enhet der programvarebegrensningene er fjernet, eller en enhet som har blitt utsatt for utiltenkt rottilgang.</span><span class="sxs-lookup"><span data-stu-id="8b0ee-119">Clever users may have a device that is jailbroken or rooted.</span></span> <span data-ttu-id="8b0ee-120">Dette betyr at brukeren kan endre operativsystemet, noe som kan gjøre enheten mer utsatt for skadelig programvare.</span><span class="sxs-lookup"><span data-stu-id="8b0ee-120">This means that the user can modify the operating system, which can make the device more susceptible to malware.</span></span> <span data-ttu-id="8b0ee-121">Disse enhetene blokkeres når denne innstillingen er **På**.</span><span class="sxs-lookup"><span data-stu-id="8b0ee-121">These devices are blocked when this setting is **On**.</span></span>  <br/> |
|<span data-ttu-id="8b0ee-122">Ikke tillat brukere å kopiere innhold fra Office-apper til personlige apper</span><span class="sxs-lookup"><span data-stu-id="8b0ee-122">Don't allow users to copy content from Office apps into personal apps</span></span>  <br/> |<span data-ttu-id="8b0ee-123">Når innstillingen er **På**, kan ikke brukeren kopiere informasjon i en arbeidsfil til en personlig fil.</span><span class="sxs-lookup"><span data-stu-id="8b0ee-123">When the setting is **On**, the user can't copy information in a work file to a personal file.</span></span> <span data-ttu-id="8b0ee-124">Hvis innstillingen er **Av**, kan brukeren kopiere informasjon fra en arbeidsfil til en personlig app eller en personlig konto.</span><span class="sxs-lookup"><span data-stu-id="8b0ee-124">If the setting is **Off**, the user can copy information from a work file to a personal app or personal account.</span></span>  <br/> |
   

