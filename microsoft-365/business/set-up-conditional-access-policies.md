---
title: Definer policyer for betinget tilgang for Microsoft 365-kampanjer
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
description: Lær hvordan du konfigurerer policyer for betinget tilgang for Microsoft 365-kampanjer.
ms.openlocfilehash: aebdb733c2dd9a05947335ad4f151104d801568e
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718833"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="07ff1-103">Definere policyer for betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="07ff1-103">Set up conditional access policies</span></span>

<span data-ttu-id="07ff1-104">Policyer for [betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) legger til betydelig ekstra sikkerhet.</span><span class="sxs-lookup"><span data-stu-id="07ff1-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="07ff1-105">Microsoft tilbyr et sett med policyer for betinget tilgang som er anbefalt for alle kunder.</span><span class="sxs-lookup"><span data-stu-id="07ff1-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="07ff1-106">Policyer for grunnlinje er et sett med forhåndsdefinerte policyer som bidrar til å beskytte organisasjoner mot mange vanlige angrep.</span><span class="sxs-lookup"><span data-stu-id="07ff1-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="07ff1-107">Disse vanlige angrepene kan inkludere passord spray, Replay og phishing.</span><span class="sxs-lookup"><span data-stu-id="07ff1-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="07ff1-108">Disse policyene krever at administratorer og brukere angir en annen form for godkjenning (kalt multifaktor-godkjenning eller MFA) når visse betingelser er oppfylt.</span><span class="sxs-lookup"><span data-stu-id="07ff1-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="07ff1-109">Hvis en bruker for eksempel logger på fra et annet land, kan påloggingen betraktes som risikabelt, og brukeren må angi en ekstra form for godkjenning.</span><span class="sxs-lookup"><span data-stu-id="07ff1-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="07ff1-110">Policyer for opprinnelig plan inkluderer følgende:</span><span class="sxs-lookup"><span data-stu-id="07ff1-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="07ff1-111">**Krev MFA for administratorer** &ndash; krever godkjenning med flere faktorer for de mest privilegerte administratorrollene, inkludert global administrator.</span><span class="sxs-lookup"><span data-stu-id="07ff1-111">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="07ff1-112">**Sluttbruker beskyttelse** &ndash; krever multifaktorautentisering bare for brukere når en pålogging er risikabelt.</span><span class="sxs-lookup"><span data-stu-id="07ff1-112">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="07ff1-113">**Blokker** &ndash; eldre klientprogrammer og noen nye apper bruker ikke nyere, sikrere godkjenningsprotokoller.</span><span class="sxs-lookup"><span data-stu-id="07ff1-113">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="07ff1-114">Disse eldre appene kan omgå policyer for betinget tilgang og få uautorisert tilgang til miljøet ditt.</span><span class="sxs-lookup"><span data-stu-id="07ff1-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="07ff1-115">Denne policyen blokkerer tilgang fra klienter som ikke støtter betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="07ff1-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="07ff1-116">**Krev MFA for Service Management** &ndash; krever multifaktorautentisering for tilgang til administrasjonsverktøy, inkludert Azure Portal (der du konfigurerer policyer for opprinnelig plan).</span><span class="sxs-lookup"><span data-stu-id="07ff1-116">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="07ff1-117">Microsoft anbefaler at du aktiverer alle disse grunnlinje policyene.</span><span class="sxs-lookup"><span data-stu-id="07ff1-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="07ff1-118">Når disse policyene er aktivert, blir administratorer og brukere bedt om å registrere seg for Azure Multii-Factor-godkjenning.</span><span class="sxs-lookup"><span data-stu-id="07ff1-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="07ff1-119">Hvis du vil ha mer informasjon om disse policyene, kan du se [Hva er policyer for opprinnelig plan](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="07ff1-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="07ff1-120">Definere policyer for opprinnelig plan</span><span class="sxs-lookup"><span data-stu-id="07ff1-120">Set up baseline policies</span></span>

1. <span data-ttu-id="07ff1-121">Gå til [Azure Portal](https://portal.azure.com), og naviger deretter til **Azure Active Directory** \> - **betinget tilgang**.</span><span class="sxs-lookup"><span data-stu-id="07ff1-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="07ff1-122">De opprinnelige policyene er oppført på siden.</span><span class="sxs-lookup"><span data-stu-id="07ff1-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="07ff1-123">![Side som viser en liste over opprinnelige policyer for betinget tilgang.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="07ff1-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="07ff1-124">Se følgende spesifikke instruksjoner for hver policy:</span><span class="sxs-lookup"><span data-stu-id="07ff1-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="07ff1-125">Krev MFA for administratorer</span><span class="sxs-lookup"><span data-stu-id="07ff1-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="07ff1-126">Krev MFA for brukere</span><span class="sxs-lookup"><span data-stu-id="07ff1-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="07ff1-127">Blokker eldre godkjenning</span><span class="sxs-lookup"><span data-stu-id="07ff1-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="07ff1-128">Krev MFA for servicestyring</span><span class="sxs-lookup"><span data-stu-id="07ff1-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="07ff1-129">Du kan definere mange tilleggs policyer, for eksempel å kreve godkjente klientprogrammer.</span><span class="sxs-lookup"><span data-stu-id="07ff1-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="07ff1-130">Hvis du vil ha mer informasjon, se [dokumentasjonen for betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="07ff1-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
