---
title: Øk trusselbeskyttelsen for Microsoft 365 Business Premium
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
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Konfigurer samsvarsfunksjoner for å forhindre tap av data og bidra til å holde sensitiv informasjon for deg og kundene dine sikre.
ms.openlocfilehash: 945f8a283b90b89da2fbe67a073e0807b80d198f
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/06/2021
ms.locfileid: "52245088"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="1abf5-103">Konfigurere samsvarsfunksjoner</span><span class="sxs-lookup"><span data-stu-id="1abf5-103">Set up compliance features</span></span>

<span data-ttu-id="1abf5-104">Din Microsoft 365 Business Premium leveres med funksjoner for å beskytte data og enheter, og hjelpe deg med å holde dine og kundenes sensitive opplysninger sikre.</span><span class="sxs-lookup"><span data-stu-id="1abf5-104">Your Microsoft 365 Business Premium comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="1abf5-105">Konfigurere DLP-funksjoner</span><span class="sxs-lookup"><span data-stu-id="1abf5-105">Set up DLP features</span></span>

<span data-ttu-id="1abf5-106">Se [Opprette en DLP-policy fra en](../compliance/create-a-dlp-policy-from-a-template.md) mal for et eksempel på hvordan du konfigurerer en policy for å beskytte mot å beskytte tap av personlige data.</span><span class="sxs-lookup"><span data-stu-id="1abf5-106">See [Create a DLP policy from a template](../compliance/create-a-dlp-policy-from-a-template.md) for an example on how to set up a policy to protect against protect loss of personal data.</span></span> 
  
<span data-ttu-id="1abf5-107">DLP leveres med mange policymaler som er klare til bruk for mange forskjellige nasjonale land.</span><span class="sxs-lookup"><span data-stu-id="1abf5-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="1abf5-108">For eksempel Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, og så videre.</span><span class="sxs-lookup"><span data-stu-id="1abf5-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="1abf5-109">Se [Hva DLP-policymalene inneholder](../compliance/what-the-dlp-policy-templates-include.md) for en fullstendig liste.</span><span class="sxs-lookup"><span data-stu-id="1abf5-109">See [What the DLP policy templates include](../compliance/what-the-dlp-policy-templates-include.md) for a full list.</span></span> <span data-ttu-id="1abf5-110">Alle disse malene kan aktiveres på samme måte som eksempelet på PII-malen.</span><span class="sxs-lookup"><span data-stu-id="1abf5-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="1abf5-111">Konfigurere e-postoppbevaring med Exchange Online Archiving</span><span class="sxs-lookup"><span data-stu-id="1abf5-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="1abf5-112">**Exchange Online Archiving** lisensfunksjoner bidrar til å opprettholde samsvar og forskriftsmessige standarder ved å bevare e-postinnhold for eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="1abf5-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="1abf5-113">Det bidrar også til å redusere risikoen hvis det er et søksmål, og gir en måte å gjenopprette data på etter et sikkerhetsbrudd eller når du trenger å gjenopprette slettede elementer.</span><span class="sxs-lookup"><span data-stu-id="1abf5-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="1abf5-114">Du kan bruke rettslig sperring for å bevare alt innholdet til en bruker, eller bruke oppbevaringspolicyer til å tilpasse det du vil bevare.</span><span class="sxs-lookup"><span data-stu-id="1abf5-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="1abf5-115">**Rettslig sperre:** Du kan bevare alt postboksinnhold, inkludert slettede elementer, ved å sette hele postboksen til en bruker på rettslig sperre.</span><span class="sxs-lookup"><span data-stu-id="1abf5-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="1abf5-116">Slik plasserer du en postboks på rettslig sperre i administrasjonssenteret:</span><span class="sxs-lookup"><span data-stu-id="1abf5-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="1abf5-117">Gå til Brukere aktive  brukere i det venstre \> **navigasjonsfeltet.**</span><span class="sxs-lookup"><span data-stu-id="1abf5-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="1abf5-118">Velg en bruker som har postboksen du vil plassere på rettslig sperre.</span><span class="sxs-lookup"><span data-stu-id="1abf5-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="1abf5-119">Utvid E-postinnstillinger **i** brukerruten, og ved siden av Flere innstillinger **velger** du **Rediger Exchange egenskaper**.</span><span class="sxs-lookup"><span data-stu-id="1abf5-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="1abf5-120">Velg \*\* postboksfunksjoner \*\* til venstre på postbokssiden for brukeren,  og velg deretter Aktiver-koblingen under **Rettslig sperring**.</span><span class="sxs-lookup"><span data-stu-id="1abf5-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="1abf5-121">I dialogboksen **Sperre for** rettslig sperre kan du angi varigheten for rettslig sperring i feltet Varighet **for** rettslig sperre.</span><span class="sxs-lookup"><span data-stu-id="1abf5-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="1abf5-122">La feltet stå tomt hvis du vil plassere en uendelig sperring.</span><span class="sxs-lookup"><span data-stu-id="1abf5-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="1abf5-123">Du kan også legge til notater og dirigere eieren av postboksen til et nettsted som du kanskje må forklare mer om rettslig sperre.</span><span class="sxs-lookup"><span data-stu-id="1abf5-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="1abf5-124">\>**Lagre**.</span><span class="sxs-lookup"><span data-stu-id="1abf5-124">\> **Save**.</span></span>
    
