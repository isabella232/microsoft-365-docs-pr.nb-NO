---
title: Validere innstillingene for appbeskyttelse på Windows 10-datamaskiner
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Lær hvordan du validerer innstillinger for Microsoft 365 for Business-app i Windows 10-enheter.
ms.openlocfilehash: c54b053c1f6efbca8fd02431c416793a044c6821
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721864"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="07a6a-103">Validere innstillingene for appbeskyttelse på Windows 10-datamaskiner</span><span class="sxs-lookup"><span data-stu-id="07a6a-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="07a6a-104">Kontroller at brukere ikke kan kopiere firmadata til personlige filer på bedriftens enheter</span><span class="sxs-lookup"><span data-stu-id="07a6a-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="07a6a-105">Etter at du [har konfigurert policyer for appbeskyttelse](protection-settings-for-windows-10-devices.md), kan det ta opptil noen timer før policyen trer i kraft på brukernes enheter.</span><span class="sxs-lookup"><span data-stu-id="07a6a-105">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices.</span></span> <span data-ttu-id="07a6a-106">Hvis **du aktiverte** **hindre brukere fra å kopiere firmadata til personlige filer og tvinge dem til å lagre arbeidsfiler i OneDrive for Business** -innstillingen for firmaets eide enheter kan du sjekke dette på brukerens enhet etter at de har koblet til Azure-annonse og logget på.</span><span class="sxs-lookup"><span data-stu-id="07a6a-106">If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they've connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="07a6a-107">**Bekrefte tilkoblingsinnstillinger**</span><span class="sxs-lookup"><span data-stu-id="07a6a-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="07a6a-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span><span class="sxs-lookup"><span data-stu-id="07a6a-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="07a6a-111">På siden **administrert av** \<leier navn\> kan du se **tilkoblingsinformasjonen** som inneholder en **Management Server-adresse** som den som vises i følgende figur.</span><span class="sxs-lookup"><span data-stu-id="07a6a-111">On the **Managed by** \<tenant name\> page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="07a6a-113">**Kontroller at du ikke kan lime inn firmadata i en app som ikke administreres**</span><span class="sxs-lookup"><span data-stu-id="07a6a-113">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="07a6a-114">Åpne Outlook 2016 som ble installert av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="07a6a-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="07a6a-115">Åpne en e-postmelding og kopier noe av innholdet fra den.</span><span class="sxs-lookup"><span data-stu-id="07a6a-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="07a6a-116">Åpne Notisblokk, og prøv å lime inn innholdet.</span><span class="sxs-lookup"><span data-stu-id="07a6a-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="07a6a-117">Du vil motta en feilmelding som sier at appen ikke får tilgang til innhold.</span><span class="sxs-lookup"><span data-stu-id="07a6a-117">You'll receive an error that states the app can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="07a6a-119">Du kan imidlertid lime inn det samme innholdet i Word 2016.</span><span class="sxs-lookup"><span data-stu-id="07a6a-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="07a6a-120">Kontroller at brukere ikke kan kopiere firmadata til personlige filer på personlige enheter</span><span class="sxs-lookup"><span data-stu-id="07a6a-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="07a6a-121">**Kontrollere tilkoblingsinnstillinger**</span><span class="sxs-lookup"><span data-stu-id="07a6a-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="07a6a-122">På Windows 10 personlig enhet der du er logget på som en lokal bruker, gå til **Windows-innstillinger**, og klikk eller trykk på **kontoer** \> **tilgang arbeid eller skole**.</span><span class="sxs-lookup"><span data-stu-id="07a6a-122">On your Windows 10 personal device where you're logged in as a local user, go to **Windows Settings**, and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="07a6a-123">Velg **Koble til** under **Få tilgang til jobb eller skole**.</span><span class="sxs-lookup"><span data-stu-id="07a6a-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="07a6a-124">Skriv inn Microsoft 365 Business legitimasjonen i dialogboksen **Konfigurer en jobb- eller skolekonto** \> **Logg på**.</span><span class="sxs-lookup"><span data-stu-id="07a6a-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="07a6a-125">Velg **Få tilgang til jobb- eller skolekonto** på siden **Få tilgang til arbeidsplassen eller skolen**, og velg deretter **Informasjon**.</span><span class="sxs-lookup"><span data-stu-id="07a6a-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Klikk eller trykk på informasjon i dialogboksen arbeid eller skole konto.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="07a6a-127">På siden for **tilgang til arbeid eller skole** kan du se **tilkoblingsinformasjonen** som inneholder en **Management Server-adresse** som den som vises i illustrasjonen nedenfor, og inkluderer ordene *via* og *Mam* innenfor.</span><span class="sxs-lookup"><span data-stu-id="07a6a-127">On the **Access work or school** page, you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="07a6a-129">**Kontroller at du ikke kan lime inn firmadata i en app som ikke administreres**</span><span class="sxs-lookup"><span data-stu-id="07a6a-129">**Verify that you cannot paste company data in a non-managed app**</span></span>
  
1. <span data-ttu-id="07a6a-130">Åpne Outlook 2016 og legg til Microsoft 365 Business-kontoen hvis nødvendig, og logg på med Microsoft 365 Business-legitimasjonen.</span><span class="sxs-lookup"><span data-stu-id="07a6a-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="07a6a-131">Åpne en e-postmelding og kopier noe av innholdet fra den.</span><span class="sxs-lookup"><span data-stu-id="07a6a-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="07a6a-132">Åpne Notisblokk, og prøv å lime inn innholdet.</span><span class="sxs-lookup"><span data-stu-id="07a6a-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="07a6a-133">Du vil motta en feilmelding som sier at appen ikke får tilgang til innhold.</span><span class="sxs-lookup"><span data-stu-id="07a6a-133">You'll receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="07a6a-135">Du kan imidlertid lime inn det samme innholdet i Word 2016.</span><span class="sxs-lookup"><span data-stu-id="07a6a-135">You can, however, paste the same content into Word 2016.</span></span>
    

