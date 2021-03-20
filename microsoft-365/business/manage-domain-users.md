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
ms.openlocfilehash: 1c939dec7229f02991b15f08c48f184efecaddb0
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913258"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="6ce55-103">Synkronisere domenebrukere til Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6ce55-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="6ce55-104">1. Klargjøre for katalogsynkronisering</span><span class="sxs-lookup"><span data-stu-id="6ce55-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="6ce55-105">Før du synkroniserer brukere og datamaskiner fra det lokale Active Directory-domenet, kan du se [Klargjøre for katalogsynkronisering til Microsoft 365.](../enterprise/prepare-for-directory-synchronization.md)</span><span class="sxs-lookup"><span data-stu-id="6ce55-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](../enterprise/prepare-for-directory-synchronization.md).</span></span> <span data-ttu-id="6ce55-106">Spesielt:</span><span class="sxs-lookup"><span data-stu-id="6ce55-106">In particular:</span></span>

   - <span data-ttu-id="6ce55-107">Kontroller at det ikke finnes duplikater i katalogen for følgende attributter: **e-post,** **proxyAddresses** og **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="6ce55-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="6ce55-108">Disse verdiene må være unike, og eventuelle duplikater må fjernes.</span><span class="sxs-lookup"><span data-stu-id="6ce55-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="6ce55-109">Vi anbefaler at du konfigurerer **userPrincipalName-attributtet** (UPN) for hver lokale brukerkonto slik at den samsvarer med den primære e-postadressen som tilsvarer den lisensierte Microsoft 365-brukeren.</span><span class="sxs-lookup"><span data-stu-id="6ce55-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="6ce55-110">For eksempel: *mary.shelley@contoso.com* i stedet *mary@contoso.local*</span><span class="sxs-lookup"><span data-stu-id="6ce55-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="6ce55-111">Hvis Active [Directory-domenet](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md)slutter på et ikke-rutbart suffiks som *.local* eller *.lan*, i stedet for et suffiks som kan rutteres på Internett, for eksempel *.com* eller *.org,* justerer du UPN-suffikset for de lokale brukerkontoene først som beskrevet i Klargjøre et domene som ikke kan rutteres for katalogsynkronisering .</span><span class="sxs-lookup"><span data-stu-id="6ce55-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md).</span></span> 

<span data-ttu-id="6ce55-112">Kjør **IdFix i** trinn fire (4) nedenfor, vil også sørge for at den lokale Active Directory er klar for katalogsynkronisering.</span><span class="sxs-lookup"><span data-stu-id="6ce55-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for directory synchronization.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="6ce55-113">2. Installere og konfigurere Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="6ce55-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="6ce55-114">Hvis du vil synkronisere brukere, grupper og kontakter fra den lokale Active Directory til Azure Active Directory, installerer du Azure Active Directory Connect og konfigurerer katalogsynkronisering.</span><span class="sxs-lookup"><span data-stu-id="6ce55-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="6ce55-115">Velg Oppsett [i](https://go.microsoft.com/fwlink/p/?linkid=2024339)  det venstre navigasjonsfeltet i administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="6ce55-115">In the [admin center](https://go.microsoft.com/fwlink/p/?linkid=2024339), select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="6ce55-116">Velg **Vis under** Synkroniser brukere fra **organisasjonens katalog** under Pålogging og sikkerhet . </span><span class="sxs-lookup"><span data-stu-id="6ce55-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="6ce55-117">Velg Kom i gang på siden **Synkroniser** brukere fra **organisasjonens** katalog.</span><span class="sxs-lookup"><span data-stu-id="6ce55-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="6ce55-118">I det første trinnet kjører du IdFix-verktøyet for å klargjøre for katalogsynkronisering.</span><span class="sxs-lookup"><span data-stu-id="6ce55-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="6ce55-119">Følg trinnene i veiviseren for å laste ned Azure AD Connect og bruke det til å synkronisere domenekontrollerte brukere til Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6ce55-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="6ce55-120">Se [Konfigurere katalogsynkronisering for Microsoft 365 for](../enterprise/set-up-directory-synchronization.md) å finne ut mer.</span><span class="sxs-lookup"><span data-stu-id="6ce55-120">See [Set up directory synchronization for Microsoft 365](../enterprise/set-up-directory-synchronization.md) to learn more.</span></span>

<span data-ttu-id="6ce55-121">Når du konfigurerer alternativene for Azure AD Connect, anbefaler vi at du  aktiverer Passordsynkronisering, Sømløs enkel pålogging og funksjonen for tilbakeskriving av passord, som også støttes i Microsoft 365 for bedrifter.</span><span class="sxs-lookup"><span data-stu-id="6ce55-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="6ce55-122">Det finnes noen flere trinn for tilbakeskriving av passord utover avmerkingsboksen i Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="6ce55-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="6ce55-123">Hvis du vil ha mer informasjon, kan du [se Slik konfigurerer du tilbakeskriving av passord](/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="6ce55-123">For more information, see [How-to: configure password writeback](/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="6ce55-124">Hvis du også vil administrere domene-sammenføyde Windows 10-enheter, kan du se Aktivere domenekretserte [Windows 10-enheter](manage-windows-devices.md) som skal administreres av Microsoft 365 Business Premium for å konfigurere en hybrid Azure AD Join.</span><span class="sxs-lookup"><span data-stu-id="6ce55-124">If you also want to manage domain-joined Windows 10 devices, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span>