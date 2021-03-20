---
title: Sikre Windows 10-enheter
f1.keywords:
- CSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
f1_keywords:
- O365E_BCSSetup4WindowsConfig
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 21e5551f-fa35-4f13-9418-f80d668b6a2b
description: Finn ut mer om hvordan du konfigurerer innstillingene for standard enhetspolicy som alle Windows 10-enheter mottar ved pålogging til jobb- eller skolekontoen.
ms.openlocfilehash: 85383b1e1d2f2af3fd49d4a0c56c5d99586d607d
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912614"
---
# <a name="secure-windows-10-devices"></a><span data-ttu-id="07e0d-103">Sikre Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="07e0d-103">Secure Windows 10 devices</span></span>

<span data-ttu-id="07e0d-104">Denne artikkelen gjelder for Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="07e0d-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="07e0d-105">Innstillingene du konfigurerer her er en del av standardpolicyen for enheter for Windows 10.</span><span class="sxs-lookup"><span data-stu-id="07e0d-105">The settings that you configure here are part of the default device policy for Windows 10.</span></span> <span data-ttu-id="07e0d-106">Alle brukere som kobler til en Windows 10-enhet, inkludert mobile enheter og PC-er, ved å logge på med jobbkontoen, mottar automatisk disse innstillingene.</span><span class="sxs-lookup"><span data-stu-id="07e0d-106">All users who connect a Windows 10 device, including mobile devices and PCs, by signing in with their work account will automatically receive these settings.</span></span> <span data-ttu-id="07e0d-107">Vi anbefaler at du godtar standardpolicyen under konfigurasjonen og legger til policyer senere som retter seg mot bestemte grupper av brukere.</span><span class="sxs-lookup"><span data-stu-id="07e0d-107">We recommend that you accept the default policy during setup and add policies later that target specific groups of users.</span></span>
  
## <a name="settings-to-secure-windows-10-devices"></a><span data-ttu-id="07e0d-108">Innstillinger for å sikre Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="07e0d-108">Settings to secure Windows 10 devices</span></span>

<span data-ttu-id="07e0d-p102">Som standard er alle innstillingene **På**. Følgende innstillinger er tilgjengelige:</span><span class="sxs-lookup"><span data-stu-id="07e0d-p102">By default all settings are **On**. The following settings are available:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="07e0d-111">Innstilling</span><span class="sxs-lookup"><span data-stu-id="07e0d-111">Setting</span></span>  <br/> |<span data-ttu-id="07e0d-112">Beskrivelse</span><span class="sxs-lookup"><span data-stu-id="07e0d-112">Description</span></span>  <br/> |
|<span data-ttu-id="07e0d-113">Beskytte PC mot virus og andre trusler ved hjelp av Windows Defender Antivirus</span><span class="sxs-lookup"><span data-stu-id="07e0d-113">Help protect PCs from viruses and other threats using Windows Defender Antivirus</span></span>  <br/> |<span data-ttu-id="07e0d-114">Krever at Windows Defender Antivirus er slått på for å beskytte PC-er fra farene ved å være koblet til Internett.</span><span class="sxs-lookup"><span data-stu-id="07e0d-114">Requires that Windows Defender Antivirus is turned on to protect PCs from the dangers of being connected to the internet.</span></span>  <br/> |
|<span data-ttu-id="07e0d-115">Beskytte PC-er fra nettbaserte trusler i Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="07e0d-115">Help protect PCs from web-based threats in Microsoft Edge</span></span>  <br/> |<span data-ttu-id="07e0d-116">Slår på innstillinger i Microsoft Edge som beskytter brukere mot skadelige nettsteder og nedlastinger.</span><span class="sxs-lookup"><span data-stu-id="07e0d-116">Turns on settings in Edge that help protect users from malicious sites and downloads.</span></span>  <br/> |
|<span data-ttu-id="07e0d-117">Bruke BitLocker til å beskytte filer og mapper på PC-er mot uautorisert tilgang</span><span class="sxs-lookup"><span data-stu-id="07e0d-117">Help protect files and folders on PCs from unauthorized access with BitLocker</span></span>  <br/> |<span data-ttu-id="07e0d-118">BitLocker beskytter dataene ved å kryptere harddiskene på datamaskinen og beskytter mot eksponering av dataene dersom en datamaskin mistes eller blir stjålet.</span><span class="sxs-lookup"><span data-stu-id="07e0d-118">Bitlocker protects data by encrypting the computer hard drives and protect against data exposure if a computer is lost or stolen.</span></span> <span data-ttu-id="07e0d-119">Hvis du vil ha mer informasjon, kan du [se Vanlige spørsmål om Bitlocker](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions).</span><span class="sxs-lookup"><span data-stu-id="07e0d-119">For more information, see [Bitlocker FAQ](/windows/security/information-protection/bitlocker/bitlocker-frequently-asked-questions).</span></span>  <br/> |
|<span data-ttu-id="07e0d-120">Slå av skjermen på enheten når den har vært inaktiv i en viss periode</span><span class="sxs-lookup"><span data-stu-id="07e0d-120">Turn off device screen when idle for this amount of time</span></span>  <br/> |<span data-ttu-id="07e0d-p104">Sørger for at bedriftsdata er beskyttet dersom en bruker er inaktiv. En bruker kan jobbe på et offentlig sted, som for eksempel en kaffebar, går bort eller blir distrahert i et øyeblikk, og lar enheten være sårbar for tilfeldig innsyn. Denne innstillingen lar deg bestemme hvor lenge en bruker kan være inaktiv før skjermen slås av.</span><span class="sxs-lookup"><span data-stu-id="07e0d-p104">Makes sure that company data is protected if a user is idle. A user may be working in a public location, like a coffee shop, and step away or be distracted for just a moment, leaving their device vulnerable to random glances. This setting lets you control how long the user can be idle before the screen shuts off.</span></span>  <br/> |
|