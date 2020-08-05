---
title: Aktivere domene-sammenføyde Windows 10-enheter som skal administreres av Microsoft 365 for bedrifter
f1.keywords:
- CSH
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
description: Lær hvordan du aktiverer Microsoft 365 til å beskytte lokale Active-Directory-tilkoblede Windows 10-enheter med bare noen få trinn.
ms.openlocfilehash: 6275c6c4be9cd9631ab095f8b0e1b39683022bb2
ms.sourcegitcommit: d988faa292c2661ffea43c7161aef92b2b4b99bc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/04/2020
ms.locfileid: "46560847"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="392d5-103">Aktivere domeneblede Windows 10-enheter som skal administreres av Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="392d5-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="392d5-104">Hvis organisasjonen bruker lokal Windows Server Active Directory, kan du konfigurere Microsoft 365 Business Premium til å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgangen til lokale ressurser som krever lokal godkjenning.</span><span class="sxs-lookup"><span data-stu-id="392d5-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="392d5-105">Hvis du vil konfigurere denne beskyttelsen, kan du implementere **Hybrid Azure AD sammenføyde enheter**.</span><span class="sxs-lookup"><span data-stu-id="392d5-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="392d5-106">Disse enhetene er koblet til både den lokale Active Directory og Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="392d5-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="392d5-107">Denne videoen beskriver fremgangsmåten for hvordan du konfigurerer dette for det vanligste scenariet, som også er beskrevet i trinnene som følger.</span><span class="sxs-lookup"><span data-stu-id="392d5-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="392d5-108">Før du kommer i gang, må du sørge for at du fullfører disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="392d5-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="392d5-109">Synkroniser brukere til Azure AD med Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="392d5-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="392d5-110">Fullfør Azure AD Connect Organizational Unit (OU)-synkronisering.</span><span class="sxs-lookup"><span data-stu-id="392d5-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="392d5-111">Kontroller at alle domenebrukerne du synkroniserer, har lisenser til Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="392d5-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="392d5-112">Se [Synkronisere domenebrukere til Microsoft](manage-domain-users.md) for fremgangsmåten.</span><span class="sxs-lookup"><span data-stu-id="392d5-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="392d5-113">1. Kontroller MDM-myndigheten i Intune</span><span class="sxs-lookup"><span data-stu-id="392d5-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="392d5-114">Gå til [Endpoint Manager,](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) og velg **Enhetsregistrering**på Siden Microsoft Intune , og kontroller deretter at **MDM-myndighet** er **Intune**på **Siden Oversikt.**</span><span class="sxs-lookup"><span data-stu-id="392d5-114">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="392d5-115">Hvis **MDM-myndighet** er **Ingen**, klikker du **MDM-myndigheten** for å sette den til **Intune**.</span><span class="sxs-lookup"><span data-stu-id="392d5-115">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="392d5-116">Hvis **MDM-myndighet** er **Microsoft Office 365**, går du til **Enheter**  >  **Registrer enheter** og bruker dialogboksen Legg til **MDM-myndighet** til høyre for å legge til **Intune MDM-myndighet** (dialogboksen **Legg til MDM Authority** er bare tilgjengelig hvis **MDM Authority** er satt til Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="392d5-116">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="392d5-117">2. Kontroller at Azure AD er aktivert for sammenføyning av datamaskiner</span><span class="sxs-lookup"><span data-stu-id="392d5-117">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="392d5-118">Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> på, og velg **Azure Active Directory** (velg Vis alle hvis Azure Active Directory ikke er synlig) i listen over **administrasjonssentre.**</span><span class="sxs-lookup"><span data-stu-id="392d5-118">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="392d5-119">Gå til **Azure Active Directory** i **administrasjonssenteret**for Azure Active Directory , velg **Enheter** og deretter **Enhetsinnstillinger**.</span><span class="sxs-lookup"><span data-stu-id="392d5-119">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="392d5-120">Kontroller at**brukere kan koble enheter til Azure AD** er aktivert</span><span class="sxs-lookup"><span data-stu-id="392d5-120">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="392d5-121">Hvis du vil aktivere alle brukere, setter du til **Alle**.</span><span class="sxs-lookup"><span data-stu-id="392d5-121">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="392d5-122">Hvis du vil aktivere bestemte brukere, setter du til **Valgt** for å aktivere en bestemt gruppe brukere.</span><span class="sxs-lookup"><span data-stu-id="392d5-122">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="392d5-123">Legg til de ønskede domenebrukerne som er synkronisert i Azure AD i en [sikkerhetsgruppe](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="392d5-123">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="392d5-124">Velg **Velg grupper** for å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.</span><span class="sxs-lookup"><span data-stu-id="392d5-124">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="392d5-125">3. Kontroller at Azure AD er aktivert for MDM</span><span class="sxs-lookup"><span data-stu-id="392d5-125">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="392d5-126">Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> på, og velg **Endepunktsbehandler**t (velg **Vis alt** hvis **Endpoint Manager** ikke er synlig)</span><span class="sxs-lookup"><span data-stu-id="392d5-126">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="392d5-127">Gå til **Enheter**Automatisk registrering av Windows **Microsoft Endpoint Manager admin center**  >  **Windows**  >  **Windows-registrering**  >  **Automatic Enrollment**i administrasjonssenteret for Microsoft Endpoint Manager .</span><span class="sxs-lookup"><span data-stu-id="392d5-127">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="392d5-128">Kontroller at MDM-brukeromfang er aktivert.</span><span class="sxs-lookup"><span data-stu-id="392d5-128">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="392d5-129">Hvis du vil registrere alle datamaskiner, kan du sette til **Alle** for å registrere alle brukerdatamaskiner som er koblet til Azure AD og nye datamaskiner når brukerne legger til en arbeidskonto i Windows.</span><span class="sxs-lookup"><span data-stu-id="392d5-129">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="392d5-130">Sett til **Noen** for å registrere datamaskinene til en bestemt gruppe brukere.</span><span class="sxs-lookup"><span data-stu-id="392d5-130">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="392d5-131">Legg til de ønskede domenebrukerne som er synkronisert i Azure AD i en [sikkerhetsgruppe](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="392d5-131">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="392d5-132">Velg **Velg grupper** for å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.</span><span class="sxs-lookup"><span data-stu-id="392d5-132">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="392d5-133">4. Opprett de nødvendige ressursene</span><span class="sxs-lookup"><span data-stu-id="392d5-133">4. Create the required resources</span></span> 

