---
title: Enhetstilstander
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Lær om de ulike enhetstilstandene i Enhetshandlinger-listen i hjemmesiden for administratorer i Microsoft 365 for bedrifter.
ms.openlocfilehash: e6f1b428413d094e0a1ce3afb026528074038736
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/02/2021
ms.locfileid: "51578471"
---
# <a name="device-states"></a><span data-ttu-id="fe79b-103">Enhetstilstander</span><span class="sxs-lookup"><span data-stu-id="fe79b-103">Device states</span></span>

<span data-ttu-id="fe79b-104">Denne artikkelen gjelder for Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="fe79b-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="fe79b-105">Enheter i **Enhetshandlinger**-listen (hjemmesiden for administratorer \> **Enhetshandling**) kan ha følgende statuser.</span><span class="sxs-lookup"><span data-stu-id="fe79b-105">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="fe79b-107">**Status**</span><span class="sxs-lookup"><span data-stu-id="fe79b-107">**Status**</span></span>|<span data-ttu-id="fe79b-108">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="fe79b-108">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fe79b-109">Administrert av Intune</span><span class="sxs-lookup"><span data-stu-id="fe79b-109">Managed by Intune</span></span>  <br/> |<span data-ttu-id="fe79b-110">Administreres av Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="fe79b-110">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="fe79b-111">Ventende tilbaketrekking</span><span class="sxs-lookup"><span data-stu-id="fe79b-111">Retire pending</span></span>  <br/> |<span data-ttu-id="fe79b-112">Microsoft 365 Business Premium gjør seg klar til å fjerne firmadata fra enheten.</span><span class="sxs-lookup"><span data-stu-id="fe79b-112">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="fe79b-113">Tilbaketrekking pågår</span><span class="sxs-lookup"><span data-stu-id="fe79b-113">Retire in progress</span></span>  <br/> |<span data-ttu-id="fe79b-114">Microsoft 365 Business Premium fjerner for øyeblikket firmadata fra enheten.</span><span class="sxs-lookup"><span data-stu-id="fe79b-114">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="fe79b-115">Tilbaketrekking mislyktes</span><span class="sxs-lookup"><span data-stu-id="fe79b-115">Retire failed</span></span>  <br/> | <span data-ttu-id="fe79b-116">Fjerning av firmadata mislyktes.</span><span class="sxs-lookup"><span data-stu-id="fe79b-116">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="fe79b-117">Tilbaketrekking avbrutt</span><span class="sxs-lookup"><span data-stu-id="fe79b-117">Retire canceled</span></span>  <br/> |<span data-ttu-id="fe79b-118">Tilbaketrekkingshandlingen ble avbrutt.</span><span class="sxs-lookup"><span data-stu-id="fe79b-118">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="fe79b-119">Ventende tømming</span><span class="sxs-lookup"><span data-stu-id="fe79b-119">Wipe pending</span></span>  <br/> |<span data-ttu-id="fe79b-120">Venter på at tilbakestilling til fabrikkinnstillinger skal starte.</span><span class="sxs-lookup"><span data-stu-id="fe79b-120">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="fe79b-121">Tømming pågår</span><span class="sxs-lookup"><span data-stu-id="fe79b-121">Wipe in progress</span></span>  <br/> |<span data-ttu-id="fe79b-122">Tilbakestilling til fabrikkinnstillinger er startet.</span><span class="sxs-lookup"><span data-stu-id="fe79b-122">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="fe79b-123">Tømming mislyktes</span><span class="sxs-lookup"><span data-stu-id="fe79b-123">Wipe failed</span></span>  <br/> |<span data-ttu-id="fe79b-124">Kan ikke tilbakestille fabrikkinnstillingene.</span><span class="sxs-lookup"><span data-stu-id="fe79b-124">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="fe79b-125">Tømming avbrutt</span><span class="sxs-lookup"><span data-stu-id="fe79b-125">Wipe canceled</span></span>  <br/> |<span data-ttu-id="fe79b-126">Tømming av fabrikken ble avbrutt.</span><span class="sxs-lookup"><span data-stu-id="fe79b-126">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="fe79b-127">Ugyldig</span><span class="sxs-lookup"><span data-stu-id="fe79b-127">Unhealthy</span></span>  <br/> |<span data-ttu-id="fe79b-128">En handling venter (eller pågår), men enheten har ikke sjekket inn på over 30 dager.</span><span class="sxs-lookup"><span data-stu-id="fe79b-128">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="fe79b-129">Sletting venter</span><span class="sxs-lookup"><span data-stu-id="fe79b-129">Delete pending</span></span>  <br/> |<span data-ttu-id="fe79b-130">Slettehandling pågår.</span><span class="sxs-lookup"><span data-stu-id="fe79b-130">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="fe79b-131">Oppdaget</span><span class="sxs-lookup"><span data-stu-id="fe79b-131">Discovered</span></span>  <br/> |<span data-ttu-id="fe79b-132">Microsoft 365 Business Premium har oppdaget enheten.</span><span class="sxs-lookup"><span data-stu-id="fe79b-132">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
