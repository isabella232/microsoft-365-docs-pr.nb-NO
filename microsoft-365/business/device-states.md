---
title: Enhetstilstander
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
description: Lær mer om enhetstilstander i Microsoft 365 Business.
ms.openlocfilehash: 15114835a5014f5bfac600eac79bcdffdaec481a
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32276989"
---
# <a name="device-states"></a><span data-ttu-id="18b9b-103">Enhetstilstander</span><span class="sxs-lookup"><span data-stu-id="18b9b-103">Device states</span></span>

## <a name="device-states"></a><span data-ttu-id="18b9b-104">Enhetstilstander</span><span class="sxs-lookup"><span data-stu-id="18b9b-104">Device states</span></span>

<span data-ttu-id="18b9b-105">Enheter i **Enhetshandlinger**-listen (hjemmesiden for administratorer \> **Enhetshandling**) kan ha følgende statuser.</span><span class="sxs-lookup"><span data-stu-id="18b9b-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="18b9b-107">**Status**</span><span class="sxs-lookup"><span data-stu-id="18b9b-107">**Status**</span></span>|<span data-ttu-id="18b9b-108">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="18b9b-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="18b9b-109">Administrert av Intune</span><span class="sxs-lookup"><span data-stu-id="18b9b-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="18b9b-110">Administrert av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="18b9b-110">Managed by Microsoft 365 Business.</span></span>  <br/> |
|<span data-ttu-id="18b9b-111">Ventende tilbaketrekking</span><span class="sxs-lookup"><span data-stu-id="18b9b-111">Retire pending</span></span>  <br/> |<span data-ttu-id="18b9b-112">Microsoft 365 Business klargjøres for å fjerne firmadata fra enheten.</span><span class="sxs-lookup"><span data-stu-id="18b9b-112">Microsoft 365 Business is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="18b9b-113">Tilbaketrekking pågår</span><span class="sxs-lookup"><span data-stu-id="18b9b-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="18b9b-114">Microsoft 365 Business fjerner firmadata fra enheten.</span><span class="sxs-lookup"><span data-stu-id="18b9b-114">Microsoft 365 Business is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="18b9b-115">Tilbaketrekking mislyktes</span><span class="sxs-lookup"><span data-stu-id="18b9b-115">Retire failed</span></span>  <br/> | <span data-ttu-id="18b9b-116">Fjerning av firmadata mislyktes.</span><span class="sxs-lookup"><span data-stu-id="18b9b-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="18b9b-117">Tilbaketrekking avbrutt</span><span class="sxs-lookup"><span data-stu-id="18b9b-117">Retire cancelled</span></span>  <br/> |<span data-ttu-id="18b9b-118">Tilbaketrekkingen ble avbrutt.</span><span class="sxs-lookup"><span data-stu-id="18b9b-118">Retire action was cancelled.</span></span>  <br/> |
|<span data-ttu-id="18b9b-119">Ventende tømming</span><span class="sxs-lookup"><span data-stu-id="18b9b-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="18b9b-120">Venter på at tilbakestilling til fabrikkinnstillinger skal starte.</span><span class="sxs-lookup"><span data-stu-id="18b9b-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="18b9b-121">Tømming pågår</span><span class="sxs-lookup"><span data-stu-id="18b9b-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="18b9b-122">Tilbakestilling til fabrikkinnstillinger er startet.</span><span class="sxs-lookup"><span data-stu-id="18b9b-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="18b9b-123">Tømming mislyktes</span><span class="sxs-lookup"><span data-stu-id="18b9b-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="18b9b-124">Kan ikke tilbakestilling til fabrikkinnstillinger.</span><span class="sxs-lookup"><span data-stu-id="18b9b-124">Couldn't perform factory reset.</span></span>  <br/> |
|<span data-ttu-id="18b9b-125">Tømming avbrutt</span><span class="sxs-lookup"><span data-stu-id="18b9b-125">Wipe cancelled</span></span>  <br/> |<span data-ttu-id="18b9b-126">Tilbakestilling til fabrikkinnstillinger ble avbrutt.</span><span class="sxs-lookup"><span data-stu-id="18b9b-126">Factory wipe was cancelled.</span></span>  <br/> |
|<span data-ttu-id="18b9b-127">Ugyldig</span><span class="sxs-lookup"><span data-stu-id="18b9b-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="18b9b-128">Dette betyr at en handling er ventende (eller pågår), men enheten har ikke blitt sjekket inn på 30 dager.</span><span class="sxs-lookup"><span data-stu-id="18b9b-128">This means that an action is pending (or in progress) but the device has not checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="18b9b-129">Sletting venter</span><span class="sxs-lookup"><span data-stu-id="18b9b-129">Delete pending</span></span>  <br/> |<span data-ttu-id="18b9b-130">Slettehandling pågår.</span><span class="sxs-lookup"><span data-stu-id="18b9b-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="18b9b-131">Oppdaget</span><span class="sxs-lookup"><span data-stu-id="18b9b-131">Discovered</span></span>  <br/> |<span data-ttu-id="18b9b-132">Microsoft 365 Business har oppdaget enheten.</span><span class="sxs-lookup"><span data-stu-id="18b9b-132">Microsoft 365 Business has detected the device.</span></span>  <br/> |
   
