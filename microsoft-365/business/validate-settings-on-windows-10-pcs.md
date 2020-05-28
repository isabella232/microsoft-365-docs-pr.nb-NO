---
title: Validere innstillingene for appbeskyttelse på Windows 10-datamaskiner
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Finn ut hvordan du kontrollerer at innstillingene for beskyttelse av Microsoft 365 for business app trådte i kraft på brukernes Windows 10-enheter.
ms.openlocfilehash: 39aee3bc811cb0090d58f9a282de7a8162c097b3
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/27/2020
ms.locfileid: "44403594"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="e8c5a-103">Validere innstillinger for enhetsbeskyttelse på Windows 10-PCer</span><span class="sxs-lookup"><span data-stu-id="e8c5a-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="e8c5a-104">Kontroller at enhetspolicyer for Windows 10 er angitt</span><span class="sxs-lookup"><span data-stu-id="e8c5a-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="e8c5a-105">Når du [har konfigurert policyer](protection-settings-for-windows-10-pcs.md)for enheter , kan det ta opptil noen timer før retningslinjene trer i kraft på brukernes enheter.</span><span class="sxs-lookup"><span data-stu-id="e8c5a-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="e8c5a-106">Du kan bekrefte at policyene trådte i kraft ved å se på ulike Windows-innstillinger-skjermbilder på brukernes enheter.</span><span class="sxs-lookup"><span data-stu-id="e8c5a-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="e8c5a-107">Fordi brukerne ikke kan endre innstillingene for Windows Update og Windows Defender Antivirus på Windows 10-enhetene sine, blir mange alternativer nedtonet.</span><span class="sxs-lookup"><span data-stu-id="e8c5a-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="e8c5a-108">Gå til **Alternativer for omstart** av innstillinger \> **oppdatering &amp; av** \> **Windows Update** \> **pånytt,** og bekreft at alle innstillingene er nedtonet.</span><span class="sxs-lookup"><span data-stu-id="e8c5a-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Alle omstart-alternativene er nedtonet.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="e8c5a-110">Gå til **Innstillinger** \> **Update &amp; sikkerhet** \> **Windows Update** Avanserte \> **alternativer** og bekreft at alle innstillingene er nedtonet.</span><span class="sxs-lookup"><span data-stu-id="e8c5a-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Alternativer for Avanserte oppdateringer i Windows er alle nedtonet.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="e8c5a-112">Gå til **Innstillinger** \> **Oppdatering &amp; sikkerhet** \> **Windows Update** Avanserte \> **alternativer** Velg hvordan \> **oppdateringer leveres**.</span><span class="sxs-lookup"><span data-stu-id="e8c5a-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="e8c5a-113">Bekreft at du kan se meldingen (i rødt) at noen innstillinger er skjult eller administrert av organisasjonen, og at alle alternativene er nedtonet.</span><span class="sxs-lookup"><span data-stu-id="e8c5a-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Velg hvordan oppdateringer skal leveres siden angir at innstillingene er skjult eller administrert av organisasjonen.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="e8c5a-115">Hvis du vil åpne Sikkerhetssenter for Windows Defender, går du til **Innstillinger** \> \*\* &amp; Oppdateringssikkerhet\*\* \> **Windows Defender** klikk Åpne Windows Defender Security \> **Center** \> **Virus &amp; trådbeskyttelse** \> **Virus &amp; trusselbeskyttelse**.</span><span class="sxs-lookup"><span data-stu-id="e8c5a-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="e8c5a-116">Kontroller at alle alternativene er nedtonet.</span><span class="sxs-lookup"><span data-stu-id="e8c5a-116">Verify that all options are grayed out.</span></span> 
    
    ![Innstillingene for virus- og trusselbeskyttelse er nedtonet.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="e8c5a-118">Beslektede emner</span><span class="sxs-lookup"><span data-stu-id="e8c5a-118">Related Topics</span></span>

[<span data-ttu-id="e8c5a-119">Microsoft 365 for forretningsdokumentasjon og ressurser</span><span class="sxs-lookup"><span data-stu-id="e8c5a-119">Microsoft 365 for business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="e8c5a-120">Komme i gang med Microsoft 365 for bedrifter</span><span class="sxs-lookup"><span data-stu-id="e8c5a-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="e8c5a-121">Administrere Microsoft 365 for bedrifter</span><span class="sxs-lookup"><span data-stu-id="e8c5a-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="e8c5a-122">Angi enhetskonfigurasjoner for PC-er med Windows 10</span><span class="sxs-lookup"><span data-stu-id="e8c5a-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

