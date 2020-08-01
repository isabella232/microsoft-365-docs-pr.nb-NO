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
ms.openlocfilehash: 2eaf5aa76cae1680b93af008af615ae872e4fb20
ms.sourcegitcommit: fab425ea4580d1924fb421e6db233d135f5b7d19
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/31/2020
ms.locfileid: "46533789"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="9eed0-103">Aktivere domeneblede Windows 10-enheter som skal administreres av Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="9eed0-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="9eed0-104">Hvis organisasjonen bruker lokal Windows Server Active Directory, kan du konfigurere Microsoft 365 Business Premium til å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgangen til lokale ressurser som krever lokal godkjenning.</span><span class="sxs-lookup"><span data-stu-id="9eed0-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="9eed0-105">Hvis du vil konfigurere denne beskyttelsen, kan du implementere **Hybrid Azure AD sammenføyde enheter**.</span><span class="sxs-lookup"><span data-stu-id="9eed0-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="9eed0-106">Disse enhetene er koblet til både den lokale Active Directory og Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9eed0-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="9eed0-107">Denne videoen beskriver fremgangsmåten for hvordan du konfigurerer dette for det vanligste scenariet, som også er beskrevet i trinnene som følger.</span><span class="sxs-lookup"><span data-stu-id="9eed0-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="9eed0-108">Før du kommer i gang, må du sørge for at du fullfører disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="9eed0-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="9eed0-109">Synkroniser brukere til Azure AD med Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9eed0-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="9eed0-110">Fullfør Azure AD Connect Organizational Unit (OU)-synkronisering.</span><span class="sxs-lookup"><span data-stu-id="9eed0-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="9eed0-111">Kontroller at alle domenebrukerne du synkroniserer, har lisenser til Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="9eed0-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="9eed0-112">Se [Synkronisere domenebrukere til Microsoft](manage-domain-users.md) for fremgangsmåten.</span><span class="sxs-lookup"><span data-stu-id="9eed0-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="9eed0-113">1. Kontroller MDM-myndigheten i Intune</span><span class="sxs-lookup"><span data-stu-id="9eed0-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="9eed0-114">Gå til portal.azure.com og øverst på siden søker du etter Intune.</span><span class="sxs-lookup"><span data-stu-id="9eed0-114">Go to portal.azure.com and on the top of the page search for Intune.</span></span>
<span data-ttu-id="9eed0-115">Velg **Enhetsregistrering** på Siden Microsoft Intune, og kontroller at **MDM-myndighet** er Intune på **Siden Microsoft** **Intune.**</span><span class="sxs-lookup"><span data-stu-id="9eed0-115">On the Microsoft Intune page, select **Device enrollment** and on the **Overview** page make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="9eed0-116">Hvis **MDM-myndighet** er **Ingen**, klikker du **MDM-myndigheten** for å sette den til **Intune**.</span><span class="sxs-lookup"><span data-stu-id="9eed0-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="9eed0-117">Hvis **MDM-myndighet** er **Microsoft Office 365**, går du til **Enheter**  >  **Registrer enheter** og bruker dialogboksen Legg til **MDM-myndighet** til høyre for å legge til **Intune MDM-myndighet** (dialogboksen **Legg til MDM Authority** er bare tilgjengelig hvis **MDM Authority** er satt til Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="9eed0-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="9eed0-118">2. Kontroller at Azure AD er aktivert for sammenføyning av datamaskiner</span><span class="sxs-lookup"><span data-stu-id="9eed0-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="9eed0-119">Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> på, og velg **Azure Active Directory** (velg Vis alle hvis Azure Active Directory ikke er synlig) i listen over **administrasjonssentre.**</span><span class="sxs-lookup"><span data-stu-id="9eed0-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="9eed0-120">Gå til **Azure Active Directory** i **administrasjonssenteret**for Azure Active Directory , velg **Enheter** og deretter **Enhetsinnstillinger**.</span><span class="sxs-lookup"><span data-stu-id="9eed0-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="9eed0-121">Kontroller at**brukere kan koble enheter til Azure AD** er aktivert</span><span class="sxs-lookup"><span data-stu-id="9eed0-121">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="9eed0-122">Hvis du vil aktivere alle brukere, setter du til **Alle**.</span><span class="sxs-lookup"><span data-stu-id="9eed0-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="9eed0-123">Hvis du vil aktivere bestemte brukere, setter du til **Valgt** for å aktivere en bestemt gruppe brukere.</span><span class="sxs-lookup"><span data-stu-id="9eed0-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="9eed0-124">Legg til de ønskede domenebrukerne som er synkronisert i Azure AD i en [sikkerhetsgruppe](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="9eed0-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="9eed0-125">Velg **Velg grupper** for å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.</span><span class="sxs-lookup"><span data-stu-id="9eed0-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="9eed0-126">3. Kontroller at Azure AD er aktivert for MDM</span><span class="sxs-lookup"><span data-stu-id="9eed0-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="9eed0-127">Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> på, og velg **Endepunktsbehandler**t (velg **Vis alt** hvis **Endpoint Manager** ikke er synlig)</span><span class="sxs-lookup"><span data-stu-id="9eed0-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="9eed0-128">Gå til **Enheter**Automatisk registrering av Windows **Microsoft Endpoint Manager admin center**  >  **Windows**  >  **Windows-registrering**  >  **Automatic Enrollment**i administrasjonssenteret for Microsoft Endpoint Manager .</span><span class="sxs-lookup"><span data-stu-id="9eed0-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="9eed0-129">Kontroller at MDM-brukeromfang er aktivert.</span><span class="sxs-lookup"><span data-stu-id="9eed0-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="9eed0-130">Hvis du vil registrere alle datamaskiner, kan du sette til **Alle** for å registrere alle brukerdatamaskiner som er koblet til Azure AD og nye datamaskiner når brukerne legger til en arbeidskonto i Windows.</span><span class="sxs-lookup"><span data-stu-id="9eed0-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="9eed0-131">Sett til **Noen** for å registrere datamaskinene til en bestemt gruppe brukere.</span><span class="sxs-lookup"><span data-stu-id="9eed0-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="9eed0-132">Legg til de ønskede domenebrukerne som er synkronisert i Azure AD i en [sikkerhetsgruppe](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="9eed0-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="9eed0-133">Velg **Velg grupper** for å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.</span><span class="sxs-lookup"><span data-stu-id="9eed0-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="9eed0-134">4. Opprett de nødvendige ressursene</span><span class="sxs-lookup"><span data-stu-id="9eed0-134">4. Create the required resources</span></span> 

