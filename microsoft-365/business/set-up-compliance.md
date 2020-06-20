---
title: Øke trusselbeskyttelsen for Microsoft 365 Business Premium
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
description: Konfigurer samsvarsfunksjoner for å forhindre tap av data og bidra til å holde og kundenes sensitive informasjon sikker.
ms.openlocfilehash: 18886ff3a0ba5e99e63c70ef083d7a69c75bac91
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785836"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="65012-103">Konfigurere samsvarsfunksjoner</span><span class="sxs-lookup"><span data-stu-id="65012-103">Set up compliance features</span></span>

<span data-ttu-id="65012-104">Microsoft 365 Business Premium leveres med funksjoner for å beskytte dataene og enhetene dine, og hjelper deg med å holde og kundenes sensitive informasjon sikker.</span><span class="sxs-lookup"><span data-stu-id="65012-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="65012-105">Konfigurere DLP-funksjoner</span><span class="sxs-lookup"><span data-stu-id="65012-105">Set up DLP features</span></span>

<span data-ttu-id="65012-106">Se [Opprette en DLP-policy fra en mal,](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for eksempel på hvordan du definerer en policy for å beskytte mot personlig identifiserbar informasjon (PII).</span><span class="sxs-lookup"><span data-stu-id="65012-106">See [Create a DLP policy from a template](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="65012-107">DLP leveres med mange policymaler som er klare til bruk for mange forskjellige lokaliteter.</span><span class="sxs-lookup"><span data-stu-id="65012-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="65012-108">For eksempel, Australia Financial Data, Canada Personal Information Act, US Financial Data, og så videre.</span><span class="sxs-lookup"><span data-stu-id="65012-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="65012-109">Se [Hva DLP-policymalene inkluderer](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) for en fullstendig liste.</span><span class="sxs-lookup"><span data-stu-id="65012-109">See [What the DLP policy templates include](https://docs.microsoft.com/microsoft-365/compliance/what-the-dlp-policy-templates-include) for a full list.</span></span> <span data-ttu-id="65012-110">Alle disse malene kan aktiveres på samme måte som eksempelet på PII-malen.</span><span class="sxs-lookup"><span data-stu-id="65012-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="65012-111">Konfigurere oppbevaring av e-post med Exchange Online-arkivering</span><span class="sxs-lookup"><span data-stu-id="65012-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="65012-112">**Exchange Online Arkivering** lisensfunksjoner bidra til å opprettholde samsvar og forskriftsmessig standarder ved å bevare e-postinnhold for eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="65012-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="65012-113">Det bidrar også til å redusere risikoen hvis det er et søksmål, og gir en måte å gjenopprette data etter et sikkerhetsbrudd eller når du trenger å gjenopprette slettede elementer.</span><span class="sxs-lookup"><span data-stu-id="65012-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="65012-114">Du kan bruke rettslig sperre til å bevare alt innholdet til en bruker, eller bruke oppbevaringspolicyer til å tilpasse det du vil beholde.</span><span class="sxs-lookup"><span data-stu-id="65012-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="65012-115">**Rettstvister holder:** Du kan beholde alt postboksinnhold, inkludert slettede elementer, ved å sette hele postboksen til en bruker på rettslig sperre.</span><span class="sxs-lookup"><span data-stu-id="65012-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="65012-116">Hvis du vil plassere en postboks på rettslig sperre, i administrasjonssenteret:</span><span class="sxs-lookup"><span data-stu-id="65012-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="65012-117">Gå til **Brukere** Aktive brukere i venstre \> **Active users**navigasjonsenhet.</span><span class="sxs-lookup"><span data-stu-id="65012-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="65012-118">Velg en bruker som har postboksen du vil plassere på rettslig sperre.</span><span class="sxs-lookup"><span data-stu-id="65012-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="65012-119">Utvid **E-postinnstillinger**i brukerruten, og velg **Rediger Exchange-egenskaper**ved siden av **Flere innstillinger**.</span><span class="sxs-lookup"><span data-stu-id="65012-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="65012-120">Velg \*\* postboksfunksjoner \*\* i venstre navigasjonsrute på postbokssiden for brukeren, og velg deretter **Aktiver-koblingen** under **Prosedyresperre**.</span><span class="sxs-lookup"><span data-stu-id="65012-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="65012-121">I dialogboksen **prosedyresperre** kan du angi varigheten for rettstvisthold i feltet Varighet for **rettstvisthold.**</span><span class="sxs-lookup"><span data-stu-id="65012-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="65012-122">La feltet stå tomt hvis du vil plassere et uendelig grep.</span><span class="sxs-lookup"><span data-stu-id="65012-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="65012-123">Du kan også legge til notater og dirigere eieren av postboksen til et webområde du kanskje må forklare mer om rettstvistholdet.</span><span class="sxs-lookup"><span data-stu-id="65012-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="65012-124">\>**Lagre**.</span><span class="sxs-lookup"><span data-stu-id="65012-124">\> **Save**.</span></span>
    
<span data-ttu-id="65012-125">**Oppbevaring:** Du kan for eksempel aktivere tilpassede oppbevaringspolicyer for å bevare for en bestemt tidsperiode eller slette innhold permanent på slutten av oppbevaringsperioden.</span><span class="sxs-lookup"><span data-stu-id="65012-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="65012-126">Hvis du vil ha mer informasjon, kan du se [Oversikt over oppbevaringspolicyer](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span><span class="sxs-lookup"><span data-stu-id="65012-126">To learn more, see [Overview of retention policies](https://docs.microsoft.com/microsoft-365/compliance/retention-policies).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="65012-127">Definere følsomhetsetiketter</span><span class="sxs-lookup"><span data-stu-id="65012-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="65012-128">Følsomhetsetiketter leveres med AIP-plan (Azure Information Protection) Plan 1, og hjelper deg med å klassifisere og eventuelt beskytte dokumenter og e-postmeldinger ved å bruke etiketter.</span><span class="sxs-lookup"><span data-stu-id="65012-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="65012-129">Etiketter kan brukes automatisk av administratorer som definerer regler og betingelser, manuelt av brukere eller ved hjelp av en kombinasjon der brukerne får anbefalinger.</span><span class="sxs-lookup"><span data-stu-id="65012-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="65012-130">Hvis du vil konfigurere følsomhetsetiketter, kan du vise [opprette og administrere følsomhetsetiketter](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span><span class="sxs-lookup"><span data-stu-id="65012-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.microsoft.com/office/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="65012-131">Installere Azure Information Protection-klienten manuelt</span><span class="sxs-lookup"><span data-stu-id="65012-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="65012-132">Slik installerer du AIP-klienten manuelt:</span><span class="sxs-lookup"><span data-stu-id="65012-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="65012-133">Last ned **AzinfoProtection_UL.exe** fra [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="65012-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="65012-134">Du kan kontrollere at installasjonen fungerte ved å vise et Word-dokument og sørge for at **alternativet Følsomhet** er tilgjengelig i kategorien **Hjem.**</span><span class="sxs-lookup"><span data-stu-id="65012-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="65012-135">![Rullegardinlisten Beskyttelsesfane i et Word-dokument.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="65012-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="65012-136">Hvis du vil ha mer informasjon, kan du se [Installere klienten](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="65012-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
