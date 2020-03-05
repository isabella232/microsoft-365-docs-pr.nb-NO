---
title: Enhetstilstander
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
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
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Finn ut mer om de ulike enhetstilstandene i enhetshandlinger-listen i administratorhjemme i Microsoft 365 Business.
ms.openlocfilehash: 878050fbe11acca1d5d434a5d2ab0b5b48510e45
ms.sourcegitcommit: ab916c216053999c9c4ef4838217e82cd861f23f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2020
ms.locfileid: "42415669"
---
# <a name="device-states"></a><span data-ttu-id="e09a5-103">Enhetstilstander</span><span class="sxs-lookup"><span data-stu-id="e09a5-103">Device states</span></span>

<span data-ttu-id="e09a5-104">Enheter i **Enhetshandlinger**-listen (hjemmesiden for administratorer \> **Enhetshandling**) kan ha følgende statuser.</span><span class="sxs-lookup"><span data-stu-id="e09a5-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="e09a5-106">**Status**</span><span class="sxs-lookup"><span data-stu-id="e09a5-106">**Status**</span></span>|<span data-ttu-id="e09a5-107">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="e09a5-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e09a5-108">Administrert av Intune</span><span class="sxs-lookup"><span data-stu-id="e09a5-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="e09a5-109">Administrert av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="e09a5-109">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="e09a5-110">Ventende tilbaketrekking</span><span class="sxs-lookup"><span data-stu-id="e09a5-110">Retire pending</span></span>  <br/> |<span data-ttu-id="e09a5-111">Microsoft 365 Business klargjøres for å fjerne firmadata fra enheten.</span><span class="sxs-lookup"><span data-stu-id="e09a5-111">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="e09a5-112">Tilbaketrekking pågår</span><span class="sxs-lookup"><span data-stu-id="e09a5-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="e09a5-113">Microsoft 365 Business fjerner firmadata fra enheten.</span><span class="sxs-lookup"><span data-stu-id="e09a5-113">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="e09a5-114">Tilbaketrekking mislyktes</span><span class="sxs-lookup"><span data-stu-id="e09a5-114">Retire failed</span></span>  <br/> | <span data-ttu-id="e09a5-115">Fjerning av firmadata mislyktes.</span><span class="sxs-lookup"><span data-stu-id="e09a5-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="e09a5-116">Avslutt avbrutt</span><span class="sxs-lookup"><span data-stu-id="e09a5-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="e09a5-117">Pensjonering handling ble avbrutt.</span><span class="sxs-lookup"><span data-stu-id="e09a5-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="e09a5-118">Ventende tømming</span><span class="sxs-lookup"><span data-stu-id="e09a5-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="e09a5-119">Venter på at tilbakestilling til fabrikkinnstillinger skal starte.</span><span class="sxs-lookup"><span data-stu-id="e09a5-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="e09a5-120">Tømming pågår</span><span class="sxs-lookup"><span data-stu-id="e09a5-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="e09a5-121">Tilbakestilling til fabrikkinnstillinger er startet.</span><span class="sxs-lookup"><span data-stu-id="e09a5-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="e09a5-122">Tømming mislyktes</span><span class="sxs-lookup"><span data-stu-id="e09a5-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="e09a5-123">Vi kunne ikke finne deg fort nok!</span><span class="sxs-lookup"><span data-stu-id="e09a5-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="e09a5-124">Tørk av avbrutt</span><span class="sxs-lookup"><span data-stu-id="e09a5-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="e09a5-125">Fabrikktørking ble avbrutt.</span><span class="sxs-lookup"><span data-stu-id="e09a5-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="e09a5-126">Ugyldig</span><span class="sxs-lookup"><span data-stu-id="e09a5-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="e09a5-127">En handling venter (eller pågår), men enheten har ikke sjekket inn på 30 + dager.</span><span class="sxs-lookup"><span data-stu-id="e09a5-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="e09a5-128">Sletting venter</span><span class="sxs-lookup"><span data-stu-id="e09a5-128">Delete pending</span></span>  <br/> |<span data-ttu-id="e09a5-129">Slettehandling pågår.</span><span class="sxs-lookup"><span data-stu-id="e09a5-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="e09a5-130">Oppdaget</span><span class="sxs-lookup"><span data-stu-id="e09a5-130">Discovered</span></span>  <br/> |<span data-ttu-id="e09a5-131">Microsoft 365 Business har oppdaget enheten.</span><span class="sxs-lookup"><span data-stu-id="e09a5-131">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
