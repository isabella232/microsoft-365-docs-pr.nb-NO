---
title: Validere innstillingene for appbeskyttelse på Windows 10-datamaskiner
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Lær hvordan du validerer Microsoft 365 Business app innstillinger i Windows 10 enheter.
ms.openlocfilehash: 5ab91d65fa7bd40ebc118df217c9711b7bbfe7a4
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32286758"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="e4d01-103">Valider beskyttelse enhetsinnstillinger i Windows PC-10</span><span class="sxs-lookup"><span data-stu-id="e4d01-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="e4d01-104">Kontroller at retningslinjer for Windows 10-enheten er satt</span><span class="sxs-lookup"><span data-stu-id="e4d01-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="e4d01-105">Når du [definerer policyer for enheter](protection-settings-for-windows-10-pcs.md), kan det ta et par timer for policyen trer i kraft på brukernes enheter.</span><span class="sxs-lookup"><span data-stu-id="e4d01-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="e4d01-106">Du kan bekrefte at policyene tok effekt ved å se på ulike innstillinger for Windows-skjermer på brukernes enheter.</span><span class="sxs-lookup"><span data-stu-id="e4d01-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="e4d01-107">Fordi brukere vil ikke kunne endre innstillingene for Windows Update og Windows Defender Antivirus på Windows 10 enheter, mange av disse alternativene valgbar.</span><span class="sxs-lookup"><span data-stu-id="e4d01-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, a lot of those options will be greyed out.</span></span>
  
1. <span data-ttu-id="e4d01-108">Gå til **Innstillinger for** \> **oppdatering &amp; sikkerhet** \> **Windows Update** \> **Alternativer for omstart** , og Bekreft at alle innstillingene er grået ut.</span><span class="sxs-lookup"><span data-stu-id="e4d01-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are greyed out.</span></span> 
    
    ![Alle alternativer for omstart er grået ut.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="e4d01-110">Gå til **Innstillinger for** \> **oppdatering &amp; sikkerhet** \> **Windows Update** \> **Avanserte alternativer** , og Bekreft at alle innstillingene er grået ut.</span><span class="sxs-lookup"><span data-stu-id="e4d01-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are greyed out.</span></span> 
    
    ![Windows avanserte alternativer for oppdateringer er grået ut.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="e4d01-112">Gå til **Innstillinger for** \> **oppdatering &amp; sikkerhet** \> **Windows Update** \> **Avanserte alternativer** \> **Velg hvordan oppdateringer leveres**.</span><span class="sxs-lookup"><span data-stu-id="e4d01-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="e4d01-113">Bekreft at du kan se meldingen (i rødt) som noen av innstillingene er skjult eller administrert av organisasjonen, og alle alternativene er grået ut.</span><span class="sxs-lookup"><span data-stu-id="e4d01-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are greyed out.</span></span>
    
    ![Velg hvordan oppdateringer leveres siden angir innstillingene er skjult eller administrert av organisasjonen.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="e4d01-115">For å åpne Sikkerhetssenter for Windows Defender, kan du gå til **Innstillinger for** \> **oppdatering &amp; sikkerhet** \> **Windows Defender** \> Klikk **Åpne Sikkerhetssenter i Windows Defender** \> **Virus &amp; tråd beskyttelse mot** \> **Virus &amp; trusselen beskyttelsesinnstillingene**.</span><span class="sxs-lookup"><span data-stu-id="e4d01-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="e4d01-116">Kontroller at alle alternativene er grået ut.</span><span class="sxs-lookup"><span data-stu-id="e4d01-116">Verify that all options are greyed out.</span></span> 
    
    ![Innstillingene for Virus og threat protection er grået ut.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="e4d01-118">Beslektede emner</span><span class="sxs-lookup"><span data-stu-id="e4d01-118">Related Topics</span></span>

[<span data-ttu-id="e4d01-119">Microsoft 365 Business dokumentasjon og ressurser</span><span class="sxs-lookup"><span data-stu-id="e4d01-119">Microsoft 365 Business documentation and resources</span></span>](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[<span data-ttu-id="e4d01-120">Komme i gang med Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="e4d01-120">Get started with Microsoft 365 Business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="e4d01-121">Administrere Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="e4d01-121">Manage Microsoft 365 Business</span></span>](manage.md)
  
[<span data-ttu-id="e4d01-122">Angi enhetskonfigurasjoner for PC-er med Windows 10</span><span class="sxs-lookup"><span data-stu-id="e4d01-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
  

