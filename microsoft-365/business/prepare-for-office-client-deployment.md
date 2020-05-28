---
title: Klargjøre for distribusjon av Office-klient av Microsoft 365 for bedrifter
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
ms.openlocfilehash: 6f3a80be9729a3818607c0f42e2cc7ece66a07ee
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/27/2020
ms.locfileid: "44401326"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a><span data-ttu-id="29106-103">Klargjøre for distribusjon av Office-klient av Microsoft 365 for bedrifter</span><span class="sxs-lookup"><span data-stu-id="29106-103">Prepare for Office client deployment by Microsoft 365 for business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="29106-104">Klargjøre for å installere Office-programmer automatisk på klientmaskiner</span><span class="sxs-lookup"><span data-stu-id="29106-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="29106-105">Du kan bruke Microsoft 365 for bedrifter til å installere 32-biters Office-apper automatisk på Windows 10-datamaskiner og holde dem oppdatert med oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="29106-105">You can use Microsoft 365 for business to automatically install the 32-bit Office apps on Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="29106-106">Automatisk installasjon fungerer best hvis sluttbrukerens datamaskin er på Windows 10 Business og:</span><span class="sxs-lookup"><span data-stu-id="29106-106">Automatic installation works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="29106-107">Ikke har eksisterende Office-skrivebordsapper (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access og OneDrive).</span><span class="sxs-lookup"><span data-stu-id="29106-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="29106-108">eller</span><span class="sxs-lookup"><span data-stu-id="29106-108">or</span></span>
    
- <span data-ttu-id="29106-109">Har en eksisterende versjon av Klikk og bruk Office installert.</span><span class="sxs-lookup"><span data-stu-id="29106-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="29106-110">Hvis du vil finne ut om du har klikk og bruk-versjonen av Office, gå til **Fil** \> **Konto** i en hvilken som helst Office-app ( **Office Konto** i Outlook).</span><span class="sxs-lookup"><span data-stu-id="29106-110">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook).</span></span> <span data-ttu-id="29106-111">Hvis du **ser Office-oppdateringer** som vist i figuren nedenfor, ble installasjonen gjort ved hjelp av Klikk og bruk.</span><span class="sxs-lookup"><span data-stu-id="29106-111">If you see **Office Updates** as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="29106-113">**Hvem drar nytte av å ha denne funksjonen**</span><span class="sxs-lookup"><span data-stu-id="29106-113">**Who benefits from having this feature**</span></span>
  
<span data-ttu-id="29106-114">Sluttbruker med PC som:</span><span class="sxs-lookup"><span data-stu-id="29106-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="29106-115">**Har** en Windows 10 Business-brukerlisens, en aktiv Microsoft 365 for business-lisens, Windows 10 Creators Update og er koblet til Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="29106-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 for business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="29106-116">**Har ikke** 64-biters Office-apper (f.eks. Word, Excel, PowerPoint).</span><span class="sxs-lookup"><span data-stu-id="29106-116">**Doesn't have** 64-bit Office apps (example: Word, Excel, PowerPoint).</span></span> <span data-ttu-id="29106-117">Hvis 64-biters Office-apper er nødvendig, er ikke denne funksjonen god passform fordi det ikke finnes noen støtte for å utløse en 64-biters 2016 Klikk og bruk-versjon av Office fra Microsoft 365 for business admin-konsollen.</span><span class="sxs-lookup"><span data-stu-id="29106-117">If 64-bit Office apps are required, then this feature isn't a good fit because there's no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 for business admin console.</span></span> 
    
- <span data-ttu-id="29106-118">**Ikke har** noen frittstående apper for 2016 Windows Installer (MSI) (for eksempel Visio eller Project).</span><span class="sxs-lookup"><span data-stu-id="29106-118">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project).</span></span> <span data-ttu-id="29106-119">Microsoft 365 for bedrifter oppgraderer Office til Klikk og trykk-til-kjøre-versjonen av Office-2016, og som ikke fungerer med frittstående apper for Office-2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="29106-119">Microsoft 365 for business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="29106-120">Tabellen nedenfor viser hvilken handling sluttbrukerne/administratorene kanskje må utføre, avhengig av starttilstanden, for å ha en vellykket 32-biters Klikk og bruk-versjon av Office-distribusjon fra Microsoft 365 for business admin-konsollen.</span><span class="sxs-lookup"><span data-stu-id="29106-120">The following table shows what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 for business admin console.</span></span>
  
