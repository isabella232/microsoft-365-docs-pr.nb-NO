---
title: Synkronisere domene brukere til Microsoft 365
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
description: Synkronisere domene kontrollerte brukere med Microsoft 365 for bedrifter.
ms.openlocfilehash: 9495d893eb6870ef7c417a78f921296bfc0e6705
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306453"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a><span data-ttu-id="09938-103">Synkronisere domene brukere til Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="09938-103">Synchronize domain users to Microsoft 365</span></span>

## <a name="1-prepare-for-directory-synchronization"></a><span data-ttu-id="09938-104">1. klargjøre for katalog synkronisering</span><span class="sxs-lookup"><span data-stu-id="09938-104">1. Prepare for Directory Synchronization</span></span> 

<span data-ttu-id="09938-105">Før du synkroniserer brukere og data maskiner fra det lokale Active Directory-domenet, kan du se gjennom [klargjør for katalog synkronisering til Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="09938-105">Before you synchronize your users and computers from the local Active Directory Domain, review [Prepare for directory synchronization to Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization).</span></span> <span data-ttu-id="09938-106">Spesielt:</span><span class="sxs-lookup"><span data-stu-id="09938-106">In particular:</span></span>

   - <span data-ttu-id="09938-107">Kontroller at det ikke finnes duplikater i katalogen for følgende attributter: **e-post**, **proxyAddresses**og **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="09938-107">Make sure that no duplicates exist in your directory for the following attributes: **mail**, **proxyAddresses**, and **userPrincipalName**.</span></span> <span data-ttu-id="09938-108">Disse verdiene må være unike, og eventuelle duplikater må fjernes.</span><span class="sxs-lookup"><span data-stu-id="09938-108">These values must be unique and any duplicates must be removed.</span></span>
   
   - <span data-ttu-id="09938-109">Vi anbefaler at du konfigurerer **userPrincipalName** -attributtet (UPN) for hver lokale bruker konto til å samsvare med den primære e-postadressen som tilsvarer den lisensierte Microsoft 365-brukeren.</span><span class="sxs-lookup"><span data-stu-id="09938-109">We recommend that you configure the **userPrincipalName** (UPN) attribute for each local user account to match the primary email address that corresponds to the licensed Microsoft 365 user.</span></span> <span data-ttu-id="09938-110">For eksempel: *Mary.Shelley@contoso.com* i stedet for *Mary@contoso. lokal*</span><span class="sxs-lookup"><span data-stu-id="09938-110">For example: *mary.shelley@contoso.com* rather than *mary@contoso.local*</span></span>
   
   - <span data-ttu-id="09938-111">Hvis Active Directory-domenet slutter på et ikke-rutbart suffiks, for eksempel *lokal* eller *LAN*, i stedet for et Internett-omrutende suffiks, som for eksempel *. com* eller *. org*, justerer du UPN-suffikset for de lokale bruker kontoene først som beskrevet i [klargjøre et ikke-rutbart domene for katalog synkronisering](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span><span class="sxs-lookup"><span data-stu-id="09938-111">If the Active Directory domain ends in a non-routable suffix like *.local* or *.lan*, instead of an internet routable suffix such as *.com* or *.org*, adjust the UPN suffix of the local user accounts first as described in [Prepare a non-routable domain for directory synchronization](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization).</span></span> 

<span data-ttu-id="09938-112">**Kjør-IdFix** i trinn fire (4) nedenfor sørger også for at den lokale Active Directory er klar for katalog synkronisering.</span><span class="sxs-lookup"><span data-stu-id="09938-112">The **Run IdFix** in step four (4) below, will also make sure your on-premises Active Directory is ready for dir sync.</span></span>

## <a name="2-install-and-configure-azure-ad-connect"></a><span data-ttu-id="09938-113">2. installere og konfigurere Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="09938-113">2. Install and configure Azure AD Connect</span></span>

<span data-ttu-id="09938-114">Hvis du vil synkronisere brukere, grupper og kontakter fra den lokale Active Directory til Azure Active Directory, må du installere Azure Active Directory Connect og konfigurere katalog synkronisering.</span><span class="sxs-lookup"><span data-stu-id="09938-114">To synchronize your users, groups, and contacts from the local Active Directory into Azure Active Directory, install Azure Active Directory Connect and set up directory synchronization.</span></span> 

 1. <span data-ttu-id="09938-115">I administrasjons senteret ved å <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> velge **konfigurasjon** i det venstre navigasjons feltet.</span><span class="sxs-lookup"><span data-stu-id="09938-115">In the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> select **Setup** in the left nav.</span></span>

 2. <span data-ttu-id="09938-116">Under **pålogging og sikkerhet**velger du **Vis**  under **Synkroniser brukere fra organisasjonens katalog**.</span><span class="sxs-lookup"><span data-stu-id="09938-116">Under **Sign-in and security**, choose **View**  under **Sync users from your org's directory**.</span></span>

 3. <span data-ttu-id="09938-117">Velg **kom i gang**på siden **synkroniserings brukere fra din organisasjons katalog** .</span><span class="sxs-lookup"><span data-stu-id="09938-117">On the **Sync users from your org's directory** page, choose **Get started**.</span></span>

 4. <span data-ttu-id="09938-118">I det første trinnet Kjør IdFix-verktøyet for å klargjøre for katalog synkronisering.</span><span class="sxs-lookup"><span data-stu-id="09938-118">In the first step  run IdFix tool to prepare for Directory sync.</span></span>

 5. <span data-ttu-id="09938-119">Følg trinnene i vei viseren for å laste ned Azure AD Connect og bruke den til å synkronisere domene kontrollerte brukere til Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="09938-119">Follow the wizard steps to download Azure AD Connect and use it to synchronize your domain-controlled users to Microsoft 365.</span></span>


<span data-ttu-id="09938-120">Se [konfigurere katalog synkronisering for Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) for å finne ut mer.</span><span class="sxs-lookup"><span data-stu-id="09938-120">See [Set up directory synchronization for Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) to learn more.</span></span>

<span data-ttu-id="09938-121">Når du konfigurerer alternativene for Azure AD Connect, anbefaler vi at du aktiverer **passord synkronisering**, **sømløs enkel pålogging**og funksjonen for **passord bakgrunns skriving** , som også støttes i Microsoft 365 for Business.</span><span class="sxs-lookup"><span data-stu-id="09938-121">As you configure your options for Azure AD Connect, we recommend that you enable **Password Synchronization**, **Seamless Single Sign-On**, and the **password writeback** feature, which is also supported in Microsoft 365 for business.</span></span>

> [!NOTE]
> <span data-ttu-id="09938-122">Det finnes noen tilleggs trinn for bakgrunns skriving for passord utover avmerkings boksen i Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="09938-122">There are some additional steps for password writeback beyond the check box in Azure AD Connect.</span></span> <span data-ttu-id="09938-123">Hvis du vil ha mer informasjon, kan du se [How-to: Configure Password bakgrunns skriving](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="09938-123">For more information, see [How-to: configure password writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback).</span></span> 

<span data-ttu-id="09938-124">Hvis du vil administrere domene tilknyttede Windows 10-enheter også, kan du se [aktivere domene tilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business Premium](manage-windows-devices.md) , for å konfigurere en hybrid Azure ad-kobling.</span><span class="sxs-lookup"><span data-stu-id="09938-124">If you want to manage domain-joined Windows 10 devices also, see [Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium](manage-windows-devices.md) to set up a hybrid Azure AD Join.</span></span> 