---
title: Bruk veiledningen som forklarer trinn for trinn hvordan du legger til AutoPilot-enheter og -profil
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
ms.openlocfilehash: 9a70978156fb26ac3aad08f1758b7ee125067d38
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072154"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="64a9c-103">Bruk veiledningen som forklarer trinn for trinn hvordan du legger til AutoPilot-enheter og -profil</span><span class="sxs-lookup"><span data-stu-id="64a9c-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="64a9c-104">Du kan bruke Windows AutoPilot for å konfigurere **nye** Windows 10 enheter for bedriften slik at de er klare for produktiv Bruk så snart du gir dem til ansatte.</span><span class="sxs-lookup"><span data-stu-id="64a9c-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they are ready for productive use as soon as you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="64a9c-105">Enhetskrav</span><span class="sxs-lookup"><span data-stu-id="64a9c-105">Device requirements</span></span>

<span data-ttu-id="64a9c-106">Enheter må oppfylle disse kravene:</span><span class="sxs-lookup"><span data-stu-id="64a9c-106">Devices need to meet these requirements:</span></span>
  
- <span data-ttu-id="64a9c-107">Windows 10 versjon 1703 eller senere.</span><span class="sxs-lookup"><span data-stu-id="64a9c-107">Windows 10, version 1703 or later.</span></span>
    
- <span data-ttu-id="64a9c-108">Nye enheter som ikke har vært gjennom Windows out-of-box experience.</span><span class="sxs-lookup"><span data-stu-id="64a9c-108">New devices that have not been through Windows out-of-box experience.</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="64a9c-109">Bruk installasjonsveiledningen til å opprette enheter og profiler</span><span class="sxs-lookup"><span data-stu-id="64a9c-109">Use the setup guide to create devices and profiles</span></span>

![Banner som peker til https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

<span data-ttu-id="64a9c-111">Hvis du ikke har opprettet noen enhetsgrupper eller profiler ennå, er den beste måten å komme i gang ved hjelp av den trinnvise veiledningen, men du kan også [legge til enheter](create-and-edit-autopilot-devices.md) og [tilordne profiler](create-and-edit-autopilot-profiles.md) til dem uten å bruke veiledningen.</span><span class="sxs-lookup"><span data-stu-id="64a9c-111">If you have no device groups or profiles created yet, the best way to get started is by using the step-by-step guide, but you can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="64a9c-112">Gå til administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="64a9c-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="64a9c-113">Velg **enheter** på venstre nav \> **AutoPilot**.</span><span class="sxs-lookup"><span data-stu-id="64a9c-113">On the left nav choose **Devices** \> **AutoPilot**.</span></span>

    ![Velg enheter og AutoPilot i administrasjonssenteret.](media/AutoPilot.png)
  
2. <span data-ttu-id="64a9c-115">På siden **AutoPilot** klikke eller tappe **Start guide**.</span><span class="sxs-lookup"><span data-stu-id="64a9c-115">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="64a9c-p101">Bla til der du har den klargjorte CSV-filen på siden **Last opp .csv-fil med en liste over enheter**, og velg **Åpne** \> **Neste**. Filen skal ha tre topptekster:</span><span class="sxs-lookup"><span data-stu-id="64a9c-p101">On the **Upload .csv file with list of devices** page, browse to a locations where you have the prepared .CSV file, then **Open** \> **Next**. The file should have three headers:</span></span>
    
  - <span data-ttu-id="64a9c-119">Kolonne A: Enhetens serienummer</span><span class="sxs-lookup"><span data-stu-id="64a9c-119">Column A: Device Serial Number</span></span>
    
  - <span data-ttu-id="64a9c-120">Kolonne B: Produkt-ID for Windows</span><span class="sxs-lookup"><span data-stu-id="64a9c-120">Column B: Windows Product ID</span></span>
    
  - <span data-ttu-id="64a9c-121">Kolonne C: Maskinvarens hash</span><span class="sxs-lookup"><span data-stu-id="64a9c-121">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="64a9c-122">Du får denne informasjonen fra leverandøren av maskinvaren, eller du kan bruke [Get-WindowsAutoPilotInfo PowerShell-skriptet](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), som genererer en CSV-fil.</span><span class="sxs-lookup"><span data-stu-id="64a9c-122">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) that will generate a CSV file.</span></span> 
    
    <span data-ttu-id="64a9c-p102">Se [CSV-fil med enhetsliste](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) hvis du vil ha mer informasjon. Du kan også laste ned en eksempelfil på siden **Laste opp .csv-fil med liste over enheter**.</span><span class="sxs-lookup"><span data-stu-id="64a9c-p102">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="64a9c-p103">Du kan velge en eksisterende profil, eller du kan lage en ny profil, på siden **Tilordne en profil**. Hvis du ikke har en ennå, vil du bli bedt om å opprette en ny.</span><span class="sxs-lookup"><span data-stu-id="64a9c-p103">On the **Assign a profile** page, you can either pick an existing profile, or create a new one. If you don't have one yet, you will be prompted to create a new one.</span></span> 
    
    <span data-ttu-id="64a9c-127">En profil er en samling innstillinger som kan brukes på én enkelt enhet eller en gruppe enheter.</span><span class="sxs-lookup"><span data-stu-id="64a9c-127">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="64a9c-p104">Standardfunksjoner er påkrevd, og angis automatisk. Standardfunksjoner er:</span><span class="sxs-lookup"><span data-stu-id="64a9c-p104">The default features are required and will be set automatically. The default features are:</span></span>
    
  - <span data-ttu-id="64a9c-130">Cortana-, OneDrive- og OEM-registrering hoppes over.</span><span class="sxs-lookup"><span data-stu-id="64a9c-130">Cortana, OneDrive and OEM registration is skipped.</span></span>
    
  - <span data-ttu-id="64a9c-131">Opprett påloggingsopplevelse med firmamerket ditt.</span><span class="sxs-lookup"><span data-stu-id="64a9c-131">Create sign-in experience with your company brand.</span></span>
    
  - <span data-ttu-id="64a9c-132">Enhetene dine skal bli koblet til kontoer for Azure Active Directory, og automatisk registrert for å administreres av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="64a9c-132">Your devices are going to be connected to Azure Active Directory accounts and automatically enrolled to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="64a9c-133">Hvis du vil ha mer informasjon, kan du se</span><span class="sxs-lookup"><span data-stu-id="64a9c-133">For more information, see</span></span>
    
    <span data-ttu-id="64a9c-134">[Om innstillinger for AutoPilot-profil](autopilot-profile-settings.md) .</span><span class="sxs-lookup"><span data-stu-id="64a9c-134">[About AutoPilot Profile settings](autopilot-profile-settings.md) .</span></span> 
    
5. <span data-ttu-id="64a9c-135">De andre innstillingene er **Hopp over personverninnstillinger** og **Ikke tillat brukeren å bli lokal administrator**. Dette er satt til **Av** som standard.</span><span class="sxs-lookup"><span data-stu-id="64a9c-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="64a9c-136">Velg **Neste**.</span><span class="sxs-lookup"><span data-stu-id="64a9c-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="64a9c-p105">Siden **Du er ferdig** indikerer at profilen du opprettet (eller valgte) brukes på den enhetsgruppen du opprettet, ved å laste opp på listen over enheter. Disse innstillingene blir aktive når enhetenes brukere senere logger på. Velg **Lukk**.</span><span class="sxs-lookup"><span data-stu-id="64a9c-p105">**You're done** page indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices. These settings will be in effect when the device users sign in next. Choose **Close**.</span></span>
    