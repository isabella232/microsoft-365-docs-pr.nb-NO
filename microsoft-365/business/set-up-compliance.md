---
title: Øke trusselen beskyttelse for Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
description: Angi Office 365 Avansert trussel beskyttelse, og beskytte sensitive data.
ms.openlocfilehash: 53741a7726222bb32329a401953be72257df95cc
ms.sourcegitcommit: 7ac06563c6ff034358e8fd3f9298fc426187ade2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/31/2019
ms.locfileid: "35086356"
---
# <a name="set-up-compliance-features"></a><span data-ttu-id="8de5e-103">Sett opp funksjoner for kompatibilitet</span><span class="sxs-lookup"><span data-stu-id="8de5e-103">Set up compliance features</span></span>

<span data-ttu-id="8de5e-104">Bedriften din Microsoft-365 leveres med funksjoner for å beskytte dine data og enheter og beskytte din egen og kundenes sensitiv informasjon.</span><span class="sxs-lookup"><span data-stu-id="8de5e-104">Your Microsoft 365 Business comes with features to protect your data and devices, and help you keep yours and your customers' sensitive information secure.</span></span>

## <a name="set-up-dlp-features"></a><span data-ttu-id="8de5e-105">Konfigurer DLP-funksjoner</span><span class="sxs-lookup"><span data-stu-id="8de5e-105">Set up DLP features</span></span>

