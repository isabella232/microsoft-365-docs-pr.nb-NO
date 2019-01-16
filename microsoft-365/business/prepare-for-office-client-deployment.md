---
title: Klargjøre for distribusjon av Office-klienten med Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 10/31/2017
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Lær hvordan du installerer 32-biters Office-programmer for Windows 10 datamaskiner og holde dem oppdatert automatisk.
ms.openlocfilehash: 16a8230d60157f1c6731ac639d89533b05aa3afe
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982156"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a><span data-ttu-id="54c21-103">Klargjøre for distribusjon av Office-klienten med Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="54c21-103">Prepare for Office client deployment by Microsoft 365 Business</span></span>

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a><span data-ttu-id="54c21-104">Klargjøre for å installere Office-programmer automatisk på klientmaskiner</span><span class="sxs-lookup"><span data-stu-id="54c21-104">Prepare to automatically install Office apps to client computers</span></span>

<span data-ttu-id="54c21-105">Du kan bruke Microsoft 365 Business for automatisk å installere 32-biters Office-appene på datamaskiner med Windows 10 og for å holde dem automatisk oppdatert med oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="54c21-105">You can use Microsoft 365 Business to automatically install the 32-bit Office apps to Windows 10 computers and keep them current with updates.</span></span>
  
<span data-ttu-id="54c21-106">Dette fungerer best hvis sluttbrukerens datamaskin bruker Windows 10 Business og:</span><span class="sxs-lookup"><span data-stu-id="54c21-106">This works best if the end user's computer is on Windows 10 Business and:</span></span>
  
- <span data-ttu-id="54c21-107">Ikke har eksisterende Office-skrivebordsapper (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access og OneDrive).</span><span class="sxs-lookup"><span data-stu-id="54c21-107">Doesn't have existing Office desktop apps (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access, and OneDrive).</span></span>
    
    <span data-ttu-id="54c21-108">eller</span><span class="sxs-lookup"><span data-stu-id="54c21-108">or</span></span>
    
- <span data-ttu-id="54c21-109">Har en eksisterende versjon av Klikk og bruk Office installert.</span><span class="sxs-lookup"><span data-stu-id="54c21-109">Has an existing version of Click-to-Run Office installed.</span></span>
    
<span data-ttu-id="54c21-p101">Hvis du vil finne ut om du har klikk og bruk-versjonen av Office, gå til **Fil** \> **Konto** i en hvilken som helst Office-app ( **Office Konto** i Outlook). Hvis du ser Office-oppdateringer som vist i figuren nedenfor, ble installasjonen utført ved hjelp av Klikk og bruk.</span><span class="sxs-lookup"><span data-stu-id="54c21-p101">To determine if you have the Click-to-Run version of Office, in any Office app go to **File** \> **Account** ( **Office Account** in Outlook). If you see Office Updates as shown in the following figure, then the installation was done by using Click-to-Run.</span></span> 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 <span data-ttu-id="54c21-113">**Hvem vil dra nytte av denne funksjonen**</span><span class="sxs-lookup"><span data-stu-id="54c21-113">**Who will benefit from having this feature**</span></span>
  
<span data-ttu-id="54c21-114">Sluttbruker med PC som:</span><span class="sxs-lookup"><span data-stu-id="54c21-114">The end user whose PC:</span></span>
  
- <span data-ttu-id="54c21-115">**Har** brukerlisens for Windows 10 Business, en aktiv Microsoft 365 Business-lisens, Windows 10 Creators Update og er knyttet til Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="54c21-115">**Has**  a Windows 10 Business user license, an active Microsoft 365 Business license, Windows 10 Creators Update, and is joined to Azure Active Directory.</span></span> 
    
- <span data-ttu-id="54c21-p102">**Ikke har** 64-biters Office-apper (for eksempel: Word, Excel og PowerPoint). Hvis 64-biters Office-apper er påkrevd, er denne funksjonen ikke å anbefale fordi det ikke er noen støtte for å utløse en 64-biters 2016 Klikk og bruk-versjon av Office fra Microsoft 365 Business-administrasjonskonsollen.</span><span class="sxs-lookup"><span data-stu-id="54c21-p102">**Doesn't have** 64-bit Office apps (example: Word, Excel, Powerpoint). If 64-bit Office apps are required, then this feature is not a good fit because there is no support for triggering a 64-bit 2016 Click-to-Run version of Office from the Microsoft 365 Business admin console.</span></span> 
    
