---
title: Bruk veiledningen som forklarer trinn for trinn hvordan du legger til AutoPilot-enheter og -profil
f1.keywords:
- NOCSH
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Finn ut hvordan du bruker Windows AutoPilot til å konfigurere nye Windows 10-enheter for bedriften din.
ms.openlocfilehash: 1fd0abb76d16b79dd11ef27b6b27a87894d89ef9
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593277"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="3c941-103">Bruk veiledningen som forklarer trinn for trinn hvordan du legger til AutoPilot-enheter og -profil</span><span class="sxs-lookup"><span data-stu-id="3c941-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="3c941-104">Du kan bruke Windows AutoPilot til å konfigurere **nye** Windows 10-enheter for bedriften, slik at de er klare til bruk når du gir dem til de ansatte.</span><span class="sxs-lookup"><span data-stu-id="3c941-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="3c941-105">Enhetskrav</span><span class="sxs-lookup"><span data-stu-id="3c941-105">Device requirements</span></span>

<span data-ttu-id="3c941-106">Enheter må oppfylle disse kravene:</span><span class="sxs-lookup"><span data-stu-id="3c941-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="3c941-107">Windows 10, versjon 1703 eller nyere</span><span class="sxs-lookup"><span data-stu-id="3c941-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="3c941-108">Nye enheter som ikke har vært gjennom Windows-opplevelsen</span><span class="sxs-lookup"><span data-stu-id="3c941-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="3c941-109">Bruk installasjonsveiledningen til å opprette enheter og profiler</span><span class="sxs-lookup"><span data-stu-id="3c941-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="3c941-110">[![Etikett for å gi deg beskjed om at administrasjonssenteret endres. Du finner mer informasjon på aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span><span class="sxs-lookup"><span data-stu-id="3c941-110">[![Label to let you know the admin center is changing and you can find more details at aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)</span></span>

<span data-ttu-id="3c941-111">Hvis du ikke har opprettet enhetsgrupper eller profiler ennå, er den beste måten å komme i gang på ved å bruke den trinnvise veiledningen.</span><span class="sxs-lookup"><span data-stu-id="3c941-111">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="3c941-112">Du kan også [legge til enheter](create-and-edit-autopilot-devices.md) og tilordne [profiler](create-and-edit-autopilot-profiles.md) til dem uten å bruke veiledningen.</span><span class="sxs-lookup"><span data-stu-id="3c941-112">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="3c941-113">Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>på .</span><span class="sxs-lookup"><span data-stu-id="3c941-113">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="3c941-114">Velg **Enheter** \> **AutoPilot**i navigasjonsruten til venstre.</span><span class="sxs-lookup"><span data-stu-id="3c941-114">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![Velg enheter og deretter AutoPilot i administrasjonssenteret.](media/AutoPilot.png)
  
2. <span data-ttu-id="3c941-116">Klikk eller trykk **startveiledning**på **AutoPilot-siden.**</span><span class="sxs-lookup"><span data-stu-id="3c941-116">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="3c941-118">Bla \*\*\*\* til en plassering der du har forberedt . CSV-fil, og **deretter Åpne** \> **Neste**.</span><span class="sxs-lookup"><span data-stu-id="3c941-118">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="3c941-119">Filen må ha tre overskrifter:</span><span class="sxs-lookup"><span data-stu-id="3c941-119">The file must have three headers:</span></span>
    
    - <span data-ttu-id="3c941-120">Kolonne A: Enhetens serienummer</span><span class="sxs-lookup"><span data-stu-id="3c941-120">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="3c941-121">Kolonne B: Produkt-ID for Windows</span><span class="sxs-lookup"><span data-stu-id="3c941-121">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="3c941-122">Kolonne C: Maskinvarens hash</span><span class="sxs-lookup"><span data-stu-id="3c941-122">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="3c941-123">Du kan få denne informasjonen fra maskinvareleverandøren, eller du kan bruke [Get-WindowsAutoPilotInfo PowerShell-skriptet](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) til å generere en CSV-fil.</span><span class="sxs-lookup"><span data-stu-id="3c941-123">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="3c941-p103">Se [CSV-fil med enhetsliste](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) hvis du vil ha mer informasjon. Du kan også laste ned en eksempelfil på siden **Laste opp .csv-fil med liste over enheter**.</span><span class="sxs-lookup"><span data-stu-id="3c941-p103">For more information, see [Device list CSV-file](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
4. <span data-ttu-id="3c941-126">På **tilordne en profil-siden** kan du enten velge en eksisterende profil eller opprette en ny.</span><span class="sxs-lookup"><span data-stu-id="3c941-126">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="3c941-127">Hvis du ikke har en ennå, blir du bedt om å opprette en.</span><span class="sxs-lookup"><span data-stu-id="3c941-127">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="3c941-128">En profil er en samling innstillinger som kan brukes på én enkelt enhet eller en gruppe enheter.</span><span class="sxs-lookup"><span data-stu-id="3c941-128">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="3c941-129">Standardfunksjonene kreves og angis automatisk.</span><span class="sxs-lookup"><span data-stu-id="3c941-129">The default features are required and are set automatically.</span></span> <span data-ttu-id="3c941-130">Standardfunksjoner er:</span><span class="sxs-lookup"><span data-stu-id="3c941-130">The default features are:</span></span>
    
    - <span data-ttu-id="3c941-131">Hopp over Cortana-, OneDrive- og OEM-registrering.</span><span class="sxs-lookup"><span data-stu-id="3c941-131">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="3c941-132">Opprett påloggingsopplevelse med firmamerket ditt.</span><span class="sxs-lookup"><span data-stu-id="3c941-132">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="3c941-133">Koble enhetene dine til Azure Active Directory-kontoer, og registrer dem automatisk for å administreres av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="3c941-133">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business.</span></span>
    
    <span data-ttu-id="3c941-134">Hvis du vil ha mer informasjon, kan du se Om innstillinger for [AutoPilot-profil](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="3c941-134">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="3c941-135">De andre innstillingene er **Hopp over personverninnstillinger** og **Ikke tillat brukeren å bli lokal administrator**. Dette er satt til **Av** som standard.</span><span class="sxs-lookup"><span data-stu-id="3c941-135">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="3c941-136">Velg **Neste**.</span><span class="sxs-lookup"><span data-stu-id="3c941-136">Choose **Next**.</span></span>
    
6. <span data-ttu-id="3c941-137">**Du er ferdig,** og angir at profilen du opprettet (eller valgte) skal brukes på enhetsgruppen du opprettet, ved å laste opp listen over enheter.</span><span class="sxs-lookup"><span data-stu-id="3c941-137">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="3c941-138">Innstillingene trer i kraft når enhetsbrukerne logger på neste.</span><span class="sxs-lookup"><span data-stu-id="3c941-138">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="3c941-139">Velg **Lukk**.</span><span class="sxs-lookup"><span data-stu-id="3c941-139">Choose **Close**.</span></span>
    