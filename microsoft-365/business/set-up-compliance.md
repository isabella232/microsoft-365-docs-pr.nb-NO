---
title: Øke trussel beskyttelse for Microsoft 365 Business Premium
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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Konfigurer samsvars funksjoner for å hindre tap av data, og bidra til at dine og kundenes sensitive opplysninger sikres.
ms.openlocfilehash: 2c95ad3f36df28af2c68cd11192bcfe92dfe29e3
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841177"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="bbbc0-103">Konfigurere samsvars funksjoner</span><span class="sxs-lookup"><span data-stu-id="bbbc0-103">Set up compliance features</span></span>

<span data-ttu-id="bbbc0-104">Microsoft 365 Business Premium leveres med funksjoner for å beskytte dataene og enhetene dine, og hjelper deg med å holde kundenes sensitive opplysninger sikre.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="bbbc0-105">Konfigurere DLP-funksjoner</span><span class="sxs-lookup"><span data-stu-id="bbbc0-105">Set up DLP features</span></span>

<span data-ttu-id="bbbc0-106">Se [opprette en DLP-policy fra en mal](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for et eksempel på hvordan du konfigurerer en policy for beskyttelse mot beskyttelse av tap av personlige data.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-106">See [Create a DLP policy from a template](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="bbbc0-107">DLP leveres med mange policyer som er klare til bruk for mange forskjellige nasjonale innstillinger.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="bbbc0-108">Økonomiske data, Canada, personlig informasjon, for eksempel, USA, økonomiske data og så videre.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="bbbc0-109">Se [hvordan policy malene for DLP inkluderer](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) en fullstendig liste.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-109">See [What the DLP policy templates include](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) for a full list.</span></span> <span data-ttu-id="bbbc0-110">Alle disse malene kan være aktivert på samme måte som for eksempel malen PII.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="bbbc0-111">Konfigurere e-postoppbevaring med Exchange Online-arkivering</span><span class="sxs-lookup"><span data-stu-id="bbbc0-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="bbbc0-112">Lisens funksjoner for å **arkivere Exchange Online** hjelper deg med å vedlikeholde samsvar og forskriftsmessige standarder ved å beholde e-postinnhold for eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="bbbc0-113">Det bidrar også til å redusere risikoen hvis det finnes en lawsuit, og gir deg en mulighet til å gjenopprette data etter et brudd eller når du må gjenopprette slettede elementer.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="bbbc0-114">Du kan bruke søksmål hold for å bevare hele en brukers innhold, eller bruke oppbevarings policyer til å tilpasse hva du vil beholde.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="bbbc0-115">**Rettslig sperre:** Du kan bevare alt innholdet i post boksen, inkludert slettede elementer ved å legge inn en brukers fullstendige post boks på en rettslig sperre.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="bbbc0-116">Hvis du vil plassere en post boks på en rettslig sperre, kan du i administrasjons senteret:</span><span class="sxs-lookup"><span data-stu-id="bbbc0-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="bbbc0-117">Gå til **brukere** som \> **aktive brukere** i venstre navigasjons rute.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="bbbc0-118">Velg en bruker som har post boksen du vil plassere på en rettslig sperre.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="bbbc0-119">I bruker-ruten utvider du **e-postinnstillinger** og klikker **Rediger Exchange-egenskaper** ved siden av **flere innstillinger**.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-119">In the user pane, expand **Mail settings** , and next to **More settings** , choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="bbbc0-120">På Postboks-siden for brukeren velger du \* \* post boks funksjoner \* \* i det venstre navigasjons feltet, og deretter velger du **Aktiver** -koblingen under **rettslig sperring**.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="bbbc0-121">I dialog boksen retts **tvist** kan du angi den rettslige sperrings varigheten i **varighets** feltet for søksmål-vent.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="bbbc0-122">La feltet stå tomt hvis du vil plassere en uendelig sperring.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="bbbc0-123">Du kan også legge til notater og dirigere eieren av post boksen til et nettsted du kanskje må forklare mer om den rettslige sperringen.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="bbbc0-124">\>**Lagre**.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-124">\> **Save**.</span></span>
    
<span data-ttu-id="bbbc0-125">**Oppbevaring:** Du kan aktivere tilpassede oppbevarings policyer, for eksempel for å beholde en bestemt tids periode, eller slette innhold permanent på slutten av oppbevarings perioden.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="bbbc0-126">Hvis du vil ha mer informasjon, kan du se [Oversikt over oppbevarings policyer](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span><span class="sxs-lookup"><span data-stu-id="bbbc0-126">To learn more, see [Overview of retention policies](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="bbbc0-127">Konfigurere følsomhet og etiketter</span><span class="sxs-lookup"><span data-stu-id="bbbc0-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="bbbc0-128">Følsomme etiketter leveres med Azure Information Protection, plan 1 og hjelper deg med å klassifisere, og du kan også beskytte dokumentene og e-postmeldingene dine ved å bruke etiketter.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="bbbc0-129">Etiketter kan brukes automatisk av administratorer som definerer regler og betingelser, manuelt av brukere eller ved å bruke en kombinasjon der brukere får anbefalinger.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="bbbc0-130">Hvis du vil sette opp følsomhet for etiketter, kan du vise video om å [opprette og behandle følsomhet](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) .</span><span class="sxs-lookup"><span data-stu-id="bbbc0-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="bbbc0-131">Installere Azure Information Protection-klienten manuelt</span><span class="sxs-lookup"><span data-stu-id="bbbc0-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="bbbc0-132">Slik installerer du den administrative klienten manuelt:</span><span class="sxs-lookup"><span data-stu-id="bbbc0-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="bbbc0-133">Last ned **AzinfoProtection_UL.exe** fra [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="bbbc0-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="bbbc0-134">Du kan kontrollere at installasjonen fungerte ved å vise et Word-dokument og sørge for at alternativet **følsomhet** er tilgjengelig på **hjem** -fanen.</span><span class="sxs-lookup"><span data-stu-id="bbbc0-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="bbbc0-135">![Kategorien beskyttelse i et Word-dokument.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="bbbc0-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="bbbc0-136">Hvis du vil ha mer informasjon, kan du se [installere klienten](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="bbbc0-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