<span data-ttu-id="1abf5-125">**Oppbevaring:** Du kan aktivere tilpassede oppbevaringspolicyer, for eksempel for å bevare for en bestemt tidsperiode eller slette innhold permanent på slutten av oppbevaringsperioden.</span><span class="sxs-lookup"><span data-stu-id="1abf5-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="1abf5-126">Hvis du vil ha mer informasjon, [kan du se Oversikt over oppbevaringspolicyer](../compliance/retention.md).</span><span class="sxs-lookup"><span data-stu-id="1abf5-126">To learn more, see [Overview of retention policies](../compliance/retention.md).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="1abf5-127">Konfigurere følsomhetsetiketter</span><span class="sxs-lookup"><span data-stu-id="1abf5-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="1abf5-128">Følsomhetsetiketter leveres med Azure Information Protection (AIP) Plan 1, og hjelper deg med å klassifisere og eventuelt beskytte dokumenter og e-postmeldinger ved å bruke etiketter.</span><span class="sxs-lookup"><span data-stu-id="1abf5-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="1abf5-129">Etiketter kan brukes automatisk av administratorer som definerer regler og betingelser, manuelt av brukere, eller ved hjelp av en kombinasjon der brukerne får anbefalinger.</span><span class="sxs-lookup"><span data-stu-id="1abf5-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="1abf5-130">Hvis du vil konfigurere følsomhetsetiketter, [kan du vise video om oppretting og behandling av følsomhetsetiketter.](../business-video/create-sensitivity-labels.md)</span><span class="sxs-lookup"><span data-stu-id="1abf5-130">To set up Sensitivity labels, view [create and manage sensitivity labels](../business-video/create-sensitivity-labels.md) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="1abf5-131">Installere Azure Information Protection-klienten manuelt</span><span class="sxs-lookup"><span data-stu-id="1abf5-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="1abf5-132">Slik installerer du AIP-klienten manuelt:</span><span class="sxs-lookup"><span data-stu-id="1abf5-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="1abf5-133">Last **AzinfoProtection_UL.exe** fra [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="1abf5-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="1abf5-134">Du kan kontrollere at installasjonen fungerte ved å vise et Word-dokument og kontrollere at **Følsomhet-alternativet** er tilgjengelig på **Hjem-fanen.**</span><span class="sxs-lookup"><span data-stu-id="1abf5-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="1abf5-135">![Rullegardinmenyen Beskyttelse-fanen i et Word-dokument.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="1abf5-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="1abf5-136">Hvis du vil ha mer informasjon, [kan du se Installere klienten](/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="1abf5-136">For more information, see [Install the client](/azure/information-protection/infoprotect-tutorial-step3).</span></span>