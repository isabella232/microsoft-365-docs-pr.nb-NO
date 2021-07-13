---
title: Bruk veiledningen som forklarer trinn for trinn hvordan du legger til AutoPilot-enheter og -profil
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- seo-marvel-mar
- AdminSurgePortfolio
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Lær hvordan du bruker Windows AutoPilot til å Windows 10 nye enheter for bedriften, slik at de er klare til bruk for ansatte.
ms.openlocfilehash: f160ddcd1e41bd44c908ecc8bbd30a9819f76902
ms.sourcegitcommit: 00f001019c653269d85718d410f970887d904304
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/12/2021
ms.locfileid: "53393443"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a><span data-ttu-id="2fbab-103">Bruk veiledningen som forklarer trinn for trinn hvordan du legger til AutoPilot-enheter og -profil</span><span class="sxs-lookup"><span data-stu-id="2fbab-103">Use the step-by-step guide to add Autopilot devices and profile</span></span>

<span data-ttu-id="2fbab-104">Du kan bruke Windows AutoPilot til å konfigurere nye **Windows 10** enheter for bedriften, slik at de er klare til bruk når du gir dem til de ansatte.</span><span class="sxs-lookup"><span data-stu-id="2fbab-104">You can use Windows AutoPilot to set up **new** Windows 10 devices for your business so they're ready for use when you give them to your employees.</span></span>
  
## <a name="device-requirements"></a><span data-ttu-id="2fbab-105">Enhetskrav</span><span class="sxs-lookup"><span data-stu-id="2fbab-105">Device requirements</span></span>

<span data-ttu-id="2fbab-106">Enheter må oppfylle disse kravene:</span><span class="sxs-lookup"><span data-stu-id="2fbab-106">Devices must meet these requirements:</span></span>
  
- <span data-ttu-id="2fbab-107">Windows 10, versjon 1703 eller nyere</span><span class="sxs-lookup"><span data-stu-id="2fbab-107">Windows 10, version 1703 or later</span></span>
    
- <span data-ttu-id="2fbab-108">Nye enheter som ikke har vært gjennom Windows en ut-av-boks-opplevelse</span><span class="sxs-lookup"><span data-stu-id="2fbab-108">New devices that haven't been through Windows out-of-box experience</span></span>
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a><span data-ttu-id="2fbab-109">Bruk installasjonsveiledningen til å opprette enheter og profiler</span><span class="sxs-lookup"><span data-stu-id="2fbab-109">Use the setup guide to create devices and profiles</span></span>

<span data-ttu-id="2fbab-110">Hvis du ikke har opprettet enhetsgrupper eller profiler ennå, er den beste måten å komme i gang på ved hjelp av den trinnvise veiledningen.</span><span class="sxs-lookup"><span data-stu-id="2fbab-110">If you haven't created device groups or profiles yet, the best way to get started is by using the step-by-step guide.</span></span> <span data-ttu-id="2fbab-111">Du kan også [legge til enheter](create-and-edit-autopilot-devices.md) og tilordne [profiler](create-and-edit-autopilot-profiles.md) til dem uten å bruke veiledningen.</span><span class="sxs-lookup"><span data-stu-id="2fbab-111">You can also [add devices](create-and-edit-autopilot-devices.md) and [assign profiles](create-and-edit-autopilot-profiles.md) to them without using the guide.</span></span> 
  
1. <span data-ttu-id="2fbab-112">Gå til administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="2fbab-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>

2. <span data-ttu-id="2fbab-113">Velg Enheter AutoPilot  i den venstre \> **navigasjonsruten.**</span><span class="sxs-lookup"><span data-stu-id="2fbab-113">On the left navigation pane, choose **Devices** \> **AutoPilot**.</span></span>

    ![Velg enheter i administrasjonssenteret, og velg deretter AutoPilot.](../media/AutoPilot.png)
  