- <span data-ttu-id="54c21-p103">**Ikke har** noen frittstående apper for 2016 Windows Installer (MSI) (for eksempel Visio eller Project). Microsoft 365 Business oppgraderer Office til Klikk og bruk-versjonen av Office 2016, og det fungerer ikke med frittstående apper for Office 2016 MSI.</span><span class="sxs-lookup"><span data-stu-id="54c21-p103">**Doesn't have** any 2016 Windows Installer (MSI) standalone apps (for example, Visio or Project). Microsoft 365 Business upgrades Office to the Click-to-Run version of Office 2016 and that doesn't work with with Office 2016 MSI standalone apps.</span></span> 
    
<span data-ttu-id="54c21-120">I tabellen nedenfor finner du detaljert informasjon om hvilken handling sluttbrukere/administratorer må utføre, avhengig av startstatus, for å få en vellykket 32-biters Klikk og bruk-versjon av Office-distribusjon fra Microsoft 365 Business-administrasjonskonsollen.</span><span class="sxs-lookup"><span data-stu-id="54c21-120">The following table details what action the end users/admins may need to take, depending on their beginning state, to have a successful 32-bit Click-to-Run version of Office deployment from the Microsoft 365 Business admin console.</span></span>
  
|<span data-ttu-id="54c21-121">**Status for Office-installasjon før start**</span><span class="sxs-lookup"><span data-stu-id="54c21-121">**Starting Office install status**</span></span>|<span data-ttu-id="54c21-122">**Handling som skal utføres før Microsoft 365 Business-Office-installasjon**</span><span class="sxs-lookup"><span data-stu-id="54c21-122">**Action to take before Microsoft 365 Business Office install**</span></span>|<span data-ttu-id="54c21-123">**Sluttstatus**</span><span class="sxs-lookup"><span data-stu-id="54c21-123">**End state**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="54c21-124">Ingen Office suite installert</span><span class="sxs-lookup"><span data-stu-id="54c21-124">No Office suite installed</span></span>  <br/> |<span data-ttu-id="54c21-125">Ingen</span><span class="sxs-lookup"><span data-stu-id="54c21-125">None</span></span>  <br/> |<span data-ttu-id="54c21-126">Office 2016 32-biters er installert ved hjelp av Klikk og bruk</span><span class="sxs-lookup"><span data-stu-id="54c21-126">Office 2016 32-bit is installed by using click-to-run</span></span>  <br/> |
|<span data-ttu-id="54c21-127">Eksisterende 32-biters Klikk og bruk-versjon av Office (2016 eller tidligere), og ingen frittstående apper</span><span class="sxs-lookup"><span data-stu-id="54c21-127">Existing Click-to-Run 32-bit version of Office (2016 or earlier) and no standalone apps</span></span>  <br/> |<span data-ttu-id="54c21-128">Ingen</span><span class="sxs-lookup"><span data-stu-id="54c21-128">None</span></span>  <br/> |<span data-ttu-id="54c21-129">Oppgradert til den nyeste 32-biters Klikk og bruk-versjonen av Office 2016, etter behov **\***</span><span class="sxs-lookup"><span data-stu-id="54c21-129">Upgraded to the latest 32-bit Click-to-Run version of Office 2016, as needed **\***</span></span> <br/> |
|<span data-ttu-id="54c21-130">Eksisterende 32-biters Klikk og bruk-versjon av Office samt 32 - eller 64-biters frittstående Office-apper (for eksempel Visio og Project)</span><span class="sxs-lookup"><span data-stu-id="54c21-130">Existing Click-to-Run 32-bit version of Office and Click-to-Run 32- or 64-bit standalone Office apps (for example, Visio, Project)</span></span>  <br/> |<span data-ttu-id="54c21-131">Ingen</span><span class="sxs-lookup"><span data-stu-id="54c21-131">None</span></span>  <br/> |<span data-ttu-id="54c21-p104">Frittstående apper berøres ikke. Programserien er oppgradert til 32-biters Klikk og bruk-versjon av Office 2016</span><span class="sxs-lookup"><span data-stu-id="54c21-p104">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> |
|<span data-ttu-id="54c21-134">Eksisterende 32-biters Klikk og bruk-versjon av Office og eventuelle 32- eller 64-biters (unntatt 2016) MSI frittstående Office-apper</span><span class="sxs-lookup"><span data-stu-id="54c21-134">Existing Click-to-Run 32-bit version of Office and any 32-bit or 64-bit (except 2016) MSI standalone Office apps</span></span>  <br/> |<span data-ttu-id="54c21-135">Ingen</span><span class="sxs-lookup"><span data-stu-id="54c21-135">None</span></span>  <br/> |<span data-ttu-id="54c21-p105">Frittstående apper berøres ikke. Programserien er oppgradert til 32-biters Klikk og bruk-versjon av Office 2016</span><span class="sxs-lookup"><span data-stu-id="54c21-p105">Standalone apps are not affected. Suite is upgraded to Click-to-Run 32-bit version of Office 2016</span></span>  <br/> ||||
|<span data-ttu-id="54c21-138">En hvilken som helst eksisterende 64-biters Klikk og bruk-versjon av Office</span><span class="sxs-lookup"><span data-stu-id="54c21-138">Any existing Click-to-Run 64-bit version of Office</span></span>  <br/> |<span data-ttu-id="54c21-139">Avinstaller 64-biters Office-apper hvis det er greit å erstatte dem med 32-biters Office-apper</span><span class="sxs-lookup"><span data-stu-id="54c21-139">Uninstall the 64-bit Office apps, if it is OK to replace it with 32-bit Office apps</span></span>  <br/> |<span data-ttu-id="54c21-140">Hvis Office 64-biters apper blir fjernet, installeres 32-biters Klikk og bruk-versjonen av Office 2016</span><span class="sxs-lookup"><span data-stu-id="54c21-140">If Office 64-bit apps are removed, the Click-to-Run 32-bit version of Office 2016 is installed</span></span>  <br/> |
|<span data-ttu-id="54c21-141">En eksisterende MSI-installasjon av Office 2016 med eller uten frittstående apper</span><span class="sxs-lookup"><span data-stu-id="54c21-141">An existing MSI install of Office 2016 with or without standalone apps</span></span>  <br/> |<span data-ttu-id="54c21-142">Avinstallere MSI Office 2016.</span><span class="sxs-lookup"><span data-stu-id="54c21-142">Uninstall MSI Office 2016.</span></span>  <br/> |<span data-ttu-id="54c21-p106">32-biters versjon av Klikk og bruk av Office 2016 er installert. Ingen endring i frittstående apper</span><span class="sxs-lookup"><span data-stu-id="54c21-p106">Click-to-Run 32-bit version of Office 2016 is installed. No change to standalone apps</span></span>  <br/> |
|<span data-ttu-id="54c21-145">Eksisterende MSI-installasjon av Office 2013 (eller tidligere) og/eller frittstående Office-apper</span><span class="sxs-lookup"><span data-stu-id="54c21-145">Existing MSI install of Office 2013 (or earlier) and/or standalone Office apps</span></span>  <br/> |<span data-ttu-id="54c21-146">Ingen</span><span class="sxs-lookup"><span data-stu-id="54c21-146">None</span></span>  <br/> |<span data-ttu-id="54c21-147">32-biters Klikk og bruk-versjonen av Office 2016 med den eksisterende MSI Office-installasjonen (og frittstående apper) finnes side ved side</span><span class="sxs-lookup"><span data-stu-id="54c21-147">Click-to-Run 32-bit version of Office 2016 with the pre-existing MSI Office install (and standalone apps) exist side-by-side</span></span>  <br/> |
||||
   
 <span data-ttu-id="54c21-p107">**(\*) Obs:** Oppgrader ikke til 32-biters Klikk og bruk-versjonen av Office 2016 på grunn av en kjent feil. Rettelse pågår.</span><span class="sxs-lookup"><span data-stu-id="54c21-p107">**(\*) Note:** Does not upgrade to Click-to-Run 32-bit version of Office 2016 due to a known bug. Fix is in progress.</span></span> 
  


