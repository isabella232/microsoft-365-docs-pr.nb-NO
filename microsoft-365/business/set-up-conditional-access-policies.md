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
search.appverid:
- BCS160
- MET150
- MOE150
description: Lær hvordan du konfigurerer policyer for betinget tilgang for Microsoft 365-kampanjer.
ms.openlocfilehash: 614e3a6e13a14114f40ecf87bf936d4165744503
ms.sourcegitcommit: 91ff1d4339f0f043c2b43997d87d84677c79e279
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2019
ms.locfileid: "36982385"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="18025-103">Definere policyer for betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="18025-103">Set up conditional access policies</span></span>

<span data-ttu-id="18025-104">Policyer for [betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) legger til substancial ekstra sikkerhet.</span><span class="sxs-lookup"><span data-stu-id="18025-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substancial additional security.</span></span> <span data-ttu-id="18025-105">Microsoft tilbyr et sett med policyer for betinget tilgang som er anbefalt for alle kunder.</span><span class="sxs-lookup"><span data-stu-id="18025-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="18025-106">Policyer for grunnlinje er et sett med forhåndsdefinerte policyer som bidrar til å beskytte organisasjoner mot mange vanlige angrep.</span><span class="sxs-lookup"><span data-stu-id="18025-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="18025-107">Disse vanlige angrepene kan inkludere passord spray, Replay og phishing.</span><span class="sxs-lookup"><span data-stu-id="18025-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="18025-108">Disse policyene krever at administratorer og brukere angir en annen form for godkjenning (kalt multifaktor-godkjenning eller MFA) når visse betingelser er oppfylt.</span><span class="sxs-lookup"><span data-stu-id="18025-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="18025-109">Hvis en bruker for eksempel logger på fra et annet land, kan påloggingen betraktes som risikabelt, og brukeren må angi en ekstra form for godkjenning.</span><span class="sxs-lookup"><span data-stu-id="18025-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="18025-110">Policyer for opprinnelig plan inkluderer følgende:</span><span class="sxs-lookup"><span data-stu-id="18025-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="18025-111">**KREV MFA for administratorer** – krever multifaktorautentisering for de mest privilegerte administratorrollene, inkludert global administrator.</span><span class="sxs-lookup"><span data-stu-id="18025-111">**Require MFA for admins** — Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="18025-112">**Sluttbruker beskyttelse** — krever godkjenning med flere faktorer bare for brukere når en pålogging er risikabelt.</span><span class="sxs-lookup"><span data-stu-id="18025-112">**End user protection** — Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="18025-113">**Blokker eldre autentisering** – eldre klientprogrammer og noen nye apper bruker ikke nyere, sikrere godkjenningsprotokoller.</span><span class="sxs-lookup"><span data-stu-id="18025-113">**Block legacy authentication** — Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="18025-114">Disse eldre appene kan omgå policyer for betinget tilgang og få uautorisert tilgang til miljøet ditt.</span><span class="sxs-lookup"><span data-stu-id="18025-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="18025-115">Denne policyen blokkerer tilgang fra klienter som ikke støtter betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="18025-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="18025-116">**KREV MFA for Service Management** – krever godkjenning med flere faktorer for tilgang til administrasjonsverktøy, inkludert Azure Portal (der du konfigurerer policyer for opprinnelig plan).</span><span class="sxs-lookup"><span data-stu-id="18025-116">**Require MFA for Service Management** — Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="18025-117">Microsoft anbefaler at du aktiverer alle disse grunnlinje policyene.</span><span class="sxs-lookup"><span data-stu-id="18025-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="18025-118">Når disse policyene er aktivert, blir administratorer og brukere bedt om å registrere seg for Azure Multii-Factor-godkjenning.</span><span class="sxs-lookup"><span data-stu-id="18025-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="18025-119">Hvis du vil ha mer informasjon om disse policyene, kan du se [Hva er policyer for opprinnelig plan](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span><span class="sxs-lookup"><span data-stu-id="18025-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="18025-120">Definere policyer for opprinnelig plan</span><span class="sxs-lookup"><span data-stu-id="18025-120">Set up baseline policies</span></span>

1. <span data-ttu-id="18025-121">Gå til [Azure Portal](https://portal.azure.com), og naviger deretter til **Azure Active Directory** \> - **betinget tilgang**.</span><span class="sxs-lookup"><span data-stu-id="18025-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="18025-122">De opprinnelige policyene er oppført på siden.</span><span class="sxs-lookup"><span data-stu-id="18025-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="18025-123">![Side som viser en liste over opprinnelige policyer for betinget tilgang.](media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="18025-123">![Page that lists baseline policies for conditional access.](media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="18025-124">Se følgende spesifikke instruksjoner for hver policy:</span><span class="sxs-lookup"><span data-stu-id="18025-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="18025-125">Krev MFA for administratorer</span><span class="sxs-lookup"><span data-stu-id="18025-125">Require MFA for admins</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="18025-126">Krev MFA for brukere</span><span class="sxs-lookup"><span data-stu-id="18025-126">Require MFA for users</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="18025-127">Blokker eldre godkjenning</span><span class="sxs-lookup"><span data-stu-id="18025-127">Block legacy authentication</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="18025-128">Krev MFA for servicestyring</span><span class="sxs-lookup"><span data-stu-id="18025-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="18025-129">Du kan definere mange tilleggs policyer, for eksempel å kreve godkjente klientprogrammer.</span><span class="sxs-lookup"><span data-stu-id="18025-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="18025-130">Se [dokumentasjonen for betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="18025-130">See the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/) for more information.</span></span>