<span data-ttu-id="392d5-134">Utføre de nødvendige oppgavene for å [konfigurere hybrid Azure AD-sammenføyning](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) er forenklet ved bruk av cmdleten [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) som finnes i [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell-modulen.</span><span class="sxs-lookup"><span data-stu-id="392d5-134">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="392d5-135">Når du starter denne cmdleten, opprettes og konfigurerer den nødvendige servicetilkoblingspunktet og gruppepolicyen.</span><span class="sxs-lookup"><span data-stu-id="392d5-135">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="392d5-136">Du kan installere denne modulen ved å påkalle følgende fra en forekomst av PowerShell:</span><span class="sxs-lookup"><span data-stu-id="392d5-136">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="392d5-137">Det anbefales at du installerer denne modulen på Windows Server som kjører Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="392d5-137">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="392d5-138">Hvis du vil opprette den nødvendige tjenestetilkoblingspunktet og gruppepolicyen, vil du starte cmdleten [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) .</span><span class="sxs-lookup"><span data-stu-id="392d5-138">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="392d5-139">Du trenger den globale administratorlegitimasjonen for Microsoft 365 Business Premium når du utfører denne oppgaven.</span><span class="sxs-lookup"><span data-stu-id="392d5-139">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="392d5-140">Når du er klar til å opprette ressursene, starter du følgende:</span><span class="sxs-lookup"><span data-stu-id="392d5-140">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="392d5-141">Den første kommandoen oppretter en tilkobling til Microsoft-skyen, og når du blir bedt om det, angir du den globale administratorlegitimasjonen for Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="392d5-141">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="392d5-142">5. Koble til gruppepolicyen</span><span class="sxs-lookup"><span data-stu-id="392d5-142">5. Link the Group Policy</span></span>

1. <span data-ttu-id="392d5-143">Høyreklikk plasseringen der du vil koble policyen i Group Policy Management Console (GPMC), og velg *Koble et eksisterende Gruppepolicyobjekt...* fra hurtigmenyen.</span><span class="sxs-lookup"><span data-stu-id="392d5-143">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="392d5-144">Velg policyen som er opprettet i trinnet ovenfor, og klikk deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="392d5-144">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="392d5-145">Få de nyeste administrative malene</span><span class="sxs-lookup"><span data-stu-id="392d5-145">Get the latest Administrative Templates</span></span>

<span data-ttu-id="392d5-146">Hvis du ikke ser policyen **Aktiver automatisk MDM-registrering ved hjelp av standard Azure AD-legitimasjon**, kan det skyldes at du ikke har ADMX installert for Windows 10, versjon 1803, versjon 1809 eller versjon 1903.</span><span class="sxs-lookup"><span data-stu-id="392d5-146">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="392d5-147">Hvis du vil løse problemet, følger du denne fremgangsmåten (Merk: Den nyeste MDM.admx er bakoverkompatibel):</span><span class="sxs-lookup"><span data-stu-id="392d5-147">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="392d5-148">Last ned: [Administrative maler (ADMX) for Windows 10 mai 2019 Oppdatering (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="392d5-148">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="392d5-149">Installere pakken på den primære domenekontrolleren (PDC).</span><span class="sxs-lookup"><span data-stu-id="392d5-149">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="392d5-150">Naviger, avhengig av hvilken versjon til mappen: **C:\Programfiler (x86)\Microsoft gruppepolicy\Windows 10 Mai 2019 Oppdatering (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="392d5-150">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="392d5-151">Gi nytt navn til **policydefinisjoner-mappen** i banen ovenfor til **PolicyDefinitions**.</span><span class="sxs-lookup"><span data-stu-id="392d5-151">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="392d5-152">Kopier **PolicyDefinitions-mappen** til **C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="392d5-152">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="392d5-153">Hvis du planlegger å bruke et sentralt policylager for hele domenet, legger du til innholdet i PolicyDefinitions der.</span><span class="sxs-lookup"><span data-stu-id="392d5-153">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="392d5-154">Start den primære domenekontrolleren på nytt for at policyen skal være tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="392d5-154">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="392d5-155">Denne prosedyren vil fungere for alle fremtidige versjoner også.</span><span class="sxs-lookup"><span data-stu-id="392d5-155">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="392d5-156">På dette tidspunktet bør du kunne se policyen **Aktiver automatisk MDM-registrering ved hjelp av standard Azure AD-legitimasjon** tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="392d5-156">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>
