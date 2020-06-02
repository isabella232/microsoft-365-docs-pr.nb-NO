---
title: Klargjøre for Office-klientdistribusjon av Microsoft 365 for bedrifter
f1.keywords:
- CSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Lær hvordan du installerer 32-biters Office-apper automatisk på Windows 10-datamaskiner og holder dem oppdatert.
ms.openlocfilehash: 2de492914edbde2afe593aac290c4a634b801443
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470951"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="5f3ce-103">Klargjøre for Office-klientdistribusjon av Microsoft 365 for bedrifter</span><span class="sxs-lookup"><span data-stu-id="5f3ce-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

<span data-ttu-id="5f3ce-104">Denne artikkelen gjelder for Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="5f3ce-105">Klargjøre for å installere Office-programmer automatisk på klientmaskiner</span><span class="sxs-lookup"><span data-stu-id="5f3ce-105">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="5f3ce-106">Du kan bruke Microsoft 365 Business Premium til å installere 32-biters Office-apper automatisk på Windows 10-datamaskiner og holde dem oppdatert med oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-106">You can use Microsoft 365 Business Premium to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="5f3ce-107">Automatisk installasjon fungerer best hvis sluttbrukerens datamaskin er på Windows 10 Business og:</span><span class="sxs-lookup"><span data-stu-id="5f3ce-107">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="5f3ce-108">Ikke har eksisterende Office-skrivebordsapper (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access og OneDrive).</span><span class="sxs-lookup"><span data-stu-id="5f3ce-108">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="5f3ce-109">eller</span><span class="sxs-lookup"><span data-stu-id="5f3ce-109">or</span></span>
    
- <span data-ttu-id="5f3ce-110">Har en eksisterende versjon av Klikk og bruk Office installert.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-110">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="5f3ce-111">Hvis du vil finne ut om du har klikk og bruk-versjonen av Office, gå til **Fil** \> **Konto** i en hvilken som helst Office-app ( **Office Konto** i Outlook).</span><span class="sxs-lookup"><span data-stu-id="5f3ce-111">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="5f3ce-112">Hvis du ser **Office-oppdateringer** som vist i figuren nedenfor, ble installasjonen gjort ved hjelp av Klikk og bruk.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-112">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="5f3ce-114">**Hvem drar nytte av å ha denne funksjonen**</span><span class="sxs-lookup"><span data-stu-id="5f3ce-114">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="5f3ce-115">Sluttbruker med PC som:</span><span class="sxs-lookup"><span data-stu-id="5f3ce-115">The end user whose PC:</span></span>
  
- <span data-ttu-id="5f3ce-116">**Har** en brukerlisens for Windows 10 Business, en aktiv Microsoft 365 for business-lisens, Windows 10 Creators Update og er koblet til Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-116">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="5f3ce-117">**Har ikke** 64-biters Office-apper (f.eks. Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="5f3ce-117">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="5f3ce-118">Hvis 64-biters Office-apper er nødvendig, passer ikke denne funksjonen, fordi det ikke er noen støtte for å utløse en 64-biters 2016 Klikk og bruk-versjon av Office fra Administrasjonskonsollen for Microsoft 365 for bedrifter.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-118">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="5f3ce-119">**Ikke har** noen frittstående apper for 2016 Windows Installer (MSI) (for eksempel Visio eller Project).</span><span class="sxs-lookup"><span data-stu-id="5f3ce-119">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="5f3ce-120">Microsoft 365 for bedrifter oppgraderer Office til Klikk og bruk-versjonen av Office-2016, og det fungerer ikke med frittstående office-apper for Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-120">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="5f3ce-121">Tabellen nedenfor viser hvilken handling sluttbrukerne/administratorene må utføre, avhengig av starttilstanden, for å ha en vellykket 32-biters klikk-til-bruk-versjon av Office-distribusjon fra administrasjonskonsollen for Microsoft 365 for bedrifter.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-121">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span>
  