<span data-ttu-id="8de5e-106">Se [opprette en DLP policy fra en mal](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for et eksempel på hvordan du konfigurerer en policy for beskyttelse mot personlig identifiserbar informasjon (PII).</span><span class="sxs-lookup"><span data-stu-id="8de5e-106">See [Create a DLP policy from a template](https://support.office.com/article/59414438-99f5-488b-975c-5023f2254369) for an example on how to set up a policy to protect against personally identifiable information (PII).</span></span> 
  
<span data-ttu-id="8de5e-107">DLP leveres med mange klare til bruk policymaler for mange forskjellige nasjonale innstillinger.</span><span class="sxs-lookup"><span data-stu-id="8de5e-107">DLP comes with many ready-to-use policy templates for many different locales.</span></span> <span data-ttu-id="8de5e-108">For eksempel økonomiske Data for Australia, Canada personlig informasjon Act, amerikanske økonomiske Data, osv. Se [Hva the DLP maler for gruppepolicy inneholder](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) en fullstendig liste.</span><span class="sxs-lookup"><span data-stu-id="8de5e-108">For example, Australia Financial Data, Canada Personal Information Act, U.S. Financial Data, etc. See [What the DLP policy templates include](https://support.office.com/article/c2e588d3-8f4f-4937-a286-8c399f28953a) for a full list.</span></span> <span data-ttu-id="8de5e-109">Alle disse malene kan aktiveres ligner eksemplet PII mal.</span><span class="sxs-lookup"><span data-stu-id="8de5e-109">All of these templates can be enabled similar to the PII template example.</span></span> 
  
## <a name="set-up-email-retention-with-exchange-online-archiving"></a><span data-ttu-id="8de5e-110">Definer tilbakeholdelse av e-post med Exchange Online-arkivering</span><span class="sxs-lookup"><span data-stu-id="8de5e-110">Set up email retention with Exchange Online Archiving</span></span>

 <span data-ttu-id="8de5e-111">**Exchange Online-arkivering** lisens funksjoner hjelper opprettholde overensstemmelse og forskriftsmessige standarder ved å beholde e-post innhold for eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="8de5e-111">**Exchange Online Archiving** license features help maintain compliance and regulatory standards by preserving email content for eDiscovery.</span></span> <span data-ttu-id="8de5e-112">I tillegg bidrar til å redusere risiko i tilfelle en lawsuit og gjør det mulig å gjenopprette data etter brudd på sikkerheten, eller når du skal gjenopprette slettede elementer.</span><span class="sxs-lookup"><span data-stu-id="8de5e-112">It also helps reduce your risk in the event of a lawsuit and provides a way to recover data after a security breach, or when you need to recover deleted items.</span></span> <span data-ttu-id="8de5e-113">Du kan bruke rettstvist hold for å beholde alt innholdet i en brukers eller bruke oppbevaringspolicyer til å tilpasse hva du vil beholde.</span><span class="sxs-lookup"><span data-stu-id="8de5e-113">You can use litigation hold to preserve all of a user's content, or use retention policies to customize what you want to preserve.</span></span>
  
<span data-ttu-id="8de5e-114">**Rettstvist sperring:** Du kan beholde alle postboksinnholdet inkludert Slettede elementer ved å plassere hele postboksen for en bruker i rettstvist holder.</span><span class="sxs-lookup"><span data-stu-id="8de5e-114">**Litigation hold:** You can preserve all mailbox content including deleted items by putting a user's entire mailbox on litigation hold.</span></span> 
    
<span data-ttu-id="8de5e-115">Hvis du vil plassere en postboks på rettstvist hold, i administrasjonssenteret:</span><span class="sxs-lookup"><span data-stu-id="8de5e-115">To place a mailbox on litigation hold, in the Admin center:</span></span>
    
1. <span data-ttu-id="8de5e-116">Gå til **brukere** i den venstre nav, \> **aktive brukere**.</span><span class="sxs-lookup"><span data-stu-id="8de5e-116">In the left nav, go to **Users** \> **Active users**.</span></span>
    
2. <span data-ttu-id="8de5e-117">Velg en bruker som har postboksen du vil plassere på rettstvist holder og Utvid **e-postinnstillinger** i ruten til brukeren og ved siden av **flere innstillinger** velger du **Rediger Exchange egenskaper**.</span><span class="sxs-lookup"><span data-stu-id="8de5e-117">Select a user whose mailbox you want to place on litigation hold and in the user pane expand **Mail settings** and next to **More settings** choose **Edit Exchange properties**.</span></span>
    
3. <span data-ttu-id="8de5e-118">På postboks-siden for brukeren å velge \*\* postboks funksjoner \*\* på venstre nav, og velg deretter **Aktiver** koblingen under **rettstvist holder**.</span><span class="sxs-lookup"><span data-stu-id="8de5e-118">On the mailbox page for the user, choose \*\* mailbox features \*\* on the left nav, and then choose the **Enable** link under **Litigation hold**.</span></span>
    
4. <span data-ttu-id="8de5e-119">**Rettstvist holder** dialogboksen kan du angi rettstvisten Hold nede-varighet i **rettstvist Hold nede-varighet** -feltet, la feltet stå tomt hvis du vil plassere en uendelig sperring.</span><span class="sxs-lookup"><span data-stu-id="8de5e-119">In the **litigation hold** dialog box you can specify the litigation hold duration in the **Litigation hold duration** field, leave field empty if you want to place an infinite hold.</span></span> <span data-ttu-id="8de5e-120">Du kan også legge til merknader og direkte eieren av e-post-boksen til et webområde, må du kanskje forklare mer om rettstvisten holder \> **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="8de5e-120">You can also add notes and direct the mail box owner to a website you might have to explain more about the litigation hold \> **Save**.</span></span>
    
<span data-ttu-id="8de5e-121">**Oppbevaring:** Du kan aktivere tilpassede policyer for dokumentoppbevaring, for eksempel å bevare i en bestemt tidsperiode eller slette innholdet permanent på slutten av Oppbevaringstiden.</span><span class="sxs-lookup"><span data-stu-id="8de5e-121">**Retention:** You can enable customized retention policies, for example, to preserve for a specific amount of time or delete content permanently at the end of the retention period.</span></span> <span data-ttu-id="8de5e-122">Hvis du vil ha mer informasjon, se [Oversikt over policyer for dokumentoppbevaring](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span><span class="sxs-lookup"><span data-stu-id="8de5e-122">To learn more, see [Overview of retention policies](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).</span></span>

## <a name="set-up-azure-information-protection-features"></a><span data-ttu-id="8de5e-123">Sett opp funksjoner for beskyttelse mot Azure-informasjon</span><span class="sxs-lookup"><span data-stu-id="8de5e-123">Set up Azure Information Protection features</span></span>

<span data-ttu-id="8de5e-124">Azure informasjon beskyttelse (AIP) hjelper deg med å klassifisere, og du kan også beskytte dokumenter og e-post, ved å bruke etiketter.</span><span class="sxs-lookup"><span data-stu-id="8de5e-124">Azure Information Protection (AIP) helps you classify and optionally, protect your documents and emails, by applying labels.</span></span> <span data-ttu-id="8de5e-125">Etiketter kan brukes automatisk som administratorer definerer regler og betingelser, manuelt av brukere eller ved å bruke en kombinasjon, der brukere får anbefalinger.</span><span class="sxs-lookup"><span data-stu-id="8de5e-125">Labels can be applied automatically by administrators who define rules and conditions, manually by users, or by using a combination where users are given recommendations.</span></span>

<span data-ttu-id="8de5e-126">Du kan bruke følgende innebygde etiketter og begrensninger på e-poster i Outlook på weben:</span><span class="sxs-lookup"><span data-stu-id="8de5e-126">In Outlook on the web you can apply the following built-in labels and restrictions to your emails:</span></span>
  
- <span data-ttu-id="8de5e-127">**Ikke Videresend**: kan mottakere lese meldingen, men de kan ikke videresende, skrive ut eller kopiere innhold</span><span class="sxs-lookup"><span data-stu-id="8de5e-127">**Do Not Forward**: Recipients can read the message, but they can't forward, print, or copy content</span></span>
    
- <span data-ttu-id="8de5e-128">**Kryptere**: hele meldingen er kryptert.</span><span class="sxs-lookup"><span data-stu-id="8de5e-128">**Encrypt**: The entire message is encrypted.</span></span> <span data-ttu-id="8de5e-129">Mottakerne må bekrefte sin identitet før du åpner kryptert innhold og kan ikke fjerne kryptering.</span><span class="sxs-lookup"><span data-stu-id="8de5e-129">Recipients must confirm their identity before accessing encrypted content and can't remove encryption.</span></span>
    
- <span data-ttu-id="8de5e-130">**Konfidensielt**: gir ansatte i organisasjonen alle tillatelser til e-post-innhold og vedlegg, men ikke til personer utenfor organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="8de5e-130">**Confidential**: Gives the employees in your organization full permissions to the email content and attachments, but not to people outside your organization.</span></span> <span data-ttu-id="8de5e-131">Dataeiere kan spore og oppheve innhold når som helst.</span><span class="sxs-lookup"><span data-stu-id="8de5e-131">Data owners can track and revoke content at any point.</span></span>
    
- <span data-ttu-id="8de5e-132">**Høyst konfidensiell**: Denne restriksjonen kan brukes på svært konfidensielle data, slik at ansatte kan vise, redigere, og svar, men ikke videresende, skrive ut eller kopiere data.</span><span class="sxs-lookup"><span data-stu-id="8de5e-132">**Highly Confidential**: This restriction can be applied to highly confidential data, allowing employees to view, edit, and reply, but not forward, print, or copy the data.</span></span> <span data-ttu-id="8de5e-133">Dataeiere kan spore og oppheve innhold når som helst.</span><span class="sxs-lookup"><span data-stu-id="8de5e-133">Data owners can track and revoke content at any point.</span></span>

### <a name="make-sure-azure-information-protection-is-activated"></a><span data-ttu-id="8de5e-134">Kontroller at Azure informasjonsbeskyttelse er aktivert</span><span class="sxs-lookup"><span data-stu-id="8de5e-134">Make sure Azure Information Protection is activated</span></span>

<span data-ttu-id="8de5e-135">Slik kontrollerer du at AIP er aktivert:</span><span class="sxs-lookup"><span data-stu-id="8de5e-135">To verify that AIP is activated :</span></span>

1. <span data-ttu-id="8de5e-136">Logge på [Azure portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="8de5e-136">Sign into [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="8de5e-137">Velg **alle tjenester** og type i *Azure informasjonsbeskyttelse* i **Søk-boksen**.</span><span class="sxs-lookup"><span data-stu-id="8de5e-137">Select **All services** and type in *Azure Information Protection* in the **Search Box**.</span></span>

3. <span data-ttu-id="8de5e-138">Når resultatet vises, klikker du start neste **Azure informasjonsbeskyttelse** for å gjøre den til favoritt og lett å finne senere.</span><span class="sxs-lookup"><span data-stu-id="8de5e-138">Once the results display, click the start next to **Azure Information Protection** to make it a favorite and easy to find later.</span></span>

4. <span data-ttu-id="8de5e-139">Velg **Azure informasjonsbeskyttelse** \> **Beskyttelse aktivering** , og kontroller at statusen er satt til aktivert.</span><span class="sxs-lookup"><span data-stu-id="8de5e-139">Select **Azure Information Protection** \> **Protection activation** and make sure the status is set to activated.</span></span> 

### <a name="view-the-azure-information-protection-policy-and-default-labels"></a><span data-ttu-id="8de5e-140">Vise informasjon om beskyttelse av Azure policy og standard etikettene</span><span class="sxs-lookup"><span data-stu-id="8de5e-140">View the Azure Information Protection policy and default labels</span></span> 

<span data-ttu-id="8de5e-141">Hvis du vil vise og endre, eksisterende etiketter:</span><span class="sxs-lookup"><span data-stu-id="8de5e-141">To view, and modify, the existing labels:</span></span>

1. <span data-ttu-id="8de5e-142">Velg **klassifiseringer** på instrumentbordet Azure informasjonsbeskyttelse \> **etiketter**.</span><span class="sxs-lookup"><span data-stu-id="8de5e-142">On the Azure Information Protection dashboard, select **Classifications** \> **Labels**.</span></span> <br/><span data-ttu-id="8de5e-143">![Standard etiketter for Azure informasjonsbeskyttelse.](media/AIPLabels.png)</span><span class="sxs-lookup"><span data-stu-id="8de5e-143">![Standard labels for Azure Information Protection.](media/AIPLabels.png)</span></span>

2. <span data-ttu-id="8de5e-144">Du kan velge en etikett til å vise alternativene, kan du endre visningsnavnet, farger og så videre.</span><span class="sxs-lookup"><span data-stu-id="8de5e-144">You can choose any label to view options, you can change the display name, colors, etc.</span></span>
 
3. <span data-ttu-id="8de5e-145">Se [endre og opprette nye etiketter](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) Hvis du vil opprette dine egne.</span><span class="sxs-lookup"><span data-stu-id="8de5e-145">See  [Modify and create new labels](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step2) if you want to create your own.</span></span> 

### <a name="install-the-azure-information-protection-client-manually"></a><span data-ttu-id="8de5e-146">Installere klienten Azure informasjonsbeskyttelse manuelt</span><span class="sxs-lookup"><span data-stu-id="8de5e-146">Install the Azure Information Protection client manually</span></span>

<span data-ttu-id="8de5e-147">Å manuelt installere AIP-klient:</span><span class="sxs-lookup"><span data-stu-id="8de5e-147">To manually install the AIP client:</span></span>

1. <span data-ttu-id="8de5e-148">Last ned **AzInfoProtection.exe** fra [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span><span class="sxs-lookup"><span data-stu-id="8de5e-148">Download **AzInfoProtection.exe** from [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=53018).</span></span>
 
2. <span data-ttu-id="8de5e-149">Du kan kontrollere at installasjonen arbeidet ved å vise et Word-dokument og kontrollere at alternativet **Beskytt** er tilgjengelige i kategorien **Hjem** .</span><span class="sxs-lookup"><span data-stu-id="8de5e-149">You can verify that the installation worked by viewing a Word document and making sure that the **Protect** option is available on the **Home** tab.</span></span> <br/><span data-ttu-id="8de5e-150">![Kategorien beskyttelse rullegardinlisten i et Word-dokument.](media/Word_Protect.png)</span><span class="sxs-lookup"><span data-stu-id="8de5e-150">![Protection tab drop-down in a Word document.](media/Word_Protect.png)</span></span>

<span data-ttu-id="8de5e-151">For mer informasjon, se [installere klienten](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span><span class="sxs-lookup"><span data-stu-id="8de5e-151">For more information see, [Install the client](https://docs.microsoft.com/azure/information-protection/infoprotect-tutorial-step3).</span></span>