|<span data-ttu-id="29106-121">**Status for Office-installasjon før start**</span><span class="sxs-lookup"><span data-stu-id="29106-121">**Starting Office install status**</span></span>|<span data-ttu-id="29106-122">**Handling som skal iverksettes før Microsoft 365 for business Office-installasjon**</span><span class="sxs-lookup"><span data-stu-id="29106-122">**Action to take before Microsoft 365 for business Office install**</span></span>|<span data-ttu-id="29106-123">**Sluttstatus**</span><span class="sxs-lookup"><span data-stu-id="29106-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="29106-124">Ingen Office suite installert</span><span class="sxs-lookup"><span data-stu-id="29106-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="29106-125">Ingen</span><span class="sxs-lookup"><span data-stu-id="29106-125">None</span></span>  <br/> |<span data-ttu-id="29106-126">Office 2016 32-biters installeres ved hjelp av Klikk og bruk</span><span class="sxs-lookup"><span data-stu-id="29106-126">Office 2016 32-bit is installed by using Click-to-Run</span></span>  <br/> |
|<span data-ttu-id="29106-127">Eksisterende 32-biters Klikk og bruk-versjon av Office (2016 eller tidligere), og ingen frittstående apper</span><span class="sxs-lookup"><span data-stu-id="29106-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="29106-128">Ingen</span><span class="sxs-lookup"><span data-stu-id="29106-128">None</span></span>  <br/> |<span data-ttu-id="29106-129">Oppgradert til den nyeste 32-biters Klikk og bruk-versjonen av Office 2016, etter behov **\***</span><span class="sxs-lookup"><span data-stu-id="29106-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="29106-130">Eksisterende Klikk og bruk 32-biters versjon av Office og Klikk og bruk 32-biters eller 64-biters frittstående Office-apper (for eksempel Visio, Project)</span><span class="sxs-lookup"><span data-stu-id="29106-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32-bit or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="29106-131">Ingen</span><span class="sxs-lookup"><span data-stu-id="29106-131">None</span></span>  <br/> |<span data-ttu-id="29106-132">Frittstående apper påvirkes ikke.</span><span class="sxs-lookup"><span data-stu-id="29106-132">Standalone apps aren't affected.</span></span> <span data-ttu-id="29106-133">Programserien er oppgradert til 32-biters Klikk og bruk-versjon av Office 2016</span><span class="sxs-lookup"><span data-stu-id="29106-133">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="29106-134">Eksisterende 32-biters Klikk og bruk-versjon av Office og eventuelle 32- eller 64-biters (unntatt 2016) MSI frittstående Office-apper</span><span class="sxs-lookup"><span data-stu-id="29106-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="29106-135">Ingen</span><span class="sxs-lookup"><span data-stu-id="29106-135">None</span></span>  <br/> |<span data-ttu-id="29106-136">Frittstående apper påvirkes ikke.</span><span class="sxs-lookup"><span data-stu-id="29106-136">Standalone apps aren't affected.</span></span> <span data-ttu-id="29106-137">Programserien er oppgradert til 32-biters Klikk og bruk-versjon av Office 2016</span><span class="sxs-lookup"><span data-stu-id="29106-137">Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="29106-138">En hvilken som helst eksisterende 64-biters Klikk og bruk-versjon av Office</span><span class="sxs-lookup"><span data-stu-id="29106-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="29106-139">Avinstaller 64-biters Office-apper hvis det er ok å erstatte dem med 32-biters Office-apper</span><span class="sxs-lookup"><span data-stu-id="29106-139">Uninstall the 64-bit Office apps, if it's OK to replace them with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="29106-140">Hvis Office 64-biters apper blir fjernet, installeres 32-biters Klikk og bruk-versjonen av Office 2016</span><span class="sxs-lookup"><span data-stu-id="29106-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="29106-141">En eksisterende MSI-installasjon av Office 2016 med eller uten frittstående apper</span><span class="sxs-lookup"><span data-stu-id="29106-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="29106-142">Avinstallere MSI Office 2016.</span><span class="sxs-lookup"><span data-stu-id="29106-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="29106-p106">32-biters versjon av Klikk og bruk av Office 2016 er installert. Ingen endring i frittstående apper</span><span class="sxs-lookup"><span data-stu-id="29106-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="29106-145">Eksisterende MSI-installasjon av Office 2013 (eller tidligere) og/eller frittstående Office-apper</span><span class="sxs-lookup"><span data-stu-id="29106-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="29106-146">Ingen</span><span class="sxs-lookup"><span data-stu-id="29106-146">None</span></span>  <br/> |<span data-ttu-id="29106-147">32-biters Klikk og bruk-versjonen av Office 2016 med den eksisterende MSI Office-installasjonen (og frittstående apper) finnes side ved side</span><span class="sxs-lookup"><span data-stu-id="29106-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="29106-148">**(\*) Obs:** Oppgrader ikke til 32-biters Klikk og bruk-versjonen av Office 2016 på grunn av en kjent feil.</span><span class="sxs-lookup"><span data-stu-id="29106-148">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug.</span></span> <span data-ttu-id="29106-149">En løsning pågår.</span><span class="sxs-lookup"><span data-stu-id="29106-149">A fix is in progress.</span></span> 
  
