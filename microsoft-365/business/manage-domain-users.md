---
title: Synkronisere domenebrukere til Microsoft 365
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Synkroniser domenekontrollerte brukere med Microsoft 365 for bedrifter.
ms.openlocfilehash: af9cb7c9b2b639edc2375679a73ab41c4cf6de71
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081907"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="41606-103">Synkronisere domenebrukere til Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="41606-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="41606-104">1. Klargjør for katalogsynkronisering</span><span class="sxs-lookup"><span data-stu-id="41606-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="41606-105">Før du synkroniserer brukere og datamaskiner fra det lokale Active Directory-domenet, kan du se [Klargjøre for katalogsynkronisering til Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="41606-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="41606-106">Spesielt:</span><span class="sxs-lookup"><span data-stu-id="41606-106">In particular:</span></span>

   - <span data-ttu-id="41606-107">Kontroller at det ikke finnes noen duplikater i katalogen for følgende attributter: **e-post**, **proxyAddresses**og **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="41606-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="41606-108">Disse verdiene må være unike, og eventuelle duplikater må fjernes.</span><span class="sxs-lookup"><span data-stu-id="41606-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="41606-109">Vi anbefaler at du konfigurerer **attributtet userPrincipalName** (UPN) for hver lokal brukerkonto slik at den samsvarer med den primære e-postadressen som tilsvarer den lisensierte Microsoft 365-brukeren.</span><span class="sxs-lookup"><span data-stu-id="41606-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="41606-110">For eksempel: *mary.shelley@contoso.com* i stedet for *mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="41606-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="41606-111">Hvis Active Directory-domenet slutter i et ikke-rutbart suffiks som *.local* eller *.lan*, i stedet for et Internett-rutbart suffiks, for eksempel *.com* eller *.org*, justerer du UPN-suffikset for de lokale brukerkontoene først som beskrevet i [Klargjør et ikke-rutbart domene for katalogsynkronisering](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="41606-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="41606-112">**Kjør IdFix** i trinn fire (4) nedenfor, vil også sørge for at den lokale Active Directory er klar for dir-synkronisering.</span><span class="sxs-lookup"><span data-stu-id="41606-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for dir sync.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="41606-113">2. Installere og konfigurere Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="41606-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="41606-114">Hvis du vil synkronisere brukere, grupper og kontakter fra den lokale Active Directory til Azure Active Directory, installerer du Azure Active Directory Connect og konfigurerer katalogsynkronisering.</span><span class="sxs-lookup"><span data-stu-id="41606-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="41606-115">Velg Oppsett i venstre navigasjonsenhet i administrasjonssenteret ved <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> å velge **Oppsett** i venstre navigasjonsenhet.</span><span class="sxs-lookup"><span data-stu-id="41606-115">In the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="41606-116">Under **Pålogging og sikkerhet**velger du **Vis** under Synkroniser brukere **fra organisasjonens katalog**.</span><span class="sxs-lookup"><span data-stu-id="41606-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="41606-117">Velg **Kom i gang**på siden Synkroniser brukere fra **organisasjonens katalog.**</span><span class="sxs-lookup"><span data-stu-id="41606-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="41606-118">I det første trinnet kjøre IdFix-verktøyet for å forberede for Katalogsynkronisering.</span><span class="sxs-lookup"><span data-stu-id="41606-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="41606-119">Følg trinnene i veiviseren for å laste ned Azure AD Connect og bruke den til å synkronisere domenekontrollerte brukere til Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="41606-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="41606-120">Se [Konfigurere katalogsynkronisering for Microsoft 365 for](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) å finne ut mer.</span><span class="sxs-lookup"><span data-stu-id="41606-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="41606-121">Når du konfigurerer alternativene for Azure AD Connect, anbefaler vi at du aktiverer **synkronisering av passord**, **sømløs enkel pålogging**og funksjonen for **tilbakeskriving** av passord, som også støttes i Microsoft 365 for bedrifter.</span><span class="sxs-lookup"><span data-stu-id="41606-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="41606-122">Det er noen flere trinn for passord writeback utover avmerkingsboksen i Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="41606-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="41606-123">Hvis du vil ha mer informasjon, kan du se [Slik gjør du det: konfigurere passord writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="41606-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="41606-124">Hvis du vil administrere domenet som er sammenkoblet med Windows 10-enheter også, kan du se [Aktivere domenet som er sammenkoblet med Windows 10-enheter, som skal administreres av Microsoft 365 Business Premium,](manage-windows-devices.md) til å konfigurere en hybrid Azure AD Join.</span><span class="sxs-lookup"><span data-stu-id="41606-124">If you want to manage domain-joined Windows 10 devices also, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 