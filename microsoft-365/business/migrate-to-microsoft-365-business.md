---
title: Oppgrader til Microsoft 365 Business fra Office 365 Business Premium
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
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Trinn som oppgraderer bedriften fra Office 365 Business Premium til Microsoft 365 Business.
ms.openlocfilehash: 95c4504d7e6e33bdededee0cfca7add0cb5f7204
ms.sourcegitcommit: 2c2248b03f7753d64490f2f7e56ec644a235b65a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/15/2019
ms.locfileid: "38640565"
---
# <a name="upgrade-to-microsoft-365-business-from-office-365-business-premium"></a><span data-ttu-id="b6db8-103">Oppgrader til Microsoft 365 Business fra Office 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="b6db8-103">Upgrade to Microsoft 365 Business from Office 365 Business Premium</span></span>

<span data-ttu-id="b6db8-104">Hvis du har en [office 365 for forretnings abonnement](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), for eksempel Office 365 Business Premium, kan du enkelt oppgradere til Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="b6db8-104">If you have an [Office 365 for business subscription](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), for example, Office 365 Business Premium, you can easily upgrade to Microsoft 365 Business.</span></span> <span data-ttu-id="b6db8-105">Oppgrader til Microsoft 365 Business hvis du vil legge til:</span><span class="sxs-lookup"><span data-stu-id="b6db8-105">Upgrade to Microsoft 365 Business if you want to add:</span></span> 
- <span data-ttu-id="b6db8-106">Windows 10 Pro (til PC-er som kjører Windows 8 eller nyere)</span><span class="sxs-lookup"><span data-stu-id="b6db8-106">Windows 10 Pro (to PCs running Windows 8 or later)</span></span>
- <span data-ttu-id="b6db8-107">Enkle kontroller som administrerer forretningsdata på enheter</span><span class="sxs-lookup"><span data-stu-id="b6db8-107">Simple controls that manage business data on devices</span></span>
- <span data-ttu-id="b6db8-108">Avanserte sikkerhetsfunksjoner.</span><span class="sxs-lookup"><span data-stu-id="b6db8-108">Advanced security capabilities.</span></span>
<span data-ttu-id="b6db8-109">Finn ut mer om Microsoft 365 Business på [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span><span class="sxs-lookup"><span data-stu-id="b6db8-109">Find out more about Microsoft 365 Business at [Microsoft.com](https://www.microsoft.com/microsoft-365/business)</span></span>

## <a name="whats-the-difference-between-office-365-business-premium-and-microsoft-365-business"></a><span data-ttu-id="b6db8-110">Hva er forskjellen mellom Office 365 Business Premium og Microsoft 365 Business?</span><span class="sxs-lookup"><span data-stu-id="b6db8-110">What's the difference between Office 365 Business Premium and Microsoft 365 Business?</span></span>
<span data-ttu-id="b6db8-111">Vi har lagt til en side-ved-side-sammenligning av disse to planene til [Microsoft 365 Business service Description](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description).</span><span class="sxs-lookup"><span data-stu-id="b6db8-111">We've added a side-by-side comparison of these two plans to the [Microsoft 365 Business Service Description](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description).</span></span> 

## <a name="before-you-get-started"></a><span data-ttu-id="b6db8-112">Før du kommer i gang</span><span class="sxs-lookup"><span data-stu-id="b6db8-112">Before you get started</span></span>

- <span data-ttu-id="b6db8-113">**Når bør jeg velge å oppgradere?**</span><span class="sxs-lookup"><span data-stu-id="b6db8-113">**When should I choose to upgrade?**</span></span> <span data-ttu-id="b6db8-114">Oppgradering er det riktige valget når du vil oppgradere **alle brukere** som er tilordnet en enkelt plan.</span><span class="sxs-lookup"><span data-stu-id="b6db8-114">Upgrade is the right choice when you want to upgrade **all users** assigned to a single plan.</span></span> <span data-ttu-id="b6db8-115">Når du velger oppgradering, blir alle plan brukerne byttet til en annen plan samtidig.</span><span class="sxs-lookup"><span data-stu-id="b6db8-115">When you choose upgrade, all plan users get switched to another plan at the same time.</span></span> <span data-ttu-id="b6db8-116">Hvis du ikke vil oppgradere alle som er tilordnet en enkelt plan, kjøper du lisenser for den nye planen (i dette tilfellet Microsoft 365 Business), og [tilordner disse lisensene individuelt](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) til hver bruker du vil oppgradere.</span><span class="sxs-lookup"><span data-stu-id="b6db8-116">If you don't want to upgrade everyone assigned to a single plan, buy licenses for the new plan (in this case Microsoft 365 Business), and [assign those licenses individually](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) to each user that you want to upgrade.</span></span> 
- <span data-ttu-id="b6db8-117">**Noen tilleggsprogrammer kan hindre oppgraderingen** Hvis du prøver å starte en oppgradering, og du har et tillegg som hindrer deg i å fortsette, kan du fjerne tillegget først og deretter legge det til på nytt senere hvis du fortsatt trenger det.</span><span class="sxs-lookup"><span data-stu-id="b6db8-117">**Some add-ons might prevent the upgrade** If you try to start an upgrade and you have an add-on that prevents you from continuing, you can remove the add-on first, and then add it back later if you still need it.</span></span> 
- <span data-ttu-id="b6db8-118">**Hvis du har forhåndsbetalt abonnementet** Det finnes ingen enkel oppgraderingsbane for forhåndsbetalte planer.</span><span class="sxs-lookup"><span data-stu-id="b6db8-118">**If you prepaid your plan** There isn't a straightforward upgrade path for prepaid plans.</span></span> <span data-ttu-id="b6db8-119">Du vet om du har en forhåndsbetalt Plan fordi du har konfigurert planen med en produkt-ID som du kanskje har kjøpt i en butikk.</span><span class="sxs-lookup"><span data-stu-id="b6db8-119">You'll know if you have a prepaid plan because you set up your plan using a product ID that you might have purchased in a store.</span></span> <span data-ttu-id="b6db8-120">Kontakt en partner, gå til Microsoft store, eller vent til den forhåndsbetalte planen utløper for å bytte til en ny plan.</span><span class="sxs-lookup"><span data-stu-id="b6db8-120">Contact a partner, go to the Microsoft Store, or wait until your prepaid plan expires to switch to a new plan.</span></span>

## <a name="upgrade-to-microsoft-365-business"></a><span data-ttu-id="b6db8-121">Oppgrader til Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="b6db8-121">Upgrade to Microsoft 365 Business</span></span>
<span data-ttu-id="b6db8-122">Kjøp lisensene ved å følge disse trinnene i det [nye administrasjonssenteret](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview):</span><span class="sxs-lookup"><span data-stu-id="b6db8-122">Buy your licenses by following these steps in the [new admin center](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview):</span></span>
1. <span data-ttu-id="b6db8-123">Logg på administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span><span class="sxs-lookup"><span data-stu-id="b6db8-123">Sign into the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>
2. <span data-ttu-id="b6db8-124">Gå til navigasjonsruten, og velg **fakturerings** \> **produkter & tjenester**.</span><span class="sxs-lookup"><span data-stu-id="b6db8-124">Go to the navigation pane and select **Billing** \> **Products & Services**.</span></span> <span data-ttu-id="b6db8-125">Finn abonnementet på Office 365, og velg det for å vise detaljene.</span><span class="sxs-lookup"><span data-stu-id="b6db8-125">Find your Office 365 subscription and select it to view the details.</span></span> 

    ![Et skjermbilde viser hvordan du finner og velger abonnementet i administrasjonssenteret.](media/FindYourSubscription.png)

3. <span data-ttu-id="b6db8-127">Velg **Oppgrader**på neste side.</span><span class="sxs-lookup"><span data-stu-id="b6db8-127">On the next page, select **Upgrade**.</span></span> 

      ![Et skjermbilde viser hvor du kan velge Oppgrader i administrasjonssenteret.](media/SelectUpgrade.png)

  > [!NOTE]
  > <span data-ttu-id="b6db8-129">Hvis du ser en melding om at **oppgradering av abonnementet ikke støttes med gruppebasert lisensiering i Azure Active Directory**, kan du trygt ignorere dette med mindre du har en veldig stor organisasjon.</span><span class="sxs-lookup"><span data-stu-id="b6db8-129">If you see a message that says **Upgrading your subscription is not supported with group-based licensing in Azure Active Directory**, you can safely ignore this unless you have a very large organization.</span></span> <span data-ttu-id="b6db8-130">Organisasjoner som har valgt dette alternativet, er klar over at de brukergruppe BAS ert lisensiering.</span><span class="sxs-lookup"><span data-stu-id="b6db8-130">Organizations who have selected this option will be aware that they're using group-based licensing.</span></span>

4. <span data-ttu-id="b6db8-131">Deretter kan du vise en liste over Office-planer som du kan oppgradere til.</span><span class="sxs-lookup"><span data-stu-id="b6db8-131">Next, you can view a list of Office plans that you can upgrade to.</span></span> <span data-ttu-id="b6db8-132">I dette tilfellet finner du Microsoft 365 forretningsplan.</span><span class="sxs-lookup"><span data-stu-id="b6db8-132">In this case, find the Microsoft 365 Business plan.</span></span> <span data-ttu-id="b6db8-133">Du kan rulle nedover hvis du vil vise alle Office-appene og-tjenestene som er inkludert i denne planen.</span><span class="sxs-lookup"><span data-stu-id="b6db8-133">You can scroll down if you want to see all the Office apps and services that are included with this plan.</span></span> <span data-ttu-id="b6db8-134">Under **Microsoft 365 Business**velger du **Oppgrader** for å legge til Microsoft 365 Business i handlekurven.</span><span class="sxs-lookup"><span data-stu-id="b6db8-134">Under **Microsoft 365 Business**, select **Upgrade** to add Microsoft 365 Business to your cart.</span></span>
5. <span data-ttu-id="b6db8-135">I handlevognen:</span><span class="sxs-lookup"><span data-stu-id="b6db8-135">In the cart:</span></span>
    1. <span data-ttu-id="b6db8-136">Vi tar automatisk med lisenser for alle dine nåværende brukere.</span><span class="sxs-lookup"><span data-stu-id="b6db8-136">We'll automatically include licenses for all your current users.</span></span> <span data-ttu-id="b6db8-137">Hvis du trenger flere eller færre lisenser, må du [kjøpe og tilordne disse lisensene enkeltvis](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="b6db8-137">If you need more or fewer licenses, you need to [buy and assign those licenses individually](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users).</span></span>  
    2. <span data-ttu-id="b6db8-138">Du kan justere hvordan du ønsker å betale: månedlig eller årlig.</span><span class="sxs-lookup"><span data-stu-id="b6db8-138">You can adjust how you'd like to pay: monthly or yearly.</span></span> <span data-ttu-id="b6db8-139">Velg rullegardinmenyen for å gjøre ditt valg.</span><span class="sxs-lookup"><span data-stu-id="b6db8-139">Select the drop-down menu to make your choice.</span></span>
6. <span data-ttu-id="b6db8-140">Velg **gå til kassen** der du ser et sammendrag av kjøpet, inkludert betalingsmåten for denne kontoen.</span><span class="sxs-lookup"><span data-stu-id="b6db8-140">Select **Go to Checkout** where you'll see a summary of your purchase, including the payment method for this account.</span></span> <span data-ttu-id="b6db8-141">Du kan også legge til en promo-kode her hvis du har en.</span><span class="sxs-lookup"><span data-stu-id="b6db8-141">You can also add a promo code here if you have one.</span></span>
7. <span data-ttu-id="b6db8-142">Velg **Bestill** for å fullføre kjøpet.</span><span class="sxs-lookup"><span data-stu-id="b6db8-142">Select **Place order** to complete your purchase.</span></span>
<span data-ttu-id="b6db8-143">Det tar Microsoft noen minutter å sette opp nye Service planer.</span><span class="sxs-lookup"><span data-stu-id="b6db8-143">It takes Microsoft a few minutes to set up your new service plans.</span></span> <span data-ttu-id="b6db8-144">Hvis du vil kontrollere fremdriften, velger du **Kontroller oppgraderingsstatus**.</span><span class="sxs-lookup"><span data-stu-id="b6db8-144">To check on progress, select **Check upgrade status**.</span></span> 
1. <span data-ttu-id="b6db8-145">Når planen er klar, må du kanskje fullføre noen ekstra konfigurasjonstrinn i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="b6db8-145">Once your plan is ready, you might need to complete some additional setup steps in the admin center.</span></span> <span data-ttu-id="b6db8-146">I navigasjonsruten velger du **hjem** for å fullføre eventuelle ekstra konfigurasjonstrinn.</span><span class="sxs-lookup"><span data-stu-id="b6db8-146">In the navigation pane, select **Home** to complete any additional setup steps.</span></span>

> [!NOTE]
> <span data-ttu-id="b6db8-147">Du vil motta en forholdsmessig refusjon for Ofifce 365-lisensene du ikke lenger trenger.</span><span class="sxs-lookup"><span data-stu-id="b6db8-147">You'll receive a prorated refund for the Ofifce 365 licenses that you no longer need.</span></span> <span data-ttu-id="b6db8-148">Bankkontoen eller kredittkortet blir belastet omtrent to dager etter at du har konfigurert den nye planen.</span><span class="sxs-lookup"><span data-stu-id="b6db8-148">Your bank account or credit card will be charged about two days after you set up the new plan.</span></span>
  
## <a name="protect-user-devices-and-files"></a><span data-ttu-id="b6db8-149">Beskytt bruker enheter og filer</span><span class="sxs-lookup"><span data-stu-id="b6db8-149">Protect user devices and files</span></span>

<span data-ttu-id="b6db8-150">Nå som Microsoft 365 Business-lisenser er tilordnet, må du fullføre trinnene for å begynne å beskytte enheter og filer.</span><span class="sxs-lookup"><span data-stu-id="b6db8-150">Now that Microsoft 365 Business licenses have been assigned, complete steps to start protecting devices and files.</span></span> <span data-ttu-id="b6db8-151">Du skal bruke noen nye alternativer som er inkludert i navigasjonsruten i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="b6db8-151">You'll use some new options included in the admin center navigation pane.</span></span>
  
1. <span data-ttu-id="b6db8-152">Gå til **enhetens** \> **policyer**i navigasjonsruten i Administrasjonssenter.</span><span class="sxs-lookup"><span data-stu-id="b6db8-152">In the admin center, in the navigation pane, go to **Devices** \> **Policies**.</span></span>
    
2. <span data-ttu-id="b6db8-153">Velg **Legg til**på siden **enhetspolicyer** .</span><span class="sxs-lookup"><span data-stu-id="b6db8-153">On the **Device policies** page, select **Add**.</span></span>
    
3. <span data-ttu-id="b6db8-154">I **Legg til policy** -ruten gi policyen et navn (for eksempel Beskytt arbeidsfiler), og velg deretter en **PolicyType** fra rullegardinlisten.</span><span class="sxs-lookup"><span data-stu-id="b6db8-154">In the **Add policy** pane give the policy a name (for example, Protect work files), and then choose a **Policy type** from the drop-down list.</span></span> 
    
    <span data-ttu-id="b6db8-155">Du kan konfigurere programpolicyer for å beskytte filer på Android-og iPhone-enheter, i tillegg til Windows 10, og du kan konfigurere policyer for enhetskonfigurasjon for firmaets eide Windows 10-enheter.</span><span class="sxs-lookup"><span data-stu-id="b6db8-155">You can set up application policies for protecting files on Android and iPhone devices, as well as Windows 10, and you can set up device configuration policies for company owned Windows 10 devices.</span></span> <span data-ttu-id="b6db8-156">Se følgende koblinger for mer informasjon:</span><span class="sxs-lookup"><span data-stu-id="b6db8-156">See the following links for details:</span></span>
    
  - [<span data-ttu-id="b6db8-157">Angi innstillinger for appbeskyttelse på Android- eller iOS-enheter</span><span class="sxs-lookup"><span data-stu-id="b6db8-157">Set app protection settings for Android or iOS devices</span></span>](app-protection-settings-for-android-and-ios.md)
    
  - [<span data-ttu-id="b6db8-158">Angi innstillinger for appbeskyttelse for Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="b6db8-158">Set application protection settings for Windows 10 devices</span></span>](protection-settings-for-windows-10-devices.md)
    
  - [<span data-ttu-id="b6db8-159">Angi innstillinger for enhetsbeskyttelse for Windows 10-PCer</span><span class="sxs-lookup"><span data-stu-id="b6db8-159">Set device protection settings for Windows 10 PCs</span></span>](protection-settings-for-windows-10-pcs.md)
    
  
4. <span data-ttu-id="b6db8-160">Når du har konfigurert policyer, kan du og de ansatte konfigurere enheter:</span><span class="sxs-lookup"><span data-stu-id="b6db8-160">After you set up policies, you and your employees can set up devices:</span></span>
    
  - <span data-ttu-id="b6db8-161">Hvis Windows-enhetene dine ikke allerede bruker Windows Pro Creator-oppdateringen, må du [oppgradere dem til Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="b6db8-161">If your Windows devices aren't already using the Windows Pro Creator update, you'll need to [upgrade them to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
    
  - <span data-ttu-id="b6db8-162">Se [konfigurere Windows-enheter for Microsoft 365 Business-brukere](set-up-windows-devices.md) for trinn for Windows-enheter.</span><span class="sxs-lookup"><span data-stu-id="b6db8-162">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for steps for Windows devices.</span></span> 
    
  - <span data-ttu-id="b6db8-163">Se [konfigurere mobile enheter for Microsoft 365 Business-brukere](set-up-mobile-devices.md) for trinn for Android-telefoner og iPhone.</span><span class="sxs-lookup"><span data-stu-id="b6db8-163">See [Set up mobile devices for Microsoft 365 Business users](set-up-mobile-devices.md) for steps for Android phones and iPhones.</span></span> 
