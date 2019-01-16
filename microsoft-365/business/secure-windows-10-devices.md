---
title: Sikre Windows 10-enheter
ms.author: sirkkuw
author: sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: overview
f1_keywords:
- O365E_BCSSetup4WindowsConfig
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: 'Lær om standard og andre innstillinger for å sikre Windows 10 enheter. '
ms.openlocfilehash: 0bdf6a56d880cb84f4a4f50550539d97c006ba49
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/16/2019
ms.locfileid: "26983656"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="d59a4-103">Sikre Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="d59a4-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="d59a4-p101">Innstillingene du konfigurerer her er en del av standardpolicyen for enheter for Windows 10. Alle brukere som kobler til en Windows 10-enhet, inkludert mobile enheter og PC-er, ved å logge på med jobbkontoen sin, får automatisk disse innstillingene. Vi anbefaler at du godtar standardpolicyen under konfigurasjonen og legger til policyer senere som retter seg mot bestemte grupper av brukere.</span><span class="sxs-lookup"><span data-stu-id="d59a4-p101">The settings that you configure here are part of the default device policy for Windows 10. All users that connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account, will automatically receive these settings. We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="d59a4-107">Innstillinger for å sikre Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="d59a4-107">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="d59a4-p102">Som standard er alle innstillingene **På**. Følgende innstillinger er tilgjengelige:</span><span class="sxs-lookup"><span data-stu-id="d59a4-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="d59a4-110">Innstilling</span><span class="sxs-lookup"><span data-stu-id="d59a4-110">Setting</span></span>  <br/> |<span data-ttu-id="d59a4-111">Beskrivelse</span><span class="sxs-lookup"><span data-stu-id="d59a4-111">Description</span></span>  <br/> |
|<span data-ttu-id="d59a4-112">Beskytte PC mot virus og andre trusler ved hjelp av Windows Defender Antivirus</span><span class="sxs-lookup"><span data-stu-id="d59a4-112">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="d59a4-113">Krever at Windows Defender Antivirus er slått på for å beskytte PC-er fra farene ved å være koblet til Internett.</span><span class="sxs-lookup"><span data-stu-id="d59a4-113">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="d59a4-114">Beskytte PC-er fra nettbaserte trusler i Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="d59a4-114">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="d59a4-115">Slår på innstillinger i Microsoft Edge som beskytter brukere mot skadelige nettsteder og nedlastinger.</span><span class="sxs-lookup"><span data-stu-id="d59a4-115">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="d59a4-116">Slå av skjermen på enheten når den har vært inaktiv i en viss periode</span><span class="sxs-lookup"><span data-stu-id="d59a4-116">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="d59a4-p103">Sørger for at bedriftsdata er beskyttet dersom en bruker er inaktiv. Det kan hende en bruker jobber på et offentlig sted, som eksempelvis en kaffebar, går bort eller blir distrahert et øyeblikk og lar enheten være sårbar for tilfeldig innsyn. Denne innstillingen lar deg bestemme hvor lenge en bruker kan være inaktiv før skjermen slås av.</span><span class="sxs-lookup"><span data-stu-id="d59a4-p103">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|<span data-ttu-id="d59a4-120">Tillat brukere å laste ned apper fra Microsoft Store</span><span class="sxs-lookup"><span data-stu-id="d59a4-120">Allow users to download apps from Microsoft Store</span></span>  <br/> |<span data-ttu-id="d59a4-p104">Lar brukere laste ned og installere apper fra Microsoft Store. Apper inkluderer alt fra spill til produktivitetsverktøy, så vi lar denne innstillingen være **På**, men du kan slå den av for ekstra sikkerhet.  </span><span class="sxs-lookup"><span data-stu-id="d59a4-p104">Lets users download and install apps from the Microsoft Store. Apps include everything from games to productivity tools, so we leave this setting **On**, but you can turn it off for extra security.  </span></span><br/> |
|<span data-ttu-id="d59a4-123">Gi brukere tilgang til Cortana</span><span class="sxs-lookup"><span data-stu-id="d59a4-123">Allow users to access Cortana</span></span>  <br/> |<span data-ttu-id="d59a4-p105">Cortana kan være svært nyttig! Hun kan aktivere eller deaktivere innstillinger for deg, gi beskrivelser og passe på at du er tidsnok til avtaler, så vi lar denne innstillingen være **På** som standard.  </span><span class="sxs-lookup"><span data-stu-id="d59a4-p105">Cortana can be very helpful! She can turn settings on or off for you, give directions, and make sure you're on time for appointments, so we keep this **On** by default.  </span></span><br/> |
|<span data-ttu-id="d59a4-126">Tillat brukere å motta Windows-tips og annonser fra Microsoft</span><span class="sxs-lookup"><span data-stu-id="d59a4-126">Allow users to receive Windows tips and advertisements from Microsoft</span></span>  <br/> |<span data-ttu-id="d59a4-127">Tips for Windows kan være praktisk, samt orientere brukere når nye funksjoner utgis.</span><span class="sxs-lookup"><span data-stu-id="d59a4-127">Windows tips can be handy and help orient users when new features are released.</span></span>  <br/> |
|<span data-ttu-id="d59a4-128">Holde Windows 10-enheter oppdatert automatisk</span><span class="sxs-lookup"><span data-stu-id="d59a4-128">Keep Windows 10 devices up to date automatically</span></span>  <br/> |<span data-ttu-id="d59a4-129">Sørger for at Windows 10-enheter automatisk mottar de nyeste oppdateringene.</span><span class="sxs-lookup"><span data-stu-id="d59a4-129">Makes sure that Windows 10 devices automatically receive the latest updates.</span></span>  <br/> |
   

