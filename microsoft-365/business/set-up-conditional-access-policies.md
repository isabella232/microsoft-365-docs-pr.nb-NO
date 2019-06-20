---
title: Definer policyer for betinget tilgang for Microsoft 365 kampanjer
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
search.appverid:
- BCS160
- MET150
- MOE150
description: Lær hvordan du setter opp betinget tilgang policyer for Microsoft 365 kampanjer.
ms.openlocfilehash: 7d8e1f16019d151478aae57b1593b0e0758e5b19
ms.sourcegitcommit: 7e46db0b35c188ee6a7b40ab3eb2d76ff6c101c5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/19/2019
ms.locfileid: "35086363"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="cc07a-103">Definer policyer for betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="cc07a-103">Set up conditional access policies</span></span>

<span data-ttu-id="cc07a-104">[Betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policyer legger substancial ekstra sikkerhet.</span><span class="sxs-lookup"><span data-stu-id="cc07a-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="cc07a-105">Microsoft tilbyr et sett med planlagte betinget tilgang policyer som er anbefalt for alle kunder.</span><span class="sxs-lookup"><span data-stu-id="cc07a-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="cc07a-106">Policyer for opprinnelig plan er et sett med forhåndsdefinerte policyer som beskytter organisasjoner mot mange vanlige angrep.</span><span class="sxs-lookup"><span data-stu-id="cc07a-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="cc07a-107">Disse vanlige angrep kan inkludere passord Sprederen, replay og phishing.</span><span class="sxs-lookup"><span data-stu-id="cc07a-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="cc07a-108">Disse policyene krever at administratorer og brukere til å angi en annen form for godkjenning (kalt multifaktorautentisering eller MFA) når visse betingelser er oppfylt.</span><span class="sxs-lookup"><span data-stu-id="cc07a-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="cc07a-109">For eksempel hvis en bruker er logger på fra et annet land, pålogging kan vurderes som risikabelt, og brukeren må angi en mer form for godkjenning.</span><span class="sxs-lookup"><span data-stu-id="cc07a-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="cc07a-110">For øyeblikket omfatter planlagt policyene følgende:</span><span class="sxs-lookup"><span data-stu-id="cc07a-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="cc07a-111">**Krever MFA for administratorer** , krever multifaktorautentisering for de mest privilegerte administrator-rollene, inkludert global administrator.</span><span class="sxs-lookup"><span data-stu-id="cc07a-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="cc07a-112">**Sluttbrukeren beskyttelse** , krever multifaktorautentisering for brukere bare når en pålogging er risikabelt.</span><span class="sxs-lookup"><span data-stu-id="cc07a-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="cc07a-113">**Eldre blokk-godkjenning** – eldre klientprogrammer og noen nye apps ikke bruke godkjenningsprotokoller som er nyere, sikrere.</span><span class="sxs-lookup"><span data-stu-id="cc07a-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="cc07a-114">Disse eldre programmer kan hoppe over policyer for betinget tilgang og få uautorisert tilgang til ditt miljø.</span><span class="sxs-lookup"><span data-stu-id="cc07a-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="cc07a-115">Denne policyen blokkerer tilgang fra klienter som ikke støtter betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="cc07a-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="cc07a-116">**Krever MFA for servicestyring** – krever multifaktorautentisering for tilgang til verktøy for systemadministrasjon, inkludert Azure portal (hvor du konfigurere policyer for opprinnelig plan).</span><span class="sxs-lookup"><span data-stu-id="cc07a-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="cc07a-117">Microsoft anbefaler at du aktiverer alle disse policyene for opprinnelig plan.</span><span class="sxs-lookup"><span data-stu-id="cc07a-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="cc07a-118">Når disse policyene er aktivert, administratorer og brukere vil bli bedt om å registrere deg for Azure Multii-faktors autentifiseringsprosess.</span><span class="sxs-lookup"><span data-stu-id="cc07a-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="cc07a-119">Hvis du vil ha mer informasjon om disse policyene, kan du se [Hva er planlagt policyer](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="cc07a-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="cc07a-120">Definer policyer for opprinnelig plan</span><span class="sxs-lookup"><span data-stu-id="cc07a-120">Set up baseline policies</span></span>

1. <span data-ttu-id="cc07a-121">Gå til [Azure portal](https://portal.azure.com), og naviger deretter til **Azure Active Directory** \> **Betinget tilgang**.</span><span class="sxs-lookup"><span data-stu-id="cc07a-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="cc07a-122">Policyer for opprinnelig plan er oppført på siden.</span><span class="sxs-lookup"><span data-stu-id="cc07a-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="cc07a-123">![Side som viser en liste over planlagte policyer for betinget tilgang.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="cc07a-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="cc07a-124">Se følgende spesifikke instruksjoner for hver policy:</span><span class="sxs-lookup"><span data-stu-id="cc07a-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="cc07a-125">Krev MFA for administratorer</span><span class="sxs-lookup"><span data-stu-id="cc07a-125">Require MFA for admins</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="cc07a-126">Reequire MFA for brukere</span><span class="sxs-lookup"><span data-stu-id="cc07a-126">Reequire MFA for users</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="cc07a-127">Eldre blokk-godkjenning</span><span class="sxs-lookup"><span data-stu-id="cc07a-127">Block legacy authentication</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="cc07a-128">Krev MFA for servicestyring</span><span class="sxs-lookup"><span data-stu-id="cc07a-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="cc07a-129">Du kan definere mange flere policyer, som for eksempel at godkjente klientprogrammer.</span><span class="sxs-lookup"><span data-stu-id="cc07a-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="cc07a-130">Se [Dokumentasjonen for betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="cc07a-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>