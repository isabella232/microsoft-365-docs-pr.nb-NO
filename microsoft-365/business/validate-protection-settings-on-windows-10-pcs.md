---
title: Validere innstillingene for appbeskyttelse på Windows 10-datamaskiner
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Valider innstillinger for appbeskyttelse for Microsoft 365 Business Premium på Windows 10-enheter, og kontroller at brukere ikke kan kopiere firmadata til personlige filer eller ikke-administrerte apper.
ms.openlocfilehash: e319ffa5149f055b5de45078facc8899acffc223
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579866"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="f1ae1-103">Validere innstillingene for appbeskyttelse på Windows 10-datamaskiner</span><span class="sxs-lookup"><span data-stu-id="f1ae1-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="f1ae1-104">Kontroller at brukere ikke kan kopiere firmadata til personlige filer på bedriftens enheter</span><span class="sxs-lookup"><span data-stu-id="f1ae1-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="f1ae1-105">Etter at du [har konfigurert policyer for appbeskyttelse](protection-settings-for-windows-10-devices.md), kan det ta opptil noen timer før policyen trer i kraft på brukernes enheter.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="f1ae1-106">Hvis du  har aktivert innstillingen Hindre brukere i å kopiere firmadata til personlige filer og tvinge dem til å lagre arbeidsfiler i **OneDrive for Business** for firmaeide enheter, kan du kontrollere dette på brukerens enhet etter at de har koblet til Azure AD og logget på.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="f1ae1-107">**Kontrollere tilkoblingsinnstillinger**</span><span class="sxs-lookup"><span data-stu-id="f1ae1-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="f1ae1-108">Når du har logget på med Microsoft 365 Business Premium-legitimasjon og koblet til Azure AD som beskrevet i Konfigurere [Windows-enheter for Microsoft 365 Business Premium-brukere,](set-up-windows-devices.md)går du til **Windows-innstillinger** Kontoer Tilgang til jobb \>  \> **eller skole**.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-108">After you sign in with Microsoft 365 Business Premium credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**.</span></span> <span data-ttu-id="f1ae1-109">Velg **Koblet til Azure \<tenant name\> AD**, og velg deretter **Informasjon**.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-109">Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="f1ae1-111">På **Administrert av-siden** kan du se tilkoblingsinformasjonen som inneholder en Adresse for administrasjonsserver, som den som \<tenant name\> vises i figuren nedenfor.  </span><span class="sxs-lookup"><span data-stu-id="f1ae1-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="f1ae1-113">**Kontroller at du ikke kan lime inn firmadata i en ikke-administrert app**</span><span class="sxs-lookup"><span data-stu-id="f1ae1-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="f1ae1-114">Åpne Outlook 2016 som ble installert av Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-114">Open Outlook 2016 that was installed by Microsoft 365 Business Premium.</span></span>
    
2. <span data-ttu-id="f1ae1-115">Åpne en e-postmelding og kopier noe av innholdet fra den.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="f1ae1-116">Åpne Notisblokk, og prøv å lime inn innholdet.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="f1ae1-117">Du får en feilmelding som sier at appen ikke har tilgang til innhold.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="f1ae1-119">Du kan imidlertid lime inn det samme innholdet i Word 2016.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="f1ae1-120">Kontroller at brukere ikke kan kopiere firmadata til personlige filer på personlige enheter</span><span class="sxs-lookup"><span data-stu-id="f1ae1-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="f1ae1-121">**Kontrollere tilkoblingsinnstillinger**</span><span class="sxs-lookup"><span data-stu-id="f1ae1-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="f1ae1-122">Gå til Windows-innstillinger på den personlige **Windows** 10-enheten der du er  logget på som en lokal bruker, og klikk eller trykk Kontoer Tilgang til jobb \> **eller skole.**</span><span class="sxs-lookup"><span data-stu-id="f1ae1-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="f1ae1-123">Velg **Koble til** under **Få tilgang til jobb eller skole**.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="f1ae1-124">Skriv inn Microsoft 365 Business Premium-legitimasjonen i dialogboksen Konfigurer en jobb- eller **skolekonto** \> **Logg på**.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-124">Enter your Microsoft 365 Business Premium credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="f1ae1-125">Velg **Få tilgang til jobb- eller skolekonto** på siden **Få tilgang til arbeidsplassen eller skolen**, og velg deretter **Informasjon**.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Klikk eller trykk informasjon i dialogboksen Jobb- eller skolekonto.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="f1ae1-127">Du kan se Tilkoblingsinformasjon som  inneholder en **Adresse** for administrasjonsserver, som den som vises i figuren nedenfor, på siden **Access-jobb** eller skole, og inneholder ordene *wip* og *mam* inni.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="f1ae1-129">**Kontroller at du ikke kan lime inn firmadata i en ikke-administrert app**</span><span class="sxs-lookup"><span data-stu-id="f1ae1-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="f1ae1-130">Åpne Outlook 2016, og legg til Microsoft 365 Business Premium-kontoen om nødvendig, og logg på med Microsoft 365 Business Premium-legitimasjonen.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-130">Open Outlook 2016 and add your Microsoft 365 Business Premium account if necessary and sign in with your Microsoft 365 Business Premium credentials.</span></span>
    
2. <span data-ttu-id="f1ae1-131">Åpne en e-postmelding og kopier noe av innholdet fra den.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="f1ae1-132">Åpne Notisblokk, og prøv å lime inn innholdet.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="f1ae1-133">Du får en feilmelding om at appen ikke har tilgang til innhold.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="f1ae1-135">Du kan imidlertid lime inn det samme innholdet i Word 2016.</span><span class="sxs-lookup"><span data-stu-id="f1ae1-135">You can, however, paste the same content into Word 2016.</span></span>
    

