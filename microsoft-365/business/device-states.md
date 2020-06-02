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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Lær om de ulike enhetstilstandene i enhetshandlingslisten i Admin-hjemmet i Microsoft 365 for bedrifter.
ms.openlocfilehash: 64138e2b6ae73c067709cde1912a96615d08ebf1
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471183"
---
# <a name="device-states"></a><span data-ttu-id="be8bc-103">Enhetstilstander</span><span class="sxs-lookup"><span data-stu-id="be8bc-103">Device states</span></span>

<span data-ttu-id="be8bc-104">Denne artikkelen gjelder for Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="be8bc-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="be8bc-105">Enheter i **Enhetshandlinger**-listen (hjemmesiden for administratorer \> **Enhetshandling**) kan ha følgende statuser.</span><span class="sxs-lookup"><span data-stu-id="be8bc-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="be8bc-107">**Status**</span><span class="sxs-lookup"><span data-stu-id="be8bc-107">**Status**</span></span>|<span data-ttu-id="be8bc-108">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="be8bc-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="be8bc-109">Administrert av Intune</span><span class="sxs-lookup"><span data-stu-id="be8bc-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="be8bc-110">Administreres av Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="be8bc-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="be8bc-111">Ventende tilbaketrekking</span><span class="sxs-lookup"><span data-stu-id="be8bc-111">Retire pending</span></span>  <br/> |<span data-ttu-id="be8bc-112">Microsoft 365 Business Premium gjør seg klar til å fjerne firmadata fra enheten.</span><span class="sxs-lookup"><span data-stu-id="be8bc-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="be8bc-113">Tilbaketrekking pågår</span><span class="sxs-lookup"><span data-stu-id="be8bc-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="be8bc-114">Microsoft 365 Business Premium fjerner for øyeblikket firmadata fra enheten.</span><span class="sxs-lookup"><span data-stu-id="be8bc-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="be8bc-115">Tilbaketrekking mislyktes</span><span class="sxs-lookup"><span data-stu-id="be8bc-115">Retire failed</span></span>  <br/> | <span data-ttu-id="be8bc-116">Fjerning av firmadata mislyktes.</span><span class="sxs-lookup"><span data-stu-id="be8bc-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="be8bc-117">Pensjonere kansellert</span><span class="sxs-lookup"><span data-stu-id="be8bc-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="be8bc-118">Trekket ble avlyst.</span><span class="sxs-lookup"><span data-stu-id="be8bc-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="be8bc-119">Ventende tømming</span><span class="sxs-lookup"><span data-stu-id="be8bc-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="be8bc-120">Venter på at tilbakestilling til fabrikkinnstillinger skal starte.</span><span class="sxs-lookup"><span data-stu-id="be8bc-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="be8bc-121">Tømming pågår</span><span class="sxs-lookup"><span data-stu-id="be8bc-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="be8bc-122">Tilbakestilling til fabrikkinnstillinger er startet.</span><span class="sxs-lookup"><span data-stu-id="be8bc-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="be8bc-123">Tømming mislyktes</span><span class="sxs-lookup"><span data-stu-id="be8bc-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="be8bc-124">Vi kunne ikke finne deg fort nok!</span><span class="sxs-lookup"><span data-stu-id="be8bc-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="be8bc-125">Tørk avbrutt</span><span class="sxs-lookup"><span data-stu-id="be8bc-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="be8bc-126">Fabrikksletting ble kansellert.</span><span class="sxs-lookup"><span data-stu-id="be8bc-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="be8bc-127">Ugyldig</span><span class="sxs-lookup"><span data-stu-id="be8bc-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="be8bc-128">En handling venter (eller pågår), men enheten har ikke sjekket inn på 30 + dager.</span><span class="sxs-lookup"><span data-stu-id="be8bc-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="be8bc-129">Sletting venter</span><span class="sxs-lookup"><span data-stu-id="be8bc-129">Delete pending</span></span>  <br/> |<span data-ttu-id="be8bc-130">Slettehandling pågår.</span><span class="sxs-lookup"><span data-stu-id="be8bc-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="be8bc-131">Oppdaget</span><span class="sxs-lookup"><span data-stu-id="be8bc-131">Discovered</span></span>  <br/> |<span data-ttu-id="be8bc-132">Microsoft 365 Business Premium har oppdaget enheten.</span><span class="sxs-lookup"><span data-stu-id="be8bc-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
