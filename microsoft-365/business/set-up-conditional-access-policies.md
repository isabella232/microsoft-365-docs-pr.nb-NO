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
ms.openlocfilehash: 3772aa0d505ef54a0587423e890ede519d571e0c
ms.sourcegitcommit: 70e920f76526f47fc849df615de4569e0ac2f4be
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/07/2019
ms.locfileid: "38031399"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="54ff8-103">Definere policyer for betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="54ff8-103">Set up conditional access policies</span></span>

<span data-ttu-id="54ff8-104">Policyer for [betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) legger til substancial ekstra sikkerhet.</span><span class="sxs-lookup"><span data-stu-id="54ff8-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="54ff8-105">Microsoft tilbyr et sett med policyer for betinget tilgang som er anbefalt for alle kunder.</span><span class="sxs-lookup"><span data-stu-id="54ff8-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="54ff8-106">Policyer for grunnlinje er et sett med forhåndsdefinerte policyer som bidrar til å beskytte organisasjoner mot mange vanlige angrep.</span><span class="sxs-lookup"><span data-stu-id="54ff8-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="54ff8-107">Disse vanlige angrepene kan inkludere passord spray, Replay og phishing.</span><span class="sxs-lookup"><span data-stu-id="54ff8-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="54ff8-108">Disse policyene krever at administratorer og brukere angir en annen form for godkjenning (kalt multifaktor-godkjenning eller MFA) når visse betingelser er oppfylt.</span><span class="sxs-lookup"><span data-stu-id="54ff8-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="54ff8-109">Hvis en bruker for eksempel logger på fra et annet land, kan påloggingen betraktes som risikabelt, og brukeren må angi en ekstra form for godkjenning.</span><span class="sxs-lookup"><span data-stu-id="54ff8-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="54ff8-110">Policyer for opprinnelig plan inkluderer følgende:</span><span class="sxs-lookup"><span data-stu-id="54ff8-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="54ff8-111">**KREV MFA for administratorer** – krever multifaktorautentisering for de mest privilegerte administratorrollene, inkludert global administrator.</span><span class="sxs-lookup"><span data-stu-id="54ff8-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="54ff8-112">**Sluttbruker beskyttelse** — krever godkjenning med flere faktorer bare for brukere når en pålogging er risikabelt.</span><span class="sxs-lookup"><span data-stu-id="54ff8-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="54ff8-113">**Blokker eldre autentisering** – eldre klientprogrammer og noen nye apper bruker ikke nyere, sikrere godkjenningsprotokoller.</span><span class="sxs-lookup"><span data-stu-id="54ff8-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="54ff8-114">Disse eldre appene kan omgå policyer for betinget tilgang og få uautorisert tilgang til miljøet ditt.</span><span class="sxs-lookup"><span data-stu-id="54ff8-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="54ff8-115">Denne policyen blokkerer tilgang fra klienter som ikke støtter betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="54ff8-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="54ff8-116">**KREV MFA for Service Management** – krever godkjenning med flere faktorer for tilgang til administrasjonsverktøy, inkludert Azure Portal (der du konfigurerer policyer for opprinnelig plan).</span><span class="sxs-lookup"><span data-stu-id="54ff8-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="54ff8-117">Microsoft anbefaler at du aktiverer alle disse grunnlinje policyene.</span><span class="sxs-lookup"><span data-stu-id="54ff8-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="54ff8-118">Når disse policyene er aktivert, blir administratorer og brukere bedt om å registrere seg for Azure Multii-Factor-godkjenning.</span><span class="sxs-lookup"><span data-stu-id="54ff8-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="54ff8-119">Hvis du vil ha mer informasjon om disse policyene, kan du se [Hva er policyer for opprinnelig plan](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="54ff8-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="54ff8-120">Definere policyer for opprinnelig plan</span><span class="sxs-lookup"><span data-stu-id="54ff8-120">Set up baseline policies</span></span>

1. <span data-ttu-id="54ff8-121">Gå til [Azure Portal](https://portal.azure.com), og naviger deretter til **Azure Active Directory** \> - **betinget tilgang**.</span><span class="sxs-lookup"><span data-stu-id="54ff8-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="54ff8-122">De opprinnelige policyene er oppført på siden.</span><span class="sxs-lookup"><span data-stu-id="54ff8-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="54ff8-123">![Side som viser en liste over opprinnelige policyer for betinget tilgang.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="54ff8-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="54ff8-124">Se følgende spesifikke instruksjoner for hver policy:</span><span class="sxs-lookup"><span data-stu-id="54ff8-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="54ff8-125">Krev MFA for administratorer</span><span class="sxs-lookup"><span data-stu-id="54ff8-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="54ff8-126">Krev MFA for brukere</span><span class="sxs-lookup"><span data-stu-id="54ff8-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="54ff8-127">Blokker eldre godkjenning</span><span class="sxs-lookup"><span data-stu-id="54ff8-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="54ff8-128">Krev MFA for servicestyring</span><span class="sxs-lookup"><span data-stu-id="54ff8-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="54ff8-129">Du kan definere mange tilleggs policyer, for eksempel å kreve godkjente klientprogrammer.</span><span class="sxs-lookup"><span data-stu-id="54ff8-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="54ff8-130">Se [dokumentasjonen for betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="54ff8-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>