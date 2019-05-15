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
description: Lær hvordan du validerer Microsoft 365 Business app innstillinger i Windows 10 enheter.
ms.openlocfilehash: 7710accf9a3cd1db788dd5215ab6d7bbb97e48a6
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074384"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a><span data-ttu-id="5966c-103">Validere innstillingene for appbeskyttelse på Windows 10-datamaskiner</span><span class="sxs-lookup"><span data-stu-id="5966c-103">Validate app protection settings on Windows 10 PCs</span></span>

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a><span data-ttu-id="5966c-104">Kontroller at brukere ikke kan kopiere firmadata til personlige filer på bedriftens enheter</span><span class="sxs-lookup"><span data-stu-id="5966c-104">Verify that users cannot copy company data to personal files on corporate devices</span></span>

<span data-ttu-id="5966c-p101">Etter at du [har konfigurert policyer for appbeskyttelse](protection-settings-for-windows-10-devices.md), kan det ta opptil noen timer før policyen trer i kraft på brukernes enheter. Hvis du har slått **På** innstillingen **Hindre brukere i å kopiere firmadata til personlige filer, og tving dem til å lagre arbeidsfiler på OneDrive for Business** for firmaeide enheter, kan du kontrollere dette på brukernes enheter etter de har koblet til Azure AD og logget seg på.</span><span class="sxs-lookup"><span data-stu-id="5966c-p101">After you [set up app protection policies](protection-settings-for-windows-10-devices.md), it may take up to a few hours for the policy to take effect on users' devices. If you turned **On** the **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** setting for company owned devices, you can check this on the user's device after they have connected to Azure AD and signed in.</span></span> 
  
 <span data-ttu-id="5966c-107">**Bekrefte tilkoblingsinnstillinger**</span><span class="sxs-lookup"><span data-stu-id="5966c-107">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="5966c-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span><span class="sxs-lookup"><span data-stu-id="5966c-p102">After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. <span data-ttu-id="5966c-111">På **administrert av** \<leier navn\> side kan du vise **tilkoblingsinformasjon** som inkluderer en **Management serveradresse** som den som vises i følgende figur.</span><span class="sxs-lookup"><span data-stu-id="5966c-111">On the **Managed by** \<tenant name\> page you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure.</span></span> 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 <span data-ttu-id="5966c-113">**Kontroller at du ikke kan lime inn firmadata til en ikke-administrert app**</span><span class="sxs-lookup"><span data-stu-id="5966c-113">**Verify that you cannot paste company data to a non-managed app**</span></span>
  
1. <span data-ttu-id="5966c-114">Åpne Outlook 2016 som ble installert av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="5966c-114">Open Outlook 2016 that was installed by Microsoft 365 Business.</span></span>
    
2. <span data-ttu-id="5966c-115">Åpne en e-postmelding og kopier noe av innholdet fra den.</span><span class="sxs-lookup"><span data-stu-id="5966c-115">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="5966c-116">Åpne Notisblokk, og prøv å lime inn innholdet.</span><span class="sxs-lookup"><span data-stu-id="5966c-116">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="5966c-117">Du får en feilmelding som sier at appen ikke får tilgang til innholdet.</span><span class="sxs-lookup"><span data-stu-id="5966c-117">You will receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="5966c-119">Du kan imidlertid lime inn det samme innholdet i Word 2016.</span><span class="sxs-lookup"><span data-stu-id="5966c-119">You can, however, paste the same content into Word 2016.</span></span>
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a><span data-ttu-id="5966c-120">Kontroller at brukere ikke kan kopiere firmadata til personlige filer på personlige enheter</span><span class="sxs-lookup"><span data-stu-id="5966c-120">Verify that users cannot copy company data to personal files on personal devices</span></span>

 <span data-ttu-id="5966c-121">**Kontrollere tilkoblingsinnstillinger**</span><span class="sxs-lookup"><span data-stu-id="5966c-121">**Verify connection settings**</span></span>
  
1. <span data-ttu-id="5966c-122">Gå til **Windows-innstillinger**, og klikk eller trykk på **Kontoer** \> **Få tilgang til jobb eller skole** på den personlige Windows 10-enheten, hvor du er logget på som lokal bruker.</span><span class="sxs-lookup"><span data-stu-id="5966c-122">On your Windows 10 personal device where you are logged in as a local user, go to **Windows Settings** and click or tap **Accounts** \> **Access work or school**.</span></span>
    
2. <span data-ttu-id="5966c-123">Velg **Koble til** under **Få tilgang til jobb eller skole**.</span><span class="sxs-lookup"><span data-stu-id="5966c-123">Under the **Access work or school**, choose **Connect**.</span></span>
    
3. <span data-ttu-id="5966c-124">Skriv inn Microsoft 365 Business legitimasjonen i dialogboksen **Konfigurer en jobb- eller skolekonto** \> **Logg på**.</span><span class="sxs-lookup"><span data-stu-id="5966c-124">Enter your Microsoft 365 Business credential into the **Set up a work or school account dialog** \> **Sign in**.</span></span>
    
4. <span data-ttu-id="5966c-125">Velg **Få tilgang til jobb- eller skolekonto** på siden **Få tilgang til arbeidsplassen eller skolen**, og velg deretter **Informasjon**.</span><span class="sxs-lookup"><span data-stu-id="5966c-125">On the **Access work or school** page, choose the **Work or school account**, and then choose **Info**.</span></span>
    
    ![Click or tap Info on the Work or school account dalog.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. <span data-ttu-id="5966c-127">Se **Tilkoblingsinformasjon** på siden **Få tilgang jobb eller skole** som inneholder en **Adresse for administrasjonsserver** som er illustrert i følgende figur. Denne inkluderer ordene  *wip*  og  *mam*  .</span><span class="sxs-lookup"><span data-stu-id="5966c-127">On the **Access work or school** page you can see the **Connection info** that includes a **Management Server Address** like the one shown in the following figure, and includes the words  *wip*  and  *mam*  within.</span></span> 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 <span data-ttu-id="5966c-129">**Kontroller at du ikke kan lime inn firmadata til en ikke-administrert app**</span><span class="sxs-lookup"><span data-stu-id="5966c-129">**Verify that you cannot paste company data to a non-managed app**</span></span>
  
1. <span data-ttu-id="5966c-130">Åpne Outlook 2016 og legg til Microsoft 365 Business-kontoen hvis nødvendig, og logg på med Microsoft 365 Business-legitimasjonen.</span><span class="sxs-lookup"><span data-stu-id="5966c-130">Open Outlook 2016 and add your Microsoft 365 Business account if necessary and sign in with your Microsoft 365 Business credentials.</span></span>
    
2. <span data-ttu-id="5966c-131">Åpne en e-postmelding og kopier noe av innholdet fra den.</span><span class="sxs-lookup"><span data-stu-id="5966c-131">Open an email and copy some content from it.</span></span>
    
    <span data-ttu-id="5966c-132">Åpne Notisblokk, og prøv å lime inn innholdet.</span><span class="sxs-lookup"><span data-stu-id="5966c-132">Open Notepad and attempt to paste the content in.</span></span>
    
    <span data-ttu-id="5966c-133">Du får en feilmelding som sier at appen ikke får tilgang til innholdet.</span><span class="sxs-lookup"><span data-stu-id="5966c-133">You will receive an error that states App can't access content.</span></span>
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    <span data-ttu-id="5966c-135">Du kan imidlertid lime inn det samme innholdet i Word 2016.</span><span class="sxs-lookup"><span data-stu-id="5966c-135">You can, however, paste the same content into Word 2016.</span></span>
    

