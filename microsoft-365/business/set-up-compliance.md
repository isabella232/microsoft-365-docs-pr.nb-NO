---
title: Øke trusselbeskyttelse for Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
description: Konfigurer samsvarsfunksjoner for å forhindre tap av data og bidra til å holde kundenes sensitive informasjon sikret.
ms.openlocfilehash: 6f4520b052c2e7acb8748d3c9d6e26777cb56d4b
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561244"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="2177e-103">Konfigurere samsvarsfunksjoner</span><span class="sxs-lookup"><span data-stu-id="2177e-103">Set up compliance features</span></span>

<span data-ttu-id="2177e-104">Microsoft 365 Business leveres med funksjoner for å beskytte data og enheter, og hjelper deg med å holde den sensitive informasjonen din og kundenes sensitive informasjon sikker.</span><span class="sxs-lookup"><span data-stu-id="2177e-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep your and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="2177e-105">Konfigurere DLP-funksjoner</span><span class="sxs-lookup"><span data-stu-id="2177e-105">Set up DLP features</span></span>

<span data-ttu-id="2177e-106">Se [Opprette en DLP-policy fra en mal](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for eksempel hvordan du konfigurerer en policy for å beskytte mot personlig identifiserbar informasjon (PII).</span><span class="sxs-lookup"><span data-stu-id="2177e-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="2177e-107">DLP leveres med mange policymaler som er klare til bruk for mange forskjellige nasjonale innstillinger.</span><span class="sxs-lookup"><span data-stu-id="2177e-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="2177e-108">For eksempel, Australia Financial Data, Canada Personal Information Act, US Financial Data, og så videre.</span><span class="sxs-lookup"><span data-stu-id="2177e-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, and so on.</span></span> <span data-ttu-id="2177e-109">Se [Hva DLP-policymalene inneholder](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for en fullstendig liste.</span><span class="sxs-lookup"><span data-stu-id="2177e-109">See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="2177e-110">Alle disse malene kan aktiveres på samme måte som pii-maleksemplet.</span><span class="sxs-lookup"><span data-stu-id="2177e-110">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="2177e-111">Konfigurere e-postoppbevaring med Exchange Online-arkivering</span><span class="sxs-lookup"><span data-stu-id="2177e-111">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="2177e-112">**Lisensfunksjoner for Exchange Online Arkivering** bidrar til å opprettholde samsvars- og forskriftsstandarder ved å bevare e-postinnhold for eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="2177e-112">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="2177e-113">Det bidrar også til å redusere risikoen hvis det er et søksmål, og gir en måte å gjenopprette data etter et sikkerhetsbrudd eller når du trenger å gjenopprette slettede elementer.</span><span class="sxs-lookup"><span data-stu-id="2177e-113">It also helps reduce your risk if there is a lawsuit, and provides a way to recover data after a security breach or when you need to recover deleted items.</span></span> <span data-ttu-id="2177e-114">Du kan bruke rettstvistsperring til å bevare alt innholdet i en bruker, eller bruke oppbevaringspolicyer til å tilpasse det du vil beholde.</span><span class="sxs-lookup"><span data-stu-id="2177e-114">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="2177e-115">**Rettstvist hold:** Du kan beholde alt postboksinnhold, inkludert slettede elementer, ved å sette hele postboksen til en bruker på rettstvist.</span><span class="sxs-lookup"><span data-stu-id="2177e-115">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="2177e-116">Hvis du vil plassere en postboks på rettslig sperre, i administrasjonssenteret:</span><span class="sxs-lookup"><span data-stu-id="2177e-116">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="2177e-117">Gå til **Brukere** \> **aktive brukere**i venstre navigasjonsenhet.</span><span class="sxs-lookup"><span data-stu-id="2177e-117">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="2177e-118">Velg en bruker du vil plassere postboksen for å plassere på rettstvistsperring.</span><span class="sxs-lookup"><span data-stu-id="2177e-118">Select a user whose mailbox you want to place on litigation hold.</span></span> <span data-ttu-id="2177e-119">I brukerruten utvider du **E-postinnstillinger**og ved siden av **Flere innstillinger**, velger **Rediger Exchange-egenskaper**.</span><span class="sxs-lookup"><span data-stu-id="2177e-119">In the user pane, expand **Mail settings**, and next to **More settings**, choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="2177e-120">Velg \*\* postboksfunksjoner \*\* til venstre, på postbokssiden for brukeren, og velg deretter **Koblingen Aktiver** under **Sperreavhold**.</span><span class="sxs-lookup"><span data-stu-id="2177e-120">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="2177e-121">I dialogboksen **sperreavrettslig sperre** kan du angi varigheten for rettstvistsperren i feltet **Sperrevarighet for rettstvist.**</span><span class="sxs-lookup"><span data-stu-id="2177e-121">In the **litigation hold** dialog box, you can specify the litigation hold duration in the **Litigation hold duration** field.</span></span> <span data-ttu-id="2177e-122">La feltet stå tomt hvis du vil plassere et uendelig hold.</span><span class="sxs-lookup"><span data-stu-id="2177e-122">Leave the field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="2177e-123">Du kan også legge til notater og dirigere eieren av postboksen til et nettsted du kanskje må forklare mer om rettstvistsperren.</span><span class="sxs-lookup"><span data-stu-id="2177e-123">You can also add notes and direct the mailbox owner to a website you might have to explain more about the litigation hold.</span></span> <span data-ttu-id="2177e-124">\>**Lagre**.</span><span class="sxs-lookup"><span data-stu-id="2177e-124">\> **Save**.</span></span>
    
<span data-ttu-id="2177e-125">**Oppbevaring:** Du kan aktivere egendefinerte oppbevaringspolicyer, for eksempel for å bevare for en bestemt tidsperiode eller slette innhold permanent på slutten av oppbevaringsperioden.</span><span class="sxs-lookup"><span data-stu-id="2177e-125">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="2177e-126">Hvis du vil ha mer informasjon, kan du se [Oversikt over oppbevaringspolicyer](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="2177e-126">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-sensitivity-labels"></a><span data-ttu-id="2177e-127">Konfigurere følsomhetsetiketter</span><span class="sxs-lookup"><span data-stu-id="2177e-127">Set up Sensitivity labels</span></span>

<span data-ttu-id="2177e-128">Følsomhetsetiketter leveres med Azure Information Protection (AIP) Plan 1, og hjelper deg med å klassifisere, og eventuelt beskytte dokumenter og e-postmeldinger ved å bruke etiketter.</span><span class="sxs-lookup"><span data-stu-id="2177e-128">Sensitivity labels come with Azure Information Protection (AIP) Plan 1, and help you classify, and optionally protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="2177e-129">Etiketter kan brukes automatisk av administratorer som definerer regler og betingelser, manuelt av brukere, eller ved hjelp av en kombinasjon der brukerne får anbefalinger.</span><span class="sxs-lookup"><span data-stu-id="2177e-129">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="2177e-130">Hvis du vil konfigurere Følsomhetsetiketter, kan du vise [video om oppretting og administrering av følsomhetsetiketter.](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9)</span><span class="sxs-lookup"><span data-stu-id="2177e-130">To set up Sensitivity labels, view [create and manage sensitivity labels](https://support.office.com/article/2fb96b54-7dd2-4f0c-ac8d-170790d4b8b9) video.</span></span>



### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="2177e-131">Installere Azure Information Protection-klienten manuelt</span><span class="sxs-lookup"><span data-stu-id="2177e-131">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="2177e-132">Slik installerer du AIP-klienten manuelt:</span><span class="sxs-lookup"><span data-stu-id="2177e-132">To manually install the AIP client:</span></span>

1. <span data-ttu-id="2177e-133">Last ned **AzinfoProtection_UL.exe** fra [Microsoft nedlastingssenter](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="2177e-133">Download **AzinfoProtection_UL.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="2177e-134">Du kan kontrollere at installasjonen fungerte ved å vise et Word-dokument og kontrollere at alternativet **Følsomhet** er tilgjengelig i kategorien **Hjem.**</span><span class="sxs-lookup"><span data-stu-id="2177e-134">You can verify that the installation worked by viewing a Word document and making sure that the **Sensitivity** option is available on the **Home** tab.</span></span>
<br/><span data-ttu-id="2177e-135">![Rullegardinlisten Beskyttelse-fanen i et Word-dokument.](../media/word-sensitivity.png)</span><span class="sxs-lookup"><span data-stu-id="2177e-135">![Protection tab drop-down in a Word document.](../media/word-sensitivity.png)</span></span>

<span data-ttu-id="2177e-136">Hvis du vil ha mer informasjon, kan du se [Installere klienten](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="2177e-136">For more information, see [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
