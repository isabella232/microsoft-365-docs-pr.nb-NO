---
title: Feilsøke AutoPilot-enheter
f1.keywords:
- NOCSH
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
description: Finn ut hvordan du feilsøker Feil på AutoPilot-enheten.
ms.openlocfilehash: 8390f695a3e11386ae2617da4061bed1d8214375
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594212"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="1c4d1-103">Feilsøke AutoPilot-enheter</span><span class="sxs-lookup"><span data-stu-id="1c4d1-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="1c4d1-104">Feilmeldinger i enhetsfil</span><span class="sxs-lookup"><span data-stu-id="1c4d1-104">Device file error messages</span></span>

<span data-ttu-id="1c4d1-105">Her er informasjon om noen av feilene du kan se mens du arbeider med AutoPilot enhetsfiler i Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="1c4d1-106">**Feilkode**</span><span class="sxs-lookup"><span data-stu-id="1c4d1-106">**Error code**</span></span>|<span data-ttu-id="1c4d1-107">**Fiks for å prøve**</span><span class="sxs-lookup"><span data-stu-id="1c4d1-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1c4d1-108">Ugyldig forespørselsorgan</span><span class="sxs-lookup"><span data-stu-id="1c4d1-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="1c4d1-109">Denne feilen bør skje sjelden, hvis du ser denne feilen, kan du prøve operasjonen på nytt.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="1c4d1-110">Maskinvarehash-verdien for en enhet er ikke riktig.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="1c4d1-111">Hvis du ser denne feilen, betyr det at verdien du oppga i CSV-filen for maskinvarehashen på én enhet, ikke er riktig.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="1c4d1-112">Kontroller først at verdien ble skrevet inn riktig.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="1c4d1-113">Hvis du tror at verdien er riktig, men denne feilen fortsatt skjer, kan du be maskinvareleverandøren om hjelp.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="1c4d1-114">Enhet tilordnet til en annen leier</span><span class="sxs-lookup"><span data-stu-id="1c4d1-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="1c4d1-115">Hvis du ser denne feilen, betyr det at verdien du oppga i CSV-filen for serienummeret eller produktnøkkelen til én eller flere enheter, ikke er riktig.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="1c4d1-116">Kontroller først at verdien ble skrevet inn riktig.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="1c4d1-117">Hvis du tror at verdien er riktig, men denne feilen fortsatt skjer, kan du be maskinvareleverandøren om hjelp.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="1c4d1-118">CSV-filen inneholder et ugyldig serienummer eller produktnøkkel</span><span class="sxs-lookup"><span data-stu-id="1c4d1-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="1c4d1-119">Hvis du ser denne feilen, betyr det at enheten du prøver å registrere, allerede er registrert av en annen organisasjon.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-119">If you see this error, it means that the device you are trying to register is already registered by another organization.</span></span> <span data-ttu-id="1c4d1-120">Hvis du vil løse denne feilen, kan du be maskinvareleverandøren om hjelp.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-120">To fix this error, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="1c4d1-121">Denne enheten støttes ikke for oppsett ved hjelp av AutoPilot</span><span class="sxs-lookup"><span data-stu-id="1c4d1-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="1c4d1-122">Denne feilen betyr at enheten ikke oppfyller autopilotdistribusjonskravene.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-122">This error means the device doesn't meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="1c4d1-123">Enheter må oppfylle disse kravene:</span><span class="sxs-lookup"><span data-stu-id="1c4d1-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="1c4d1-124">Windows 10 versjon 1703 eller senere.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="1c4d1-125">Nye enheter som ikke har vært gjennom Windows-opplevelsen.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-125">New devices that haven't been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="1c4d1-126">Finner ikke enheten</span><span class="sxs-lookup"><span data-stu-id="1c4d1-126">Device not found</span></span>  <br/> |<span data-ttu-id="1c4d1-127">Denne feilen betyr at én eller flere enheter i CSV-filen ikke er registrert i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-127">This error means that one or more devices in your CSV file isn't registered to your organization.</span></span> <span data-ttu-id="1c4d1-128">Hvis du vil løse dette, kan du be maskinvareleverandøren om hjelp.</span><span class="sxs-lookup"><span data-stu-id="1c4d1-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