|<span data-ttu-id="5f3ce-122">**Status for Office-installasjon før start**</span><span class="sxs-lookup"><span data-stu-id="5f3ce-122">**Starting Office install status**</span></span>|<span data-ttu-id="5f3ce-123">**Tiltak som skal iverksettes før Microsoft 365 for bedrifter Office installeres**</span><span class="sxs-lookup"><span data-stu-id="5f3ce-123">**Action to take before Microsoft 365 for business Office install**</span></span>|<span data-ttu-id="5f3ce-124">**Sluttstatus**</span><span class="sxs-lookup"><span data-stu-id="5f3ce-124">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5f3ce-125">Ingen Office suite installert</span><span class="sxs-lookup"><span data-stu-id="5f3ce-125">No Office suite installed</span></span>  <br/> |<span data-ttu-id="5f3ce-126">Ingen</span><span class="sxs-lookup"><span data-stu-id="5f3ce-126">None</span></span>  <br/> |<span data-ttu-id="5f3ce-127">Office-2016 32-biters er installert ved hjelp av Klikk og bruk</span><span class="sxs-lookup"><span data-stu-id="5f3ce-127">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="5f3ce-128">Eksisterende 32-biters Klikk og bruk-versjon av Office (2016 eller tidligere), og ingen frittstående apper</span><span class="sxs-lookup"><span data-stu-id="5f3ce-128">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="5f3ce-129">Ingen</span><span class="sxs-lookup"><span data-stu-id="5f3ce-129">None</span></span>  <br/> |<span data-ttu-id="5f3ce-130">Oppgradert til den nyeste 32-biters Klikk og bruk-versjonen av Office 2016, etter behov **\***</span><span class="sxs-lookup"><span data-stu-id="5f3ce-130">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="5f3ce-131">Eksisterende Klikk og bruk 32-biters versjon av Office og Klikk og bruk 32-biters eller 64-biters frittstående Office-apper (for eksempel Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="5f3ce-131">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="5f3ce-132">Ingen</span><span class="sxs-lookup"><span data-stu-id="5f3ce-132">None</span></span>  <br/> |<span data-ttu-id="5f3ce-133">Frittstående apper påvirkes ikke.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-133">Standalone apps aren't affected.</span></span> <span data-ttu-id="5f3ce-134">Programserien er oppgradert til 32-biters Klikk og bruk-versjon av Office 2016</span><span class="sxs-lookup"><span data-stu-id="5f3ce-134">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="5f3ce-135">Eksisterende 32-biters Klikk og bruk-versjon av Office og eventuelle 32- eller 64-biters (unntatt 2016) MSI frittstående Office-apper</span><span class="sxs-lookup"><span data-stu-id="5f3ce-135">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="5f3ce-136">Ingen</span><span class="sxs-lookup"><span data-stu-id="5f3ce-136">None</span></span>  <br/> |<span data-ttu-id="5f3ce-137">Frittstående apper påvirkes ikke.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-137">Standalone apps aren't affected.</span></span> <span data-ttu-id="5f3ce-138">Programserien er oppgradert til 32-biters Klikk og bruk-versjon av Office 2016</span><span class="sxs-lookup"><span data-stu-id="5f3ce-138">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="5f3ce-139">En hvilken som helst eksisterende 64-biters Klikk og bruk-versjon av Office</span><span class="sxs-lookup"><span data-stu-id="5f3ce-139">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="5f3ce-140">Avinstaller 64-biters Office-apper hvis det er ok å erstatte dem med 32-biters Office-apper</span><span class="sxs-lookup"><span data-stu-id="5f3ce-140">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="5f3ce-141">Hvis Office 64-biters apper blir fjernet, installeres 32-biters Klikk og bruk-versjonen av Office 2016</span><span class="sxs-lookup"><span data-stu-id="5f3ce-141">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="5f3ce-142">En eksisterende MSI-installasjon av Office 2016 med eller uten frittstående apper</span><span class="sxs-lookup"><span data-stu-id="5f3ce-142">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="5f3ce-143">Avinstallere MSI Office 2016.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-143">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="5f3ce-p106">32-biters versjon av Klikk og bruk av Office 2016 er installert. Ingen endring i frittstående apper</span><span class="sxs-lookup"><span data-stu-id="5f3ce-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="5f3ce-146">Eksisterende MSI-installasjon av Office 2013 (eller tidligere) og/eller frittstående Office-apper</span><span class="sxs-lookup"><span data-stu-id="5f3ce-146">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="5f3ce-147">Ingen</span><span class="sxs-lookup"><span data-stu-id="5f3ce-147">None</span></span>  <br/> |<span data-ttu-id="5f3ce-148">32-biters Klikk og bruk-versjonen av Office 2016 med den eksisterende MSI Office-installasjonen (og frittstående apper) finnes side ved side</span><span class="sxs-lookup"><span data-stu-id="5f3ce-148">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="5f3ce-149">**(\*) Obs:** Oppgrader ikke til 32-biters Klikk og bruk-versjonen av Office 2016 på grunn av en kjent feil.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-149">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="5f3ce-150">En løsning pågår.</span><span class="sxs-lookup"><span data-stu-id="5f3ce-150">A fix is in progress.</span></span> 
  