<span data-ttu-id="9eed0-135">Utføre de nødvendige oppgavene for å [konfigurere hybrid Azure AD-sammenføyning](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) er forenklet ved bruk av cmdleten [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) som finnes i [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell-modulen.</span><span class="sxs-lookup"><span data-stu-id="9eed0-135">Performing the required tasks to [configure hybrid Azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="9eed0-136">Når du starter denne cmdleten, opprettes og konfigurerer den nødvendige servicetilkoblingspunktet og gruppepolicyen.</span><span class="sxs-lookup"><span data-stu-id="9eed0-136">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="9eed0-137">Du kan installere denne modulen ved å påkalle følgende fra en forekomst av PowerShell:</span><span class="sxs-lookup"><span data-stu-id="9eed0-137">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="9eed0-138">Det anbefales at du installerer denne modulen på Windows Server som kjører Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9eed0-138">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="9eed0-139">Hvis du vil opprette den nødvendige tjenestetilkoblingspunktet og gruppepolicyen, vil du starte cmdleten [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) .</span><span class="sxs-lookup"><span data-stu-id="9eed0-139">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="9eed0-140">Du trenger den globale administratorlegitimasjonen for Microsoft 365 Business Premium når du utfører denne oppgaven.</span><span class="sxs-lookup"><span data-stu-id="9eed0-140">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="9eed0-141">Når du er klar til å opprette ressursene, starter du følgende:</span><span class="sxs-lookup"><span data-stu-id="9eed0-141">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="9eed0-142">Den første kommandoen oppretter en tilkobling til Microsoft-skyen, og når du blir bedt om det, angir du den globale administratorlegitimasjonen for Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="9eed0-142">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="9eed0-143">5. Koble til gruppepolicyen</span><span class="sxs-lookup"><span data-stu-id="9eed0-143">5. Link the Group Policy</span></span>

1. <span data-ttu-id="9eed0-144">Høyreklikk plasseringen der du vil koble policyen i Group Policy Management Console (GPMC), og velg *Koble et eksisterende Gruppepolicyobjekt...* fra hurtigmenyen.</span><span class="sxs-lookup"><span data-stu-id="9eed0-144">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="9eed0-145">Velg policyen som er opprettet i trinnet ovenfor, og klikk deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="9eed0-145">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="9eed0-146">Få de nyeste administrative malene</span><span class="sxs-lookup"><span data-stu-id="9eed0-146">Get the latest Administrative Templates</span></span>

<span data-ttu-id="9eed0-147">Hvis du ikke ser policyen **Aktiver automatisk MDM-registrering ved hjelp av standard Azure AD-legitimasjon**, kan det skyldes at du ikke har ADMX installert for Windows 10, versjon 1803, versjon 1809 eller versjon 1903.</span><span class="sxs-lookup"><span data-stu-id="9eed0-147">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="9eed0-148">Hvis du vil løse problemet, følger du denne fremgangsmåten (Merk: Den nyeste MDM.admx er bakoverkompatibel):</span><span class="sxs-lookup"><span data-stu-id="9eed0-148">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="9eed0-149">Last ned: [Administrative maler (ADMX) for Windows 10 mai 2019 Oppdatering (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="9eed0-149">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="9eed0-150">Installere pakken på den primære domenekontrolleren (PDC).</span><span class="sxs-lookup"><span data-stu-id="9eed0-150">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="9eed0-151">Naviger, avhengig av hvilken versjon til mappen: **C:\Programfiler (x86)\Microsoft gruppepolicy\Windows 10 Mai 2019 Oppdatering (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="9eed0-151">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="9eed0-152">Gi nytt navn til **policydefinisjoner-mappen** i banen ovenfor til **PolicyDefinitions**.</span><span class="sxs-lookup"><span data-stu-id="9eed0-152">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="9eed0-153">Kopier **PolicyDefinitions-mappen** til **C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="9eed0-153">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="9eed0-154">Hvis du planlegger å bruke et sentralt policylager for hele domenet, legger du til innholdet i PolicyDefinitions der.</span><span class="sxs-lookup"><span data-stu-id="9eed0-154">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="9eed0-155">Start den primære domenekontrolleren på nytt for at policyen skal være tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="9eed0-155">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="9eed0-156">Denne prosedyren vil fungere for alle fremtidige versjoner også.</span><span class="sxs-lookup"><span data-stu-id="9eed0-156">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="9eed0-157">På dette tidspunktet bør du kunne se policyen **Aktiver automatisk MDM-registrering ved hjelp av standard Azure AD-legitimasjon** tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="9eed0-157">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>