2. <span data-ttu-id="2fbab-115">Klikk eller **trykk startveiledning på AutoPilot-siden.** </span><span class="sxs-lookup"><span data-stu-id="2fbab-115">On the **AutoPilot** page, click or tap **Start guide**.</span></span>
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. <span data-ttu-id="2fbab-117">Gå **Upload .csv en fil** med liste over enheter på siden for å gå til en plassering der du har den .CSV filen, og deretter **åpne** \> **Neste**.</span><span class="sxs-lookup"><span data-stu-id="2fbab-117">On the **Upload .csv file with list of devices** page, browse to a location where you have the prepared .CSV file, then **Open** \> **Next**.</span></span> <span data-ttu-id="2fbab-118">Filen må ha tre overskrifter:</span><span class="sxs-lookup"><span data-stu-id="2fbab-118">The file must have three headers:</span></span>
    
    - <span data-ttu-id="2fbab-119">Kolonne A: Enhetens serienummer</span><span class="sxs-lookup"><span data-stu-id="2fbab-119">Column A: Device Serial Number</span></span>
    
    - <span data-ttu-id="2fbab-120">Kolonne B: Produkt-ID for Windows</span><span class="sxs-lookup"><span data-stu-id="2fbab-120">Column B: Windows Product ID</span></span>
    
    - <span data-ttu-id="2fbab-121">Kolonne C: Maskinvarens hash</span><span class="sxs-lookup"><span data-stu-id="2fbab-121">Column C: Hardware Hash</span></span>
    
    <span data-ttu-id="2fbab-122">Du kan få denne informasjonen fra maskinvareleverandøren, eller du kan bruke [Get-WindowsAutoPilotInfo PowerShell-skriptet](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) til å generere en CSV-fil.</span><span class="sxs-lookup"><span data-stu-id="2fbab-122">You can get this information from your hardware vendor, or you can use the [Get-WindowsAutoPilotInfo PowerShell script](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) to generate a CSV file.</span></span> 
    
    <span data-ttu-id="2fbab-p103">Se [CSV-fil med enhetsliste](../admin/misc/device-list.md) hvis du vil ha mer informasjon. Du kan også laste ned en eksempelfil på siden **Laste opp .csv-fil med liste over enheter**.</span><span class="sxs-lookup"><span data-stu-id="2fbab-p103">For more information, see [Device list CSV-file](../admin/misc/device-list.md). You can also download a sample file on the **Upload .csv file with list of devices** page.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="2fbab-125">Dette skriptet bruker WMI til å hente egenskaper som en kunde trenger for å registrere en enhet Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2fbab-125">This script uses WMI to retrieve properties needed for a customer to register a device with Windows Autopilot.</span></span> <span data-ttu-id="2fbab-126">Vær oppmerksom på at det er vanlig at den resulterende CSV-filen ikke samler inn en Windows-produkt-ID (PKID) fordi dette ikke er nødvendig for å registrere en enhet og PKID som NULL i utdata-CSV er helt greit.</span><span class="sxs-lookup"><span data-stu-id="2fbab-126">Note that it is normal for the resulting CSV file to not collect a Windows Product ID (PKID) value since this is not required to register a device and PKID being NULL in the output CSV is totally fine.</span></span> <span data-ttu-id="2fbab-127">Bare serienummeret og maskinvarenummeret fylles ut.</span><span class="sxs-lookup"><span data-stu-id="2fbab-127">Only the serial number and hardware hash will be populated.</span></span>
    
