---
title: Feilsøke AutoPilot-enheter
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
description: Lær hvordan du feilsøker AutoPilot filfeil.
ms.openlocfilehash: 9d4a47f78c38d8c076f5b3876a36b6bf46eaaaf3
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32279842"
---
# <a name="troubleshoot-autopilot-device-errors"></a><span data-ttu-id="9886a-103">Feilsøke AutoPilot-enheter</span><span class="sxs-lookup"><span data-stu-id="9886a-103">Troubleshoot AutoPilot device errors</span></span>

## <a name="device-file-error-messages"></a><span data-ttu-id="9886a-104">Feilmeldinger-filen for enheten</span><span class="sxs-lookup"><span data-stu-id="9886a-104">Device file error messages</span></span>

<span data-ttu-id="9886a-105">Her er informasjon om noen av feilene som du kan se mens du arbeider med filer i AutoPilot-enhet i Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="9886a-105">Here's info on some of the errors you might see while working with AutoPilot device files in Microsoft 365 Business.</span></span> 
  
|<span data-ttu-id="9886a-106">**Feilkode**</span><span class="sxs-lookup"><span data-stu-id="9886a-106">**Error code**</span></span>|<span data-ttu-id="9886a-107">**Løsning å prøve**</span><span class="sxs-lookup"><span data-stu-id="9886a-107">**Fix to try**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9886a-108">Ugyldig forespørselens brødtekst</span><span class="sxs-lookup"><span data-stu-id="9886a-108">Invalid request body</span></span>  <br/> |<span data-ttu-id="9886a-109">Denne feilen skjer sjelden, hvis du ser denne feilen, kan du prøve operasjonen på nytt.</span><span class="sxs-lookup"><span data-stu-id="9886a-109">This error should happen rarely, if you see this error, try the operation again.</span></span>  <br/> |
|<span data-ttu-id="9886a-110">Maskinvarenummer for en enhet er ikke riktig.</span><span class="sxs-lookup"><span data-stu-id="9886a-110">Hardware hash value for a device isn't correct.</span></span>  <br/> |<span data-ttu-id="9886a-111">Hvis du ser denne feilen, betyr det at verdien du har angitt i CSV-filen for maskinvarenummeret for én enhet er ikke riktig.</span><span class="sxs-lookup"><span data-stu-id="9886a-111">If you see this error, it means that the value you provided in your CSV file for the hardware hash of one device isn't correct.</span></span> <span data-ttu-id="9886a-112">Først bekrefter du at verdien er riktig skrevet.</span><span class="sxs-lookup"><span data-stu-id="9886a-112">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="9886a-113">Hvis du tror at verdien er riktig, men denne feilen skjer fortsatt, spør din maskinvareleverandør for hjelp.</span><span class="sxs-lookup"><span data-stu-id="9886a-113">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="9886a-114">Enheten som er tilordnet til en annen leier</span><span class="sxs-lookup"><span data-stu-id="9886a-114">Device assigned to another tenant</span></span>  <br/> |<span data-ttu-id="9886a-115">Hvis du ser denne feilen, betyr det at verdien du har angitt i CSV-filen for serienummeret eller en produktnøkkel for én eller flere enheter ikke er riktig.</span><span class="sxs-lookup"><span data-stu-id="9886a-115">If you see this error, it means that the value you provided in your CSV file for either the serial number or the product key of one or more devices isn't correct.</span></span> <span data-ttu-id="9886a-116">Først bekrefter du at verdien er riktig skrevet.</span><span class="sxs-lookup"><span data-stu-id="9886a-116">First, verify that the value was typed correctly.</span></span> <span data-ttu-id="9886a-117">Hvis du tror at verdien er riktig, men denne feilen skjer fortsatt, spør din maskinvareleverandør for hjelp.</span><span class="sxs-lookup"><span data-stu-id="9886a-117">If you think that the value is correct, but this error is still happening, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="9886a-118">CSV-filen inneholder en ugyldig serienummer eller produktnøkkelen</span><span class="sxs-lookup"><span data-stu-id="9886a-118">The CSV file contains an invalid serial number or product key</span></span>  <br/> |<span data-ttu-id="9886a-119">Hvis du ser denne feilen betyr det at du er under forsøk på å registrere enheten allerede er registrert av en annen organisasjon.</span><span class="sxs-lookup"><span data-stu-id="9886a-119">If you see this error it means that the device you are tyring to register is already registered by an other organization.</span></span> <span data-ttu-id="9886a-120">Hvis du vil løse dette problemet ved å be maskinvareleverandøren for å få hjelp.</span><span class="sxs-lookup"><span data-stu-id="9886a-120">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
|<span data-ttu-id="9886a-121">Denne enheten støttes ikke for installasjon ved hjelp av AutoPilot</span><span class="sxs-lookup"><span data-stu-id="9886a-121">This device is not supported for setup by using AutoPilot</span></span>  <br/> | <span data-ttu-id="9886a-122">Denne feilen betyr at enheten ikke oppfyller kravene for AutoPilot-distribusjon.</span><span class="sxs-lookup"><span data-stu-id="9886a-122">This error means the device does not meet AutoPilot deployment requirements.</span></span> <span data-ttu-id="9886a-123">Enheter må oppfylle disse kravene:</span><span class="sxs-lookup"><span data-stu-id="9886a-123">Devices need to meet these requirements:</span></span>  <br/>  <span data-ttu-id="9886a-124">Windows 10 versjon 1703 eller senere.</span><span class="sxs-lookup"><span data-stu-id="9886a-124">Windows 10, version 1703 or later.</span></span>  <br/>  <span data-ttu-id="9886a-125">Nye enheter som ikke har vært gjennom Windows out-of-box experience.</span><span class="sxs-lookup"><span data-stu-id="9886a-125">New devices that have not been through Windows out-of-box experience.</span></span>  <br/> |
|<span data-ttu-id="9886a-126">Finner ikke enhet</span><span class="sxs-lookup"><span data-stu-id="9886a-126">Device not found</span></span>  <br/> |<span data-ttu-id="9886a-127">Denne feilen betyr at en eller flere enheter i CSV-filen ikke er registrert for organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="9886a-127">This error means that one or more devices in your CSV file is not registered to your organization.</span></span> <span data-ttu-id="9886a-128">Hvis du vil løse dette problemet ved å be maskinvareleverandøren for å få hjelp.</span><span class="sxs-lookup"><span data-stu-id="9886a-128">To fix this, ask your hardware vendor for help.</span></span>  <br/> |
   
