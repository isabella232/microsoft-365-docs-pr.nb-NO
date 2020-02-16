---
title: Definere policyer for betinget tilgang for Microsoft 365-kampanjer
f1.keywords:
- NOCSH
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
description: Finn ut hvordan du konfigurerer policyer for betinget tilgang for Microsoft 365-kampanjer.
ms.openlocfilehash: 1ef90bd77da43ded624d85cef9c7a33beec74345
ms.sourcegitcommit: 3dd9944a6070a7f35c4bc2b57df397f844c3fe79
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/15/2020
ms.locfileid: "42064618"
---
# <a name="set-up-conditional-access-policies"></a><span data-ttu-id="8f81d-103">Definere policyer for betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="8f81d-103">Set up conditional access policies</span></span>

<span data-ttu-id="8f81d-104">[Retningslinjer for betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) legger til betydelig ekstra sikkerhet.</span><span class="sxs-lookup"><span data-stu-id="8f81d-104">[Conditional access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policies add substantial additional security.</span></span> <span data-ttu-id="8f81d-105">Microsoft inneholder et sett med betingelseslinjer for betinget tilgang som anbefales for alle kunder.</span><span class="sxs-lookup"><span data-stu-id="8f81d-105">Microsoft provides a set of baseline conditional access policies that are recommended for all customers.</span></span> <span data-ttu-id="8f81d-106">Grunnlinjepolicyer er et sett med forhåndsdefinerte policyer som bidrar til å beskytte organisasjoner mot mange vanlige angrep.</span><span class="sxs-lookup"><span data-stu-id="8f81d-106">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="8f81d-107">Disse vanlige angrepene kan inkludere passordspray, replay og phishing.</span><span class="sxs-lookup"><span data-stu-id="8f81d-107">These common attacks can include password spray, replay, and phishing.</span></span>

<span data-ttu-id="8f81d-108">Disse policyene krever at administratorer og brukere angir en annen form for godkjenning (kalt multifaktorautentisering eller MFA) når visse betingelser er oppfylt.</span><span class="sxs-lookup"><span data-stu-id="8f81d-108">These policies require admins and users to enter a second form of authentication (called multifactor authentication, or MFA) when certain conditions are met.</span></span> <span data-ttu-id="8f81d-109">Hvis en bruker for eksempel logger på fra et annet land, kan påloggingen anses som risikabelt, og brukeren må oppgi en ekstra form for godkjenning.</span><span class="sxs-lookup"><span data-stu-id="8f81d-109">For example, if a user is signing in from a different country, the sign-in might be considered risky and the user must provide an additional form of authentication.</span></span> 

<span data-ttu-id="8f81d-110">For øyeblikket inkluderer opprinnelige policyer følgende:</span><span class="sxs-lookup"><span data-stu-id="8f81d-110">Currently, baseline policies include the following:</span></span>
- <span data-ttu-id="8f81d-111">**Kreve MFA for administratorer** &ndash; Krever godkjenning med flere faktorer for de mest privilegerte administratorrollene, inkludert global administrator.</span><span class="sxs-lookup"><span data-stu-id="8f81d-111">**Require MFA for admins** &ndash; Requires multi-factor authentication for the most privileged administrator roles, including global administrator.</span></span>
- <span data-ttu-id="8f81d-112">**Sluttbrukerbeskyttelse** &ndash; Krever godkjenning med flere faktorer for brukere bare når en pålogging er risikabelt.</span><span class="sxs-lookup"><span data-stu-id="8f81d-112">**End user protection** &ndash; Requires multi-factor authentication for users only when a sign-in is risky.</span></span> 
- <span data-ttu-id="8f81d-113">**Blokker eldre godkjenning** &ndash; Eldre klientapper og noen nye apper bruker ikke nyere, sikrere godkjenningsprotokoller.</span><span class="sxs-lookup"><span data-stu-id="8f81d-113">**Block legacy authentication** &ndash; Older client apps and some new apps don't use newer, more secure, authentication protocols.</span></span> <span data-ttu-id="8f81d-114">Disse eldre appene kan omgå retningslinjer for betinget tilgang og få uautorisert tilgang til miljøet ditt.</span><span class="sxs-lookup"><span data-stu-id="8f81d-114">These older apps can bypass conditional access policies and gain unauthorized access to your environment.</span></span> <span data-ttu-id="8f81d-115">Denne policyen blokkerer tilgang fra klienter som ikke støtter betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="8f81d-115">This policy blocks access from clients that don't support conditional access.</span></span> 
- <span data-ttu-id="8f81d-116">**Krev MFA for servicebehandling** &ndash; Krever godkjenning med flere faktorer for tilgang til administrasjonsverktøy, inkludert Azure-portal (der du konfigurerer opprinnelige policyer).</span><span class="sxs-lookup"><span data-stu-id="8f81d-116">**Require MFA for Service Management** &ndash; Requires multi-factor authentication for access to management tools, including Azure portal (where you configure baseline policies).</span></span> 

<span data-ttu-id="8f81d-117">Microsoft anbefaler at du aktiverer alle disse grunnlinjepolicyene.</span><span class="sxs-lookup"><span data-stu-id="8f81d-117">Microsoft recommends you enable all of these baseline policies.</span></span> <span data-ttu-id="8f81d-118">Når disse policyene er aktivert, blir administratorer og brukere bedt om å registrere seg for Azure Multii-Factor-godkjenning.</span><span class="sxs-lookup"><span data-stu-id="8f81d-118">After these policies are enabled, admins and users will be prompted to register for Azure Multii-Factor authentication.</span></span>

<span data-ttu-id="8f81d-119">Hvis du vil ha mer informasjon om disse policyene, kan du se [Hva er policyer for opprinnelig plan?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)</span><span class="sxs-lookup"><span data-stu-id="8f81d-119">For more information about these policies, see [What are baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?</span></span>


## <a name="set-up-baseline-policies"></a><span data-ttu-id="8f81d-120">Definere policyer for opprinnelig plan</span><span class="sxs-lookup"><span data-stu-id="8f81d-120">Set up baseline policies</span></span>

1. <span data-ttu-id="8f81d-121">Gå til [Azure-portalen](https://portal.azure.com), og naviger deretter til **Azure Active Directory** \> **Betinget tilgang**.</span><span class="sxs-lookup"><span data-stu-id="8f81d-121">Go to [Azure portal](https://portal.azure.com), and then navigate to **Azure Active Directory** \> **Conditional Access**.</span></span>
    
    <span data-ttu-id="8f81d-122">Policyene for opprinnelig plan er oppført på siden.</span><span class="sxs-lookup"><span data-stu-id="8f81d-122">The baseline policies are listed on the page.</span></span> <br/> <br/>
    <span data-ttu-id="8f81d-123">![Side som viser grunnlinjepolicyer for betinget tilgang.](../media/baslinepolicies.png)</span><span class="sxs-lookup"><span data-stu-id="8f81d-123">![Page that lists baseline policies for conditional access.](../media/baslinepolicies.png)</span></span>
1. <span data-ttu-id="8f81d-124">Se følgende spesifikke instruksjoner for hver policy:</span><span class="sxs-lookup"><span data-stu-id="8f81d-124">See the following specific instructions for each policy:</span></span>

  - [<span data-ttu-id="8f81d-125">Kreve MFA for administratorer</span><span class="sxs-lookup"><span data-stu-id="8f81d-125">Require MFA for admins</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [<span data-ttu-id="8f81d-126">Kreve MFA for brukere</span><span class="sxs-lookup"><span data-stu-id="8f81d-126">Require MFA for users</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [<span data-ttu-id="8f81d-127">Blokkere eldre godkjenning</span><span class="sxs-lookup"><span data-stu-id="8f81d-127">Block legacy authentication</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [<span data-ttu-id="8f81d-128">Kreve MFA for serviceadministrasjon</span><span class="sxs-lookup"><span data-stu-id="8f81d-128">Require MFA for service management</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

<span data-ttu-id="8f81d-129">Du kan definere mange tilleggspolicyer, for eksempel kreve godkjente klientapper.</span><span class="sxs-lookup"><span data-stu-id="8f81d-129">You can set up many additional policies, such as requiring approved client apps.</span></span> <span data-ttu-id="8f81d-130">Hvis du vil ha mer informasjon, kan du se [dokumentasjonen for betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="8f81d-130">For more information, see the [Conditional Access Documentation](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>