4. <span data-ttu-id="2fbab-128">På siden **Tilordne en profil** kan du enten velge en eksisterende profil eller opprette en ny.</span><span class="sxs-lookup"><span data-stu-id="2fbab-128">On the **Assign a profile** page, you can either pick an existing profile or create a new one.</span></span> <span data-ttu-id="2fbab-129">Hvis du ikke har en ennå, blir du bedt om å opprette en.</span><span class="sxs-lookup"><span data-stu-id="2fbab-129">If you don't have one yet, you'll be prompted to create one.</span></span> 
    
    <span data-ttu-id="2fbab-130">En profil er en samling innstillinger som kan brukes på én enkelt enhet eller en gruppe enheter.</span><span class="sxs-lookup"><span data-stu-id="2fbab-130">A profile is a collection of settings that can be applied to a single device or to a group of devices.</span></span>
    
    <span data-ttu-id="2fbab-131">Standardfunksjonene er obligatoriske og angis automatisk.</span><span class="sxs-lookup"><span data-stu-id="2fbab-131">The default features are required and are set automatically.</span></span> <span data-ttu-id="2fbab-132">Standardfunksjoner er:</span><span class="sxs-lookup"><span data-stu-id="2fbab-132">The default features are:</span></span>
    
    - <span data-ttu-id="2fbab-133">Hopp Cortana, OneDrive og OEM-registrering.</span><span class="sxs-lookup"><span data-stu-id="2fbab-133">Skip Cortana, OneDrive, and OEM registration.</span></span>
    
    - <span data-ttu-id="2fbab-134">Opprett påloggingsopplevelse med firmamerket ditt.</span><span class="sxs-lookup"><span data-stu-id="2fbab-134">Create sign-in experience with your company brand.</span></span>
    
    - <span data-ttu-id="2fbab-135">Koble til enhetene til å Azure Active Directory kontoer, og registrere dem automatisk for å bli administrert av Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="2fbab-135">Connect your devices to Azure Active Directory accounts, and automatically enroll them to be managed by Microsoft 365 Business Premium.</span></span>
    
    <span data-ttu-id="2fbab-136">Hvis du vil ha mer informasjon, [kan du se Om innstillinger for AutoPilot-profil](autopilot-profile-settings.md).</span><span class="sxs-lookup"><span data-stu-id="2fbab-136">For more information, see [About AutoPilot Profile settings](autopilot-profile-settings.md).</span></span> 
    
5. <span data-ttu-id="2fbab-137">De andre innstillingene er **Hopp over personverninnstillinger** og **Ikke tillat brukeren å bli lokal administrator**. Dette er satt til **Av** som standard.</span><span class="sxs-lookup"><span data-stu-id="2fbab-137">The other settings are **Skip privacy settings** and **Don't allow user to become the local admin**. These are both set to **Off** by default.</span></span> 
    
    <span data-ttu-id="2fbab-138">Velg **Neste**.</span><span class="sxs-lookup"><span data-stu-id="2fbab-138">Choose **Next**.</span></span>
    
6. <span data-ttu-id="2fbab-139">**Du er ferdig angir** at profilen du opprettet (eller valgte) vil bli brukt på enhetsgruppen du opprettet ved å laste opp listen over enheter.</span><span class="sxs-lookup"><span data-stu-id="2fbab-139">**You're done** indicates that the profile you created (or chose) will be applied to the device group you created by uploading the list of devices.</span></span> <span data-ttu-id="2fbab-140">Innstillingene trer i kraft når brukerne av enheten logger på neste gang.</span><span class="sxs-lookup"><span data-stu-id="2fbab-140">The settings will be in effect when the device users sign in next.</span></span> <span data-ttu-id="2fbab-141">Velg **Lukk**.</span><span class="sxs-lookup"><span data-stu-id="2fbab-141">Choose **Close**.</span></span>

## <a name="related-content"></a><span data-ttu-id="2fbab-142">Beslektet innhold</span><span class="sxs-lookup"><span data-stu-id="2fbab-142">Related content</span></span>

<span data-ttu-id="2fbab-143">[Om innstillinger for AutoPilot-profil](autopilot-profile-settings.md) (artikkel)</span><span class="sxs-lookup"><span data-stu-id="2fbab-143">[About AutoPilot Profile settings](autopilot-profile-settings.md) (article)</span></span>\
<span data-ttu-id="2fbab-144">[Alternativer for å beskytte enheter og appdata](../admin/devices/choose-device-security.md) (artikkel)</span><span class="sxs-lookup"><span data-stu-id="2fbab-144">[Options for protecting your devices and app data](../admin/devices/choose-device-security.md) (article)</span></span>
