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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: c3ac23c5-d4b4-4b1b-b7ce-ea759521bf8c
description: Finn ut mer om de ulike enhetstilstandene i listen Enhetshandlinger i Administratorhjem i Microsoft 365 for bedrifter.
ms.openlocfilehash: 1a66e76dd3a74428923292427b01551db2449e48
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/21/2020
ms.locfileid: "43627250"
---
# <a name="device-states"></a><span data-ttu-id="ca093-103">Enhetstilstander</span><span class="sxs-lookup"><span data-stu-id="ca093-103">Device states</span></span>

<span data-ttu-id="ca093-104">Enheter i **Enhetshandlinger**-listen (hjemmesiden for administratorer \> **Enhetshandling**) kan ha følgende statuser.</span><span class="sxs-lookup"><span data-stu-id="ca093-104">Devices in the **Device actions** list (Admin home \> **Device actions**) can have the following states.</span></span>
  
![In the Device actions list, you can see the Devices states.](../media/a621c47e-45d9-4e1a-beb9-c03254d40c1d.png)
  
|<span data-ttu-id="ca093-106">**Status**</span><span class="sxs-lookup"><span data-stu-id="ca093-106">**Status**</span></span>|<span data-ttu-id="ca093-107">**Beskrivelse**</span><span class="sxs-lookup"><span data-stu-id="ca093-107">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ca093-108">Administrert av Intune</span><span class="sxs-lookup"><span data-stu-id="ca093-108">Managed by Intune</span></span>  <br/> |<span data-ttu-id="ca093-109">Administrert av Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="ca093-109">Managed by Microsoft 365 Business Premium.</span></span>  <br/> |
|<span data-ttu-id="ca093-110">Ventende tilbaketrekking</span><span class="sxs-lookup"><span data-stu-id="ca093-110">Retire pending</span></span>  <br/> |<span data-ttu-id="ca093-111">Microsoft 365 Business Premium gjør seg klar til å fjerne firmadata fra enheten.</span><span class="sxs-lookup"><span data-stu-id="ca093-111">Microsoft 365 Business Premium is getting ready to remove company data from the device.</span></span>  <br/> |
|<span data-ttu-id="ca093-112">Tilbaketrekking pågår</span><span class="sxs-lookup"><span data-stu-id="ca093-112">Retire in progress</span></span>  <br/> |<span data-ttu-id="ca093-113">Microsoft 365 Business Premium fjerner for øyeblikket firmadata fra enheten.</span><span class="sxs-lookup"><span data-stu-id="ca093-113">Microsoft 365 Business Premium is currently removing company data from the device.</span></span>  <br/> |
|<span data-ttu-id="ca093-114">Tilbaketrekking mislyktes</span><span class="sxs-lookup"><span data-stu-id="ca093-114">Retire failed</span></span>  <br/> | <span data-ttu-id="ca093-115">Fjerning av firmadata mislyktes.</span><span class="sxs-lookup"><span data-stu-id="ca093-115">Remove company data action failed.</span></span>  <br/> |
|<span data-ttu-id="ca093-116">Tilbakefør avsagt</span><span class="sxs-lookup"><span data-stu-id="ca093-116">Retire canceled</span></span>  <br/> |<span data-ttu-id="ca093-117">Pensjonisthandlingen ble avbrutt.</span><span class="sxs-lookup"><span data-stu-id="ca093-117">Retire action was canceled.</span></span>  <br/> |
|<span data-ttu-id="ca093-118">Ventende tømming</span><span class="sxs-lookup"><span data-stu-id="ca093-118">Wipe pending</span></span>  <br/> |<span data-ttu-id="ca093-119">Venter på at tilbakestilling til fabrikkinnstillinger skal starte.</span><span class="sxs-lookup"><span data-stu-id="ca093-119">Waiting for factory reset to start.</span></span>  <br/> |
|<span data-ttu-id="ca093-120">Tømming pågår</span><span class="sxs-lookup"><span data-stu-id="ca093-120">Wipe in progress</span></span>  <br/> |<span data-ttu-id="ca093-121">Tilbakestilling til fabrikkinnstillinger er startet.</span><span class="sxs-lookup"><span data-stu-id="ca093-121">Factory reset has been issued.</span></span>  <br/> |
|<span data-ttu-id="ca093-122">Tømming mislyktes</span><span class="sxs-lookup"><span data-stu-id="ca093-122">Wipe failed</span></span>  <br/> |<span data-ttu-id="ca093-123">Kunne ikke tilbakestille fabrikkinnstillingene.</span><span class="sxs-lookup"><span data-stu-id="ca093-123">Couldn't do factory reset.</span></span>  <br/> |
|<span data-ttu-id="ca093-124">Tørk avbrutt</span><span class="sxs-lookup"><span data-stu-id="ca093-124">Wipe canceled</span></span>  <br/> |<span data-ttu-id="ca093-125">Fabrikkslettingen ble kansellert.</span><span class="sxs-lookup"><span data-stu-id="ca093-125">Factory wipe was canceled.</span></span>  <br/> |
|<span data-ttu-id="ca093-126">Ugyldig</span><span class="sxs-lookup"><span data-stu-id="ca093-126">Unhealthy</span></span>  <br/> |<span data-ttu-id="ca093-127">En handling venter (eller pågår), men enheten har ikke sjekket inn på 30 + dager.</span><span class="sxs-lookup"><span data-stu-id="ca093-127">An action is pending (or in progress), but the device hasn't checked in for 30+ days.</span></span>  <br/> |
|<span data-ttu-id="ca093-128">Sletting venter</span><span class="sxs-lookup"><span data-stu-id="ca093-128">Delete pending</span></span>  <br/> |<span data-ttu-id="ca093-129">Slettehandling pågår.</span><span class="sxs-lookup"><span data-stu-id="ca093-129">Delete action is pending.</span></span>  <br/> |
|<span data-ttu-id="ca093-130">Oppdaget</span><span class="sxs-lookup"><span data-stu-id="ca093-130">Discovered</span></span>  <br/> |<span data-ttu-id="ca093-131">Microsoft 365 Business Premium har oppdaget enheten.</span><span class="sxs-lookup"><span data-stu-id="ca093-131">Microsoft 365 Business Premium has detected the device.</span></span>  <br/> |
   
