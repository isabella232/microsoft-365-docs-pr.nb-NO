---
title: Redigere eller angi innstillinger for programbeskyttelse for Windows 10-enheter
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
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
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Lær hvordan du oppretter eller redigerer policyer for appbehandling og beskytter arbeidsfiler på brukernes personlige Windows 10-enheter.
ms.openlocfilehash: 64c6aa620171a373cd7564c7de3abbf4a4546c4e
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "50912826"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a><span data-ttu-id="5289e-103">Angi eller redigere innstillinger for programbeskyttelse for Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="5289e-103">Set or edit application protection settings for Windows 10 devices</span></span>

<span data-ttu-id="5289e-104">Denne artikkelen gjelder for Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="5289e-104">This article applies to Microsoft 365 Business Premium.</span></span>

## <a name="edit-an-app-management-policy-for-windows-10"></a><span data-ttu-id="5289e-105">Redigere en policy for appbehandling for Windows 10</span><span class="sxs-lookup"><span data-stu-id="5289e-105">Edit an app management policy for Windows 10</span></span>

1. <span data-ttu-id="5289e-106">Gå til administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="5289e-106">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span>     
2. <span data-ttu-id="5289e-107">Velg Enheter policyer **til** \> **venstre.**</span><span class="sxs-lookup"><span data-stu-id="5289e-107">On the left nav, choose **Devices** \> **Policies** .</span></span>
1. <span data-ttu-id="5289e-108">Velg en eksisterende policy for Windows-appen, og velg deretter **Rediger**.</span><span class="sxs-lookup"><span data-stu-id="5289e-108">Choose an existing Windows app policy and then **Edit**.</span></span>
1. <span data-ttu-id="5289e-109">Velg **Rediger** ved siden av en innstilling du vil endre, og velg deretter **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="5289e-109">Choose **Edit** next to a setting you want to change and then **Save**.</span></span>

## <a name="create-an-app-management-policy-for-windows-10"></a><span data-ttu-id="5289e-110">Opprette en policy for appbehandling for Windows 10</span><span class="sxs-lookup"><span data-stu-id="5289e-110">Create an app management policy for Windows 10</span></span>

<span data-ttu-id="5289e-111">Hvis brukerne har personlige Windows 10-enheter der de utfører arbeidsoppgaver, kan du beskytte dataene dine på disse enhetene i tillegg.</span><span class="sxs-lookup"><span data-stu-id="5289e-111">If your users have personal Windows 10 devices on which they perform work tasks, you can protect your data on those devices as well.</span></span>
  
