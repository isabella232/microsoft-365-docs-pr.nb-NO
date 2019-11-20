---
title: Feilsøke AutoPilot-enheter
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: troubleshooting
f1_keywords:
- ZTDTroubleshootDeviceErrors
- O365E_ZTDTroubleshootDeviceErrors
- BCS365_ZTDTroubleshootDeviceErrors
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 1f468690-530c-47ea-918f-fede24607c53
description: Finn ut hvordan du feilsøker feil i AutoPilot-enheten.
ms.openlocfilehash: 1b5358bd6686c2548e82ec5297ac0ad675835718
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718703"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="7bf78-103">Feilsøke AutoPilot-enheter</span><span class="sxs-lookup"><span data-stu-id="7bf78-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="7bf78-104">Feilmeldinger for enhetsfiler</span><span class="sxs-lookup"><span data-stu-id="7bf78-104">Device file error messages</span></span>

<span data-ttu-id="7bf78-105">Her er informasjon om noen av feilene du kan se mens du arbeider med AutoPilot enhetsfiler i Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="7bf78-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="7bf78-106">**Feilkode**</span><span class="sxs-lookup"><span data-stu-id="7bf78-106">**Error code**</span></span>|<span data-ttu-id="7bf78-107">**Fix å prøve**</span><span class="sxs-lookup"><span data-stu-id="7bf78-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7bf78-108">Ugyldig forespørsels tekst</span><span class="sxs-lookup"><span data-stu-id="7bf78-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="7bf78-109">Denne feilen oppstår sjelden, hvis du ser denne feilen, kan du prøve operasjonen på nytt.</span><span class="sxs-lookup"><span data-stu-id="7bf78-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="7bf78-110">Maskinvarenummer verdi for en enhet er ikke riktig.</span><span class="sxs-lookup"><span data-stu-id="7bf78-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="7bf78-111">Hvis du ser denne feilen, betyr det at verdien du angav i CSV-filen for maskinvarenummeret til én enhet, ikke er riktig.</span><span class="sxs-lookup"><span data-stu-id="7bf78-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="7bf78-112">Først må du kontrollere at verdien ble skrevet inn riktig.</span><span class="sxs-lookup"><span data-stu-id="7bf78-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="7bf78-113">Hvis du tror at verdien er riktig, men denne feilen fortsatt skjer, kan du be maskinvareleverandøren om hjelp.</span><span class="sxs-lookup"><span data-stu-id="7bf78-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="7bf78-114">Enhet som er tilordnet en annen Tenant</span><span class="sxs-lookup"><span data-stu-id="7bf78-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="7bf78-115">Hvis du ser denne feilen, betyr det at verdien du angav i CSV-filen for enten serienummeret eller produktnøkkelen til én eller flere enheter, ikke er riktig.</span><span class="sxs-lookup"><span data-stu-id="7bf78-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="7bf78-116">Først må du kontrollere at verdien ble skrevet inn riktig.</span><span class="sxs-lookup"><span data-stu-id="7bf78-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="7bf78-117">Hvis du tror at verdien er riktig, men denne feilen fortsatt skjer, kan du be maskinvareleverandøren om hjelp.</span><span class="sxs-lookup"><span data-stu-id="7bf78-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="7bf78-118">CSV-filen inneholder et ugyldig serienummer eller en produktnøkkel</span><span class="sxs-lookup"><span data-stu-id="7bf78-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="7bf78-119">Hvis du ser denne feilen, betyr det at enheten du prøver å registrere, allerede er registrert av en annen organisasjon.</span><span class="sxs-lookup"><span data-stu-id="7bf78-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="7bf78-120">Spør maskinvareleverandøren om hjelp for å rette opp denne feilen.</span><span class="sxs-lookup"><span data-stu-id="7bf78-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="7bf78-121">Denne enheten støttes ikke for installasjon ved hjelp av AutoPilot</span><span class="sxs-lookup"><span data-stu-id="7bf78-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="7bf78-122">Denne feilen betyr at enheten ikke oppfyller kravene til distribusjon av AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="7bf78-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="7bf78-123">Enheter må oppfylle disse kravene:</span><span class="sxs-lookup"><span data-stu-id="7bf78-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="7bf78-124">Windows 10 versjon 1703 eller senere.</span><span class="sxs-lookup"><span data-stu-id="7bf78-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="7bf78-125">Ny anordninger det har ikke ' blitt igjennom Vinduer ut-av-bokse med erfaring.</span><span class="sxs-lookup"><span data-stu-id="7bf78-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="7bf78-126">Finner ikke enheten</span><span class="sxs-lookup"><span data-stu-id="7bf78-126">Device not found</span></span>  <br/> |<span data-ttu-id="7bf78-127">Denne feilen betyr at én eller flere enheter i CSV-filen ikke er registrert i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="7bf78-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="7bf78-128">Du kan løse dette problemet ved å be maskinvareleverandøren om hjelp.</span><span class="sxs-lookup"><span data-stu-id="7bf78-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
