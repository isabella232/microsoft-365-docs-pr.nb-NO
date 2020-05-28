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
description: Finn ut mer om de ulike enhetstilstandene i listen Enhetshandlinger i Administratorhjem i Microsoft 365 for bedrifter.
ms.openlocfilehash: 90c11caa03249408ba2916d303bcb4a59fbcca8c
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/27/2020
ms.locfileid: "44400958"
---
# <a name="device-states"></a><span data-ttu-id="45b3a-103">Enhetstilstander</span><span class="sxs-lookup"><span data-stu-id="45b3a-103">Device states</span></span>

<span data-ttu-id="45b3a-104">Enheter i **Enhetshandlinger**-listen (hjemmesiden for administratorer \> **Enhetshandling**) kan ha følgende statuser.</span><span class="sxs-lookup"><span data-stu-id="45b3a-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="45b3a-106">**Status**</span><span class="sxs-lookup"><span data-stu-id="45b3a-106">**Status**</span></span>|<span data-ttu-id="45b3a-107">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="45b3a-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="45b3a-108">Administrert av Intune</span><span class="sxs-lookup"><span data-stu-id="45b3a-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="45b3a-109">Administrert av Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="45b3a-109">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="45b3a-110">Ventende tilbaketrekking</span><span class="sxs-lookup"><span data-stu-id="45b3a-110">Retire pending</span></span>  <br/> |<span data-ttu-id="45b3a-111">Microsoft 365 Business Premium gjør seg klar til å fjerne firmadata fra enheten.</span><span class="sxs-lookup"><span data-stu-id="45b3a-111">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="45b3a-112">Tilbaketrekking pågår</span><span class="sxs-lookup"><span data-stu-id="45b3a-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="45b3a-113">Microsoft 365 Business Premium fjerner for øyeblikket firmadata fra enheten.</span><span class="sxs-lookup"><span data-stu-id="45b3a-113">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="45b3a-114">Tilbaketrekking mislyktes</span><span class="sxs-lookup"><span data-stu-id="45b3a-114">Retire failed</span></span>  <br/> | <span data-ttu-id="45b3a-115">Fjerning av firmadata mislyktes.</span><span class="sxs-lookup"><span data-stu-id="45b3a-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="45b3a-116">Tilbakefør avsagt</span><span class="sxs-lookup"><span data-stu-id="45b3a-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="45b3a-117">Pensjonisthandlingen ble avbrutt.</span><span class="sxs-lookup"><span data-stu-id="45b3a-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="45b3a-118">Ventende tømming</span><span class="sxs-lookup"><span data-stu-id="45b3a-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="45b3a-119">Venter på at tilbakestilling til fabrikkinnstillinger skal starte.</span><span class="sxs-lookup"><span data-stu-id="45b3a-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="45b3a-120">Tømming pågår</span><span class="sxs-lookup"><span data-stu-id="45b3a-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="45b3a-121">Tilbakestilling til fabrikkinnstillinger er startet.</span><span class="sxs-lookup"><span data-stu-id="45b3a-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="45b3a-122">Tømming mislyktes</span><span class="sxs-lookup"><span data-stu-id="45b3a-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="45b3a-123">Kunne ikke tilbakestille fabrikkinnstillingene.</span><span class="sxs-lookup"><span data-stu-id="45b3a-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="45b3a-124">Tørk avbrutt</span><span class="sxs-lookup"><span data-stu-id="45b3a-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="45b3a-125">Fabrikkslettingen ble kansellert.</span><span class="sxs-lookup"><span data-stu-id="45b3a-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="45b3a-126">Ugyldig</span><span class="sxs-lookup"><span data-stu-id="45b3a-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="45b3a-127">En handling venter (eller pågår), men enheten har ikke sjekket inn på 30 + dager.</span><span class="sxs-lookup"><span data-stu-id="45b3a-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="45b3a-128">Sletting venter</span><span class="sxs-lookup"><span data-stu-id="45b3a-128">Delete pending</span></span>  <br/> |<span data-ttu-id="45b3a-129">Slettehandling pågår.</span><span class="sxs-lookup"><span data-stu-id="45b3a-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="45b3a-130">Oppdaget</span><span class="sxs-lookup"><span data-stu-id="45b3a-130">Discovered</span></span>  <br/> |<span data-ttu-id="45b3a-131">Microsoft 365 Business Premium har oppdaget enheten.</span><span class="sxs-lookup"><span data-stu-id="45b3a-131">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
