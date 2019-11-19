---
title: Øk trussel beskyttelsen for Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
description: Konfigurer samsvarsfunksjoner for å forhindre tap av data og merke sensitive data.
ms.openlocfilehash: 6fae95e8c5e6d133e3163dbdfd3c09cfede11382
ms.sourcegitcommit: 5d11f516e78ea4a74145e19ba2300f0792c8bac1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/19/2019
ms.locfileid: "38715126"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="e7968-103">Definere samsvarsfunksjoner</span><span class="sxs-lookup"><span data-stu-id="e7968-103">Set up compliance features</span></span>

<span data-ttu-id="e7968-104">Microsoft 365 Business leveres med funksjoner som beskytter dataene og enhetene dine, og hjelper deg med å holde dine og kundenes sensitive opplysninger sikre.</span><span class="sxs-lookup"><span data-stu-id="e7968-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="e7968-105">Definere DLP-funksjoner</span><span class="sxs-lookup"><span data-stu-id="e7968-105">Set up DLP features</span></span>

<span data-ttu-id="e7968-106">Se [opprette en DLP-policy fra en mal](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for å få et eksempel på hvordan du konfigurerer en policy for å beskytte mot personlig identifiserbar informasjon (PII).</span><span class="sxs-lookup"><span data-stu-id="e7968-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="e7968-107">DLP leveres med mange maler som er klare til bruk, for mange forskjellige nasjonale innstillinger.</span><span class="sxs-lookup"><span data-stu-id="e7968-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="e7968-108">For eksempel, Australia Financial data, Canada personlig informasjon Act, US Financial data, og så videre.</span><span class="sxs-lookup"><span data-stu-id="e7968-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="e7968-109">Se [hva DLP policy malene inkluderer](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for en fullstendig liste.</span><span class="sxs-lookup"><span data-stu-id="e7968-109">See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="e7968-110">Alle disse malene kan aktiveres på samme måte som PII-mal eksempelet.</span><span class="sxs-lookup"><span data-stu-id="e7968-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="e7968-111">Konfigurere e-oppbevaring med Exchange Online-arkivering</span><span class="sxs-lookup"><span data-stu-id="e7968-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="e7968-112">**Exchange Online arkiverings** lisens funksjoner bidrar til å opprettholde samsvar og forskriftsmessige standarder ved å bevare e-innhold for eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="e7968-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="e7968-113">Det bidrar også til å redusere risikoen hvis det er en rettssak, og gir en måte å gjenopprette data etter et sikkerhetsbrudd eller når du trenger å gjenopprette slettede elementer.</span><span class="sxs-lookup"><span data-stu-id="e7968-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="e7968-114">Du kan bruke rettslig sperre for å bevare alt innholdet til en bruker, eller bruke oppbevaringspolicyer til å tilpasse det du vil beholde.</span><span class="sxs-lookup"><span data-stu-id="e7968-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="e7968-115">**Rettstvist Hold:** Du kan beholde alt postboksinnhold inkludert slettede elementer ved å sette en brukers hele postboksen under rettslig sperre.</span><span class="sxs-lookup"><span data-stu-id="e7968-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="e7968-116">Hvis du vil plassere en postboks under rettslig sperre, i administrasjonssenteret:</span><span class="sxs-lookup"><span data-stu-id="e7968-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="e7968-117">I venstre NAV går du til **brukere** \> **aktive brukere**.</span><span class="sxs-lookup"><span data-stu-id="e7968-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="e7968-118">Velg en bruker med postboksen du vil plassere under rettslig sperre.</span><span class="sxs-lookup"><span data-stu-id="e7968-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="e7968-119">I bruker ruten utvider du **e-postinnstillinger**, og ved siden av **flere innstillinger**velger du **Rediger Exchange-egenskaper**.</span><span class="sxs-lookup"><span data-stu-id="e7968-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="e7968-120">På Postboks-siden for brukeren, velger \* \* postkassen funksjoner \* \* på venstre nav, og velg deretter **Aktiver** kobling under **rettslig sperre**.</span><span class="sxs-lookup"><span data-stu-id="e7968-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="e7968-121">I dialogboksen **rettslig sperre** kan du angi den rettstvist holde varigheten i feltet **rettstvist Hold varighet** .</span><span class="sxs-lookup"><span data-stu-id="e7968-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="e7968-122">La feltet stå tomt hvis du vil plassere et uendelig hold.</span><span class="sxs-lookup"><span data-stu-id="e7968-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="e7968-123">Du kan også legge til notater og dirigere eieren av postboksen til et webområde du kanskje må forklare mer om rettstvist sperringen.</span><span class="sxs-lookup"><span data-stu-id="e7968-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="e7968-124">\>**Lagre**.</span><span class="sxs-lookup"><span data-stu-id="e7968-124">\> **Save**.</span></span>
    
<span data-ttu-id="e7968-125">**Bevaring:** Du kan aktivere egendefinerte oppbevaringspolicyer, for eksempel for å beholde en bestemt tidsperiode eller slette innhold permanent på slutten av oppbevaringsperioden.</span><span class="sxs-lookup"><span data-stu-id="e7968-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="e7968-126">Hvis du vil ha mer informasjon, kan du se [Oversikt over oppbevaringspolicyer](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="e7968-126">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="e7968-127">Sette opp følsomhet etiketter</span><span class="sxs-lookup"><span data-stu-id="e7968-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="e7968-128">Følsomhet etiketter kommer med Azure Information Protection (AIP) plan 1, og hjelper deg med å klassifisere, og eventuelt beskytte dokumenter og e-post, ved å bruke etiketter.</span><span class="sxs-lookup"><span data-stu-id="e7968-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="e7968-129">Etiketter kan brukes automatisk av administratorer som definerer regler og betingelser, manuelt av brukere, eller ved å bruke en kombinasjon der brukere får anbefalinger.</span><span class="sxs-lookup"><span data-stu-id="e7968-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="e7968-130">For å sette opp følsomhet etiketter, se [opprette og administrere følsomhet etiketter](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span><span class="sxs-lookup"><span data-stu-id="e7968-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="e7968-131">Installere Azure Information Protection-klienten manuelt</span><span class="sxs-lookup"><span data-stu-id="e7968-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="e7968-132">Slik installerer du den AIP-klienten manuelt:</span><span class="sxs-lookup"><span data-stu-id="e7968-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="e7968-133">Dataoverføre **AzinfoProtection_UL. exe** fra [Microsoft Dataoverføre Senter](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="e7968-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="e7968-134">Du kan kontrollere at installasjonen fungerte ved å vise et Word-dokument og sørge for at alternativet **følsomhet** er tilgjengelig i kategorien **hjem** .</span><span class="sxs-lookup"><span data-stu-id="e7968-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="e7968-135">![Kategorien beskyttelse i et Word-dokument.](media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="e7968-135">![Protection tab drop-down in a Word document.](media/word-sensitivity.png)</span></span>

<span data-ttu-id="e7968-136">Hvis du vil ha mer informasjon, se [installere klienten](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="e7968-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
