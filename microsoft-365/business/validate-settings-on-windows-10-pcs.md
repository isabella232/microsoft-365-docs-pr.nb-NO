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
description: Lær hvordan du kontrollerer at beskyttelsesinnstillingene for Microsoft 365 for business-apper trer i kraft på brukernes Windows 10-enheter.
ms.openlocfilehash: ff99b3a4fce49aebdb5c72f51e46678a7821e186
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912418"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="61681-103">Validere innstillinger for enhetsbeskyttelse på Windows 10-PC-er</span><span class="sxs-lookup"><span data-stu-id="61681-103">Validate device protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-windows-10-device-policies-are-set"></a><span data-ttu-id="61681-104">Kontroller at windows 10-enhetspolicyer er angitt</span><span class="sxs-lookup"><span data-stu-id="61681-104">Verify that Windows 10 device policies are set</span></span>

<span data-ttu-id="61681-105">Når du [har konfigurert policyer](protection-settings-for-windows-10-pcs.md)for enheter, kan det ta opptil et par timer før policyen trer i kraft på brukernes enheter.</span><span class="sxs-lookup"><span data-stu-id="61681-105">After you [set up devices policies](protection-settings-for-windows-10-pcs.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="61681-106">Du kan bekrefte at policyene trer i kraft ved å se på ulike Skjermbilder for Windows-innstillinger på brukernes enheter.</span><span class="sxs-lookup"><span data-stu-id="61681-106">You can confirm that the policies took effect by looking at various Windows Settings screens on the users' devices.</span></span> <span data-ttu-id="61681-107">Fordi brukerne ikke kan endre Windows Update- og Windows Defender Antivirus-innstillingene på Windows 10-enhetene sine, vil mange alternativer være nedtonet.</span><span class="sxs-lookup"><span data-stu-id="61681-107">Because the users won't be able to modify the Windows Update and Windows Defender Antivirus settings on their Windows 10 devices, many options will be grayed out.</span></span>
  
1. <span data-ttu-id="61681-108">Gå til **Innstillinger** \> **Oppdater &amp; sikkerhetsalternativer** \> **for Windows Update Start** på \> **nytt,** og bekreft at alle innstillingene er nedtonet.</span><span class="sxs-lookup"><span data-stu-id="61681-108">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Restart options** and confirm that all settings are grayed out.</span></span> 
    
    ![Alle alternativene for Omstart er nedtonet.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. <span data-ttu-id="61681-110">Gå til **Innstillinger Oppdater** \> **sikkerhet &amp; Windows** \> **Update** \> **Avanserte alternativer** og bekreft at alle innstillingene er nedtonet.</span><span class="sxs-lookup"><span data-stu-id="61681-110">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** and confirm that all settings are grayed out.</span></span> 
    
    ![Alternativer for avanserte oppdateringer i Windows er nedtonet.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. <span data-ttu-id="61681-112">Gå til **Innstillinger Oppdater** \> **sikkerhet &amp; Windows** \> **Update** \> **Avanserte alternativer** \> **Velg hvordan oppdateringer skal leveres**.</span><span class="sxs-lookup"><span data-stu-id="61681-112">Go to **Settings** \> **Update &amp; security** \> **Windows Update** \> **Advanced options** \> **Choose how updates are delivered**.</span></span>
    
    <span data-ttu-id="61681-113">Bekreft at du kan se meldingen (i rødt) om at noen innstillinger er skjult eller administrert av organisasjonen, og at alle alternativene er nedtonet.</span><span class="sxs-lookup"><span data-stu-id="61681-113">Confirm that you can see the message (in red) that some settings are hidden or managed by your organization, and all the options are grayed out.</span></span>
    
    ![Velg hvordan oppdateringer leveres-siden angir at innstillingene er skjult eller administrert av organisasjonen.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. <span data-ttu-id="61681-115">Hvis du vil åpne Windows Defender Sikkerhetssenter, går du til Innstillinger  Oppdater sikkerhet Windows Defender og klikker Åpne Windows \> **&amp;** \>  \> **Defender Security Center** Virus thread \> **&amp; protection** Virus threat protection \> **&amp; settings**.</span><span class="sxs-lookup"><span data-stu-id="61681-115">To open the Windows Defender Security Center, go to **Settings** \> **Update &amp; security** \> **Windows Defender** \> click **Open Windows Defender Security Center** \> **Virus &amp; thread protection** \> **Virus &amp; threat protection settings**.</span></span> 
    
5. <span data-ttu-id="61681-116">Kontroller at alle alternativene er nedtonet.</span><span class="sxs-lookup"><span data-stu-id="61681-116">Verify that all options are grayed out.</span></span> 
    
    ![Innstillingene for virus- og trusselbeskyttelse er nedtonet.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a><span data-ttu-id="61681-118">Beslektede emner</span><span class="sxs-lookup"><span data-stu-id="61681-118">Related Topics</span></span>

[<span data-ttu-id="61681-119">Dokumentasjon og ressurser for Microsoft 365 for bedrifter</span><span class="sxs-lookup"><span data-stu-id="61681-119">Microsoft 365 for business documentation and resources</span></span>](./index.yml)
  
[<span data-ttu-id="61681-120">Komme i gang med Microsoft 365 for bedrifter</span><span class="sxs-lookup"><span data-stu-id="61681-120">Get started with Microsoft 365 for business</span></span>](microsoft-365-business-overview.md)
  
[<span data-ttu-id="61681-121">Administrere Microsoft 365 for bedrifter</span><span class="sxs-lookup"><span data-stu-id="61681-121">Manage Microsoft 365 for business</span></span>](manage.md)
  
[<span data-ttu-id="61681-122">Angi enhetskonfigurasjoner for PC-er med Windows 10</span><span class="sxs-lookup"><span data-stu-id="61681-122">Set device configurations for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
