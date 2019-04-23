---
title: Bruk veiledningen som forklarer trinn for trinn hvordan du legger til AutoPilot-enheter og -profil
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Lær hvordan du bruker Windows AutoPilot til å definere nye Windows 10 enheter for bedriften.
ms.openlocfilehash: e0802ddcc0964d0b8d102f7dbdb9116b33cdcf58
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32277141"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="4077e-103">Bruk veiledningen som forklarer trinn for trinn hvordan du legger til AutoPilot-enheter og -profil</span><span class="sxs-lookup"><span data-stu-id="4077e-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="4077e-104">Du kan bruke Windows AutoPilot til å konfigurere nye Windows 10-enheter for bedriften din, slik at de er klare til produktiv bruk når du gir dem til ansatte.</span><span class="sxs-lookup"><span data-stu-id="4077e-104">You can use Windows AutoPilot to set up new Windows 10 devices for your business so they are ready for productive use as soon as you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="4077e-105">Enhetskrav</span><span class="sxs-lookup"><span data-stu-id="4077e-105">Device requirements</span></span>

<span data-ttu-id="4077e-106">Enheter må oppfylle disse kravene:</span><span class="sxs-lookup"><span data-stu-id="4077e-106">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="4077e-107">Windows 10 versjon 1703 eller senere.</span><span class="sxs-lookup"><span data-stu-id="4077e-107">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="4077e-108">Nye enheter som ikke har vært gjennom Windows out-of-box experience.</span><span class="sxs-lookup"><span data-stu-id="4077e-108">New devices that have not been through Windows out-of-box experience.</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="4077e-109">Bruk installasjonsveiledningen til å opprette enheter og profiler</span><span class="sxs-lookup"><span data-stu-id="4077e-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="4077e-110">Hvis du ikke har opprettet noen enhetsgrupper eller profiler ennå, er den beste måten å komme i gang ved hjelp av den trinnvise veiledningen, men du kan også [legge til enheter](create-and-edit-autopilot-devices.md) og [tilordne profiler](create-and-edit-autopilot-profiles.md) til dem uten å bruke veiledningen.</span><span class="sxs-lookup"><span data-stu-id="4077e-110">If you have no device groups or profiles created yet, the best way to get started is by using the step-by-step guide, but you can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="4077e-111">I Microsoft 365 Businessadministrasjonssenteret velger du **Distribuere Windows med AutoPilot** på kortet **Enhetshandlinger**.</span><span class="sxs-lookup"><span data-stu-id="4077e-111">In the Microsoft 365 Business admin center, locate the **Device actions** card, and choose **Deploy Windows with Autopilot**.</span></span>
    
    ![On the Device actions card, choose Deploy Windows with Autopilot.](media/160d5c2a-11a8-48f9-a8aa-70f084b85448.png)
  
2. <span data-ttu-id="4077e-113">Klikk eller trykk på **Startveiledning** på **Klargjøre Windows**.</span><span class="sxs-lookup"><span data-stu-id="4077e-113">On the **Prepare Windows** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="4077e-p101">Bla til der du har den klargjorte CSV-filen på siden **Last opp .csv-fil med en liste over enheter**, og velg **Åpne** \> **Neste**. Filen skal ha tre topptekster:</span><span class="sxs-lookup"><span data-stu-id="4077e-p101">On the **Upload .csv file with list of devices** page, browse to a locations where you have the prepared .CSV file, then **Open** \> **Next**. The file should have three headers:</span></span>
    
  - <span data-ttu-id="4077e-117">Kolonne A: Enhetens serienummer</span><span class="sxs-lookup"><span data-stu-id="4077e-117">Column A: Device Serial Number</span></span>
    
  - <span data-ttu-id="4077e-118">Kolonne B: Produkt-ID for Windows</span><span class="sxs-lookup"><span data-stu-id="4077e-118">Column B: Windows Product ID</span></span>
    
  - <span data-ttu-id="4077e-119">Kolonne C: Maskinvarens hash</span><span class="sxs-lookup"><span data-stu-id="4077e-119">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="4077e-120">Du får denne informasjonen fra leverandøren av maskinvaren, eller du kan bruke [Get-WindowsAutoPilotInfo PowerShell-skriptet](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), som genererer en CSV-fil.</span><span class="sxs-lookup"><span data-stu-id="4077e-120">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a CSV file.</span></span> 
    
    <span data-ttu-id="4077e-p102">Se [CSV-fil med enhetsliste](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) hvis du vil ha mer informasjon. Du kan også laste ned en eksempelfil på siden **Laste opp .csv-fil med liste over enheter**.</span><span class="sxs-lookup"><span data-stu-id="4077e-p102">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="4077e-p103">Du kan velge en eksisterende profil, eller du kan lage en ny profil, på siden **Tilordne en profil**. Hvis du ikke har en ennå, vil du bli bedt om å opprette en ny.</span><span class="sxs-lookup"><span data-stu-id="4077e-p103">On the **Assign a profile** page, you can either pick an existing profile, or create a new one. If you don't have one yet, you will be prompted to create a new one.</span></span> 
    
    <span data-ttu-id="4077e-125">En profil er en samling innstillinger som kan brukes på én enkelt enhet eller en gruppe enheter.</span><span class="sxs-lookup"><span data-stu-id="4077e-125">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="4077e-p104">Standardfunksjoner er påkrevd, og angis automatisk. Standardfunksjoner er:</span><span class="sxs-lookup"><span data-stu-id="4077e-p104">The default features are required and will be set automatically. The default features are:</span></span>
    
  - <span data-ttu-id="4077e-128">Cortana-, OneDrive- og OEM-registrering hoppes over.</span><span class="sxs-lookup"><span data-stu-id="4077e-128">Cortana, OneDrive and OEM registration is skipped.</span></span>
    
  - <span data-ttu-id="4077e-129">Opprett påloggingsopplevelse med firmamerket ditt.</span><span class="sxs-lookup"><span data-stu-id="4077e-129">Create sign-in experience with your company brand.</span></span>
    
  - <span data-ttu-id="4077e-130">Enhetene dine skal bli koblet til kontoer for Azure Active Directory, og automatisk registrert for å administreres av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="4077e-130">Your devices are going to be connected to Azure Active Directory accounts and automatically enrolled to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="4077e-131">Hvis du vil ha mer informasjon, kan du se</span><span class="sxs-lookup"><span data-stu-id="4077e-131">For more information, see</span></span>
    
    <span data-ttu-id="4077e-132">[Om innstillinger for AutoPilot-profil](autopilot-profile-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="4077e-132">[About AutoPilot Profile settings](autopilot-profile-settings.md) .</span></span> 
    
5. <span data-ttu-id="4077e-133">De andre innstillingene er **Hopp over personverninnstillinger** og **Ikke tillat brukeren å bli lokal administrator**. Dette er satt til **Av** som standard.</span><span class="sxs-lookup"><span data-stu-id="4077e-133">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="4077e-134">Velg **Neste**.</span><span class="sxs-lookup"><span data-stu-id="4077e-134">Choose **Next**.</span></span>
    
6. <span data-ttu-id="4077e-p105">Siden **Du er ferdig** indikerer at profilen du opprettet (eller valgte) brukes på den enhetsgruppen du opprettet, ved å laste opp på listen over enheter. Disse innstillingene blir aktive når enhetenes brukere senere logger på. Velg **Lukk**.</span><span class="sxs-lookup"><span data-stu-id="4077e-p105">**You're done** page indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices. These settings will be in effect when the device users sign in next. Choose **Close**.</span></span>
    