1. <span data-ttu-id="5289e-112">Gå til administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .</span><span class="sxs-lookup"><span data-stu-id="5289e-112">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.</span></span> 
2. <span data-ttu-id="5289e-113">Velg Legg til  enheter \> **policyer til** \> **venstre.**</span><span class="sxs-lookup"><span data-stu-id="5289e-113">On the left nav, choose **Devices** \> **Policies** \> **Add**.</span></span>
3. <span data-ttu-id="5289e-114">Angi et unikt navn for denne policyen i **Legg til Policy**-ruten.</span><span class="sxs-lookup"><span data-stu-id="5289e-114">On the **Add policy** pane, enter a unique name for this policy.</span></span> 
4. <span data-ttu-id="5289e-115">Velg **Programbehandling for Windows 10** under **Policytype**.</span><span class="sxs-lookup"><span data-stu-id="5289e-115">Under **Policy type**, choose **Application Management for Windows 10**.</span></span>
5. <span data-ttu-id="5289e-116">Velg **Personlig eller**  Firmaeid under **Enhetstype**.</span><span class="sxs-lookup"><span data-stu-id="5289e-116">Under **Device type**, choose either **Personal** or **Company Owned**.</span></span>
6. <span data-ttu-id="5289e-117">**Krypter arbeidsfiler** aktiveres automatisk.</span><span class="sxs-lookup"><span data-stu-id="5289e-117">The **Encrypt work files** is turned on automatically.</span></span> 
7. <span data-ttu-id="5289e-118">Sett **Forhindre brukere fra å kopiere bedriftsdata til personlige filer, og tvinge dem til å lagre arbeidsfiler til OneDrive for Business** til **På** hvis du ikke vil at brukerne skal lagre arbeidsfiler på PCen.</span><span class="sxs-lookup"><span data-stu-id="5289e-118">Set **Prevent users from copying company data to personal files and force them to save work files to OneDrive for Business** to **On** if you don't want the users to save work files on their PC.</span></span> 
9. <span data-ttu-id="5289e-119">Utvid **Gjenopprett data på Windows-enheter**.</span><span class="sxs-lookup"><span data-stu-id="5289e-119">Expand **Recover data on Windows devices**.</span></span> <span data-ttu-id="5289e-120">Vi anbefaler at du slår den **på**.</span><span class="sxs-lookup"><span data-stu-id="5289e-120">We recommend that you turn it **On**.</span></span>
    <span data-ttu-id="5289e-121">Før du kan bla til plasseringen av Sertifikatet for datagjenopprettingsagent, må du først opprette ett.</span><span class="sxs-lookup"><span data-stu-id="5289e-121">Before you can browse to the location of the Data Recovery Agent certificate, you have to first create one.</span></span> <span data-ttu-id="5289e-122">Hvis du vil ha instruksjoner, kan du se Opprette og [bekrefte et EFS-sertifikat (Encrypting File System) Data Recovery Agent (DRA).](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate)</span><span class="sxs-lookup"><span data-stu-id="5289e-122">For instructions, see [Create and verify an Encrypting File System (EFS) Data Recovery Agent (DRA) certificate](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate).</span></span>
    
    <span data-ttu-id="5289e-123">Som standard blir arbeidsfiler kryptert ved hjelp av en hemmelig nøkkel som er lagret på enheten og knyttet til brukerens profil.</span><span class="sxs-lookup"><span data-stu-id="5289e-123">By default, work files are encrypted using a secret key that is stored on the device and associated with the user's profile.</span></span> <span data-ttu-id="5289e-124">Bare brukeren kan åpne og dekryptere filen.</span><span class="sxs-lookup"><span data-stu-id="5289e-124">Only the user can open and decrypt the file.</span></span> <span data-ttu-id="5289e-125">Men hvis en enhet mistes eller en bruker fjernes, kan en fil bli sittende fast i en kryptert tilstand.</span><span class="sxs-lookup"><span data-stu-id="5289e-125">However, if a device is lost or a user is removed, a file can be stuck in an encrypted state.</span></span> <span data-ttu-id="5289e-126">En administrator kan bruke datagjenopprettingsagentsertifikatet (DRA) til å dekryptere filen.</span><span class="sxs-lookup"><span data-stu-id="5289e-126">An admin can use the Data Recovery Agent (DRA) certificate to decrypt the file.</span></span>
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. <span data-ttu-id="5289e-128">Utvid **Beskytt flere nettverks-** og skyplasseringer hvis du vil legge til flere domener eller SharePoint Online-plasseringer for å sikre at filene i alle de oppførte appene er beskyttet.</span><span class="sxs-lookup"><span data-stu-id="5289e-128">Expand **Protect additional network and cloud locations** if you want to add additional domains or SharePoint Online locations to make sure that files in all the listed apps are protected.</span></span> <span data-ttu-id="5289e-129">Hvis du trenger å angi mer enn ett element for hvert felt, kan du bruke semikolon (;) mellom elementene.</span><span class="sxs-lookup"><span data-stu-id="5289e-129">If you need to enter more than one item for either field, use a semicolon (;) between the items.</span></span>
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. <span data-ttu-id="5289e-p104">Bestem deretter **Hvem får disse innstillingene?** Hvis du ikke vil bruke den standard sikkerhetsgruppen **Alle brukere**, velger du **Endre** og deretter sikkerhetsgruppene som vil få disse innstillingene \> **Velg**.</span><span class="sxs-lookup"><span data-stu-id="5289e-p104">Next decide **Who will get these settings?** If you don't want to use the default **All Users** security group, choose **Change**, choose the security groups who will get these settings \> **Select**.</span></span>
12. <span data-ttu-id="5289e-133">Velg til slutt **Legg til** for å lagre policyen og tilordne den til enhetene.</span><span class="sxs-lookup"><span data-stu-id="5289e-133">Finally, choose **Add** to save the policy, and assign it to devices.</span></span>