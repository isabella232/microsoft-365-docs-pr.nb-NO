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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
description: Konfigurer Office 365 avansert trusselbeskyttelse, og Beskytt sensitive data.
ms.openlocfilehash: 8144bcebe8a0cdf28a5e092f592362922ccbdd48
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288749"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="3e11a-103">Definere samsvarsfunksjoner</span><span class="sxs-lookup"><span data-stu-id="3e11a-103">Set up compliance features</span></span>

<span data-ttu-id="3e11a-104">Microsoft 365 Business leveres med funksjoner som beskytter dataene og enhetene dine, og hjelper deg med å holde dine og kundenes sensitive opplysninger sikre.</span><span class="sxs-lookup"><span data-stu-id="3e11a-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="3e11a-105">Definere DLP-funksjoner</span><span class="sxs-lookup"><span data-stu-id="3e11a-105">Set up DLP features</span></span>

<span data-ttu-id="3e11a-106">Se [opprette en DLP-policy fra en mal](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for å få et eksempel på hvordan du konfigurerer en policy for å beskytte mot personlig identifiserbar informasjon (PII).</span><span class="sxs-lookup"><span data-stu-id="3e11a-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="3e11a-107">DLP leveres med mange maler som er klare til bruk, for mange forskjellige nasjonale innstillinger.</span><span class="sxs-lookup"><span data-stu-id="3e11a-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="3e11a-108">For eksempel, Australia Financial data, Canada personlig informasjon Act, amerikanske finansielle data, etc. Se [hva DLP policy malene inkluderer](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for en fullstendig liste.</span><span class="sxs-lookup"><span data-stu-id="3e11a-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="3e11a-109">Alle disse malene kan aktiveres på samme måte som PII-mal eksempelet.</span><span class="sxs-lookup"><span data-stu-id="3e11a-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="3e11a-110">Konfigurere e-oppbevaring med Exchange Online-arkivering</span><span class="sxs-lookup"><span data-stu-id="3e11a-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="3e11a-111">**Exchange Online arkiverings** lisens funksjoner bidrar til å opprettholde samsvar og forskriftsmessige standarder ved å bevare e-innhold for eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="3e11a-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="3e11a-112">Det bidrar også til å redusere risikoen i tilfelle en rettssak og gir en måte å gjenopprette data etter et sikkerhetsbrudd, eller når du trenger å gjenopprette slettede elementer.</span><span class="sxs-lookup"><span data-stu-id="3e11a-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="3e11a-113">Du kan bruke rettslig sperre for å bevare alt innholdet til en bruker, eller bruke oppbevaringspolicyer til å tilpasse det du vil beholde.</span><span class="sxs-lookup"><span data-stu-id="3e11a-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="3e11a-114">**Rettstvist Hold:** Du kan beholde alt postboksinnhold inkludert slettede elementer ved å sette en brukers hele postboksen under rettslig sperre.</span><span class="sxs-lookup"><span data-stu-id="3e11a-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="3e11a-115">Hvis du vil plassere en postboks under rettslig sperre, i administrasjonssenteret:</span><span class="sxs-lookup"><span data-stu-id="3e11a-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="3e11a-116">I venstre NAV går du til **brukere** \> **aktive brukere**.</span><span class="sxs-lookup"><span data-stu-id="3e11a-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="3e11a-117">Velg en bruker som har postboksen du vil plassere ved rettslig sperre, og i bruker ruten utvider du **e-postinnstillinger** og ved siden av **flere innstillinger** Velg **Rediger Exchange-egenskaper**.</span><span class="sxs-lookup"><span data-stu-id="3e11a-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="3e11a-118">På Postboks-siden for brukeren, velger \* \* postkassen funksjoner \* \* på venstre nav, og velg deretter **Aktiver** kobling under **rettslig sperre**.</span><span class="sxs-lookup"><span data-stu-id="3e11a-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="3e11a-119">I dialogboksen **rettslig sperre** kan du angi den rettstvist holde varigheten i feltet **rettstvist Hold varighet** , la feltet stå tomt hvis du vil plassere et uendelig hold.</span><span class="sxs-lookup"><span data-stu-id="3e11a-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="3e11a-120">Du kan også legge til notater og dirigere postbokseieren til et webområde du kanskje må forklare mer om den rettslige sperren \> **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="3e11a-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="3e11a-121">**Bevaring:** Du kan aktivere egendefinerte oppbevaringspolicyer, for eksempel for å beholde en bestemt tidsperiode eller slette innhold permanent på slutten av oppbevaringsperioden.</span><span class="sxs-lookup"><span data-stu-id="3e11a-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="3e11a-122">Hvis du vil ha mer informasjon, kan du se [Oversikt over oppbevaringspolicyer](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="3e11a-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-azure-information-protection-features"></a><span data-ttu-id="3e11a-123">Konfigurere funksjoner for Azure informasjonsbeskyttelse</span><span class="sxs-lookup"><span data-stu-id="3e11a-123">Set up Azure Information Protection features</span></span>

<span data-ttu-id="3e11a-124">Azure Information Protection (AIP) hjelper deg med å klassifisere og eventuelt beskytte dokumentene og e-postmeldingene ved å bruke etiketter.</span><span class="sxs-lookup"><span data-stu-id="3e11a-124">Azure Information Protection (AIP) helps you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="3e11a-125">Etiketter kan brukes automatisk av administratorer som definerer regler og betingelser, manuelt av brukere, eller ved å bruke en kombinasjon der brukere får anbefalinger.</span><span class="sxs-lookup"><span data-stu-id="3e11a-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="3e11a-126">I Outlook på nettet kan du bruke følgende innebygde etiketter og begrensninger på e-postene dine:</span><span class="sxs-lookup"><span data-stu-id="3e11a-126">In Outlook on the web you can apply the following built-in labels and restrictions to your emails:</span></span>
  
- <span data-ttu-id="3e11a-127">**Ikke Videresend**: mottakerne kan lese meldingen, men de kan ikke videresende, skrive ut eller kopiere innhold</span><span class="sxs-lookup"><span data-stu-id="3e11a-127">**Do Not Forward**: Recipients can read the message, but they can't forward, print, or copy content</span></span>
    
- <span data-ttu-id="3e11a-128">**Krypter**: hele meldingen er kryptert.</span><span class="sxs-lookup"><span data-stu-id="3e11a-128">**Encrypt**: The entire message is encrypted.</span></span> <span data-ttu-id="3e11a-129">Mottakerne må bekrefte identiteten sin før de får tilgang til kryptert innhold og ikke kan fjerne kryptering.</span><span class="sxs-lookup"><span data-stu-id="3e11a-129">Recipients must confirm their identity before accessing encrypted content and can't remove encryption.</span></span>
    
- <span data-ttu-id="3e11a-130">**Konfidensielt**: gir de ansatte i organisasjonen full tilgang til e-innhold og vedlegg, men ikke til personer utenfor organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="3e11a-130">**Confidential**: Gives the employees in your organization full permissions to the email content and attachments, but not to people outside your organization.</span></span> <span data-ttu-id="3e11a-131">Data eiere kan spore og tilbakekalle innhold på et hvilket som helst tidspunkt.</span><span class="sxs-lookup"><span data-stu-id="3e11a-131">Data owners can track and revoke content at any point.</span></span>
    
- <span data-ttu-id="3e11a-132">**Svært konfidensielt**: denne begrensningen kan brukes på svært konfidensielle data, slik at de ansatte til å vise, redigere og svare, men ikke videresende, skrive ut eller kopiere dataene.</span><span class="sxs-lookup"><span data-stu-id="3e11a-132">**Highly Confidential**: This restriction can be applied to highly confidential data, allowing employees to view, edit, and reply, but not forward, print, or copy the data.</span></span> <span data-ttu-id="3e11a-133">Data eiere kan spore og tilbakekalle innhold på et hvilket som helst tidspunkt.</span><span class="sxs-lookup"><span data-stu-id="3e11a-133">Data owners can track and revoke content at any point.</span></span>

### <a name="make-sure-azure-information-protection-is-activated"></a><span data-ttu-id="3e11a-134">Kontroller at Azure Information Protection er aktivert</span><span class="sxs-lookup"><span data-stu-id="3e11a-134">Make sure Azure Information Protection is activated</span></span>

<span data-ttu-id="3e11a-135">Slik kontrollerer du at AIP er aktivert:</span><span class="sxs-lookup"><span data-stu-id="3e11a-135">To verify that AIP is activated :</span></span>

1. <span data-ttu-id="3e11a-136">Logg på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="3e11a-136">Sign into [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="3e11a-137">Velg **alle tjenester** og skriv inn *Azure informasjonsbeskyttelse* i **søkeboksen**.</span><span class="sxs-lookup"><span data-stu-id="3e11a-137">Select **All services** and type in *Azure Information Protection* in the **Search Box**.</span></span>

3. <span data-ttu-id="3e11a-138">Når resultatene vises, klikker du på Start ved siden av **Azure Information Protection** for å gjøre det til en favoritt og lett å finne senere.</span><span class="sxs-lookup"><span data-stu-id="3e11a-138">Once the results display, click the start next to **Azure Information Protection** to make it a favorite and easy to find later.</span></span>

4. <span data-ttu-id="3e11a-139">Velg aktivering av **Azure informasjonsbeskyttelse** \> **beskyttelse** og kontroller at statusen er satt til aktivert.</span><span class="sxs-lookup"><span data-stu-id="3e11a-139">Select **Azure Information Protection** \> **Protection activation** and make sure the status is set to activated.</span></span> 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a><span data-ttu-id="3e11a-140">Vise policyen for Azure informasjonsbeskyttelse og standard etiketter</span><span class="sxs-lookup"><span data-stu-id="3e11a-140">View the Azure Information Protection policy and default labels</span></span> 

<span data-ttu-id="3e11a-141">Hvis du vil vise, og endre, de eksisterende etikettene:</span><span class="sxs-lookup"><span data-stu-id="3e11a-141">To view, and modify, the existing labels:</span></span>

1. <span data-ttu-id="3e11a-142">Velg **klassifiserings** \> **etiketter**på instrumentbordet for Azure informasjonsbeskyttelse.</span><span class="sxs-lookup"><span data-stu-id="3e11a-142">On the Azure Information Protection dashboard, select **Classifications** \> **Labels**.</span></span> <br/><span data-ttu-id="3e11a-143">![Standard etiketter for Azure Information Protection.](media/AIPLabels.png)</span><span class="sxs-lookup"><span data-stu-id="3e11a-143">![Standard labels for Azure Information Protection.](media/AIPLabels.png)</span></span>

2. <span data-ttu-id="3e11a-144">Du kan velge hvilken som helst etikett for å vise alternativer, du kan endre visningsnavnet, farger, etc.</span><span class="sxs-lookup"><span data-stu-id="3e11a-144">You can choose any label to view options, you can change the display name, colors, etc.</span></span>
 
3. <span data-ttu-id="3e11a-145">Se [endre og opprette nye etiketter](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) hvis du vil lage dine egne.</span><span class="sxs-lookup"><span data-stu-id="3e11a-145">See  [Modify and create new labels](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) if you want to create your own.</span></span> 

### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="3e11a-146">Installere Azure Information Protection-klienten manuelt</span><span class="sxs-lookup"><span data-stu-id="3e11a-146">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="3e11a-147">Slik installerer du den AIP-klienten manuelt:</span><span class="sxs-lookup"><span data-stu-id="3e11a-147">To manually install the AIP client:</span></span>

1. <span data-ttu-id="3e11a-148">Dataoverføre **AzInfoProtection. exe** fra [Microsoft Dataoverføre Senter](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="3e11a-148">Download **AzInfoProtection.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="3e11a-149">Du kan kontrollere at installasjonen fungerte ved å vise et Word-dokument og sørge for at alternativet **Beskytt** er tilgjengelig i kategorien **hjem** .</span><span class="sxs-lookup"><span data-stu-id="3e11a-149">You can verify that the installation worked by viewing a Word document and making sure that the **Protect** option is available on the **Home** tab.</span></span> <br/><span data-ttu-id="3e11a-150">![Kategorien beskyttelse i et Word-dokument.](media/Word_Protect.png)</span><span class="sxs-lookup"><span data-stu-id="3e11a-150">![Protection tab drop-down in a Word document.](media/Word_Protect.png)</span></span>

<span data-ttu-id="3e11a-151">Hvis du vil ha mer informasjon, kan [du se installere klienten](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="3e11a-151">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
