---
title: Aktiver domene-sammenføyde Windows 10-enheter som skal administreres av Microsoft 365 for bedrifter
f1.keywords:
- CSH
ms.author: efrene
author: efrene
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
description: Lær hvordan du aktiverer Microsoft 365 å beskytte lokale Active-Directory-sammenføyde Windows 10 enheter med bare noen få trinn.
ms.openlocfilehash: eb95c437030ae13a44f5e8043b3544d5846001c2
ms.sourcegitcommit: 4886457c0d4248407bddec56425dba50bb60d9c4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/03/2021
ms.locfileid: "53287699"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="94519-103">Aktiver domeneføyde Windows 10 enheter som skal administreres av Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="94519-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="94519-104">Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business Premium til å beskytte Windows 10-enhetene, samtidig som du beholder tilgang til lokale ressurser som krever lokal godkjenning.</span><span class="sxs-lookup"><span data-stu-id="94519-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="94519-105">Hvis du vil konfigurere denne beskyttelsen, kan du implementere **Hybrid Azure AD-sammenføyde enheter.**</span><span class="sxs-lookup"><span data-stu-id="94519-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="94519-106">Disse enhetene er koblet til både den lokale Active Directory og Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="94519-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

## <a name="watch-configure-hybrid-azure-active-directory-join"></a><span data-ttu-id="94519-107">Se: Konfigurere hybrid Azure Active Directory bli med</span><span class="sxs-lookup"><span data-stu-id="94519-107">Watch: Configure Hybrid Azure Active Directory join</span></span>

<span data-ttu-id="94519-108">Denne videoen beskriver trinnene for hvordan du konfigurerer dette for det vanligste scenarioet, som også er beskrevet i fremgangsmåten nedenfor.</span><span class="sxs-lookup"><span data-stu-id="94519-108">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="before-you-begin"></a><span data-ttu-id="94519-109">Før du starter</span><span class="sxs-lookup"><span data-stu-id="94519-109">Before you begin</span></span>

- <span data-ttu-id="94519-110">Synkroniser brukere med Azure AD med Azure AD Koble til.</span><span class="sxs-lookup"><span data-stu-id="94519-110">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="94519-111">Fullfør Azure AD Koble til Organizational Unit (OU)-synkronisering.</span><span class="sxs-lookup"><span data-stu-id="94519-111">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="94519-112">Kontroller at alle domenebrukerne du synkroniserer, har lisenser for å Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="94519-112">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="94519-113">Se [Synkronisere domenebrukere til Microsoft](manage-domain-users.md) for å se fremgangsmåten.</span><span class="sxs-lookup"><span data-stu-id="94519-113">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="94519-114">1. Bekreft MDM Authority i Intune</span><span class="sxs-lookup"><span data-stu-id="94519-114">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="94519-115">Gå til [Endpoint Manager,](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) og på Microsoft Intune velger du Enhetsregistrering **,** og  deretter kontrollerer du at **MDM-autoritet** er Intune på **Oversikt-siden.**</span><span class="sxs-lookup"><span data-stu-id="94519-115">Go to [Endpoint Manager](https://endpoint.microsoft.com/#blade/Microsoft_Intune_Enrollment/EnrollmentMenu/overview) and on the Microsoft Intune page, select **Device enrollment**, then on the **Overview** page, make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="94519-116">Hvis **MDM-autoritet** **er Ingen,** klikker du **MDM-instansen** for å sette den til **Intune**.</span><span class="sxs-lookup"><span data-stu-id="94519-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="94519-117">Hvis **MDM-autoritet** er **Microsoft Office 365,** går du til Enheter Registrere enheter og bruker dialogboksen Legg til MDM-autoritet til høyre for å legge til  >   **Intune MDM-autoritet** (dialogboksen Legg til **MDM-autoritet** er bare tilgjengelig hvis **MDM-myndigheten** er satt til  Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="94519-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="94519-118">2. Kontroller at Azure AD er aktivert for sammenføyning av datamaskiner</span><span class="sxs-lookup"><span data-stu-id="94519-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="94519-119">Gå til administrasjonssenteret på, og Azure Active Directory (velg Vis alle hvis Azure Active Directory ikke er synlig) i listen <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> **over administrasjonssentre.** </span><span class="sxs-lookup"><span data-stu-id="94519-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="94519-120">I **administrasjonssenteret Azure Active Directory** går du **til Azure Active Directory** , **velger Enheter** og deretter **Enhetsinnstillinger**.</span><span class="sxs-lookup"><span data-stu-id="94519-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="94519-121">Kontroller **at brukere kan bli med i enheter til Azure AD** er aktivert</span><span class="sxs-lookup"><span data-stu-id="94519-121">Verify **Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="94519-122">Hvis du vil aktivere alle brukere, setter du til **Alle**.</span><span class="sxs-lookup"><span data-stu-id="94519-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="94519-123">Hvis du vil aktivere bestemte brukere, setter du til **Valgt** for å aktivere en bestemt gruppe brukere.</span><span class="sxs-lookup"><span data-stu-id="94519-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="94519-124">Legg til de ønskede domenebrukerne synkronisert i Azure AD i en [sikkerhetsgruppe.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="94519-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="94519-125">Velg **Velg grupper for** å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.</span><span class="sxs-lookup"><span data-stu-id="94519-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="94519-126">3. Kontroller at Azure AD er aktivert for MDM</span><span class="sxs-lookup"><span data-stu-id="94519-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="94519-127">Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> på, og velg  Endepunktadministrasjon t (velg Vis **alle hvis** Endpoint Manager ikke er synlig)</span><span class="sxs-lookup"><span data-stu-id="94519-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen** t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="94519-128">Gå til **Windows** Windows registrering automatisk registrering i  >  **Microsoft Endpoint Manager**  >    >  **administrasjonssenteret**.</span><span class="sxs-lookup"><span data-stu-id="94519-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="94519-129">Kontroller at MDM-brukeromfang er aktivert.</span><span class="sxs-lookup"><span data-stu-id="94519-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="94519-130">Hvis du vil registrere  alle datamaskinene, setter du til Alle til å registrere automatisk alle brukerdatamaskiner som er sammenføyd med Azure AD og nye datamaskiner når brukerne legger til en jobbkonto Windows.</span><span class="sxs-lookup"><span data-stu-id="94519-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="94519-131">Sett til **Noen for** å registrere datamaskinene til en bestemt gruppe brukere.</span><span class="sxs-lookup"><span data-stu-id="94519-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="94519-132">Legg til de ønskede domenebrukerne synkronisert i Azure AD i en [sikkerhetsgruppe.](../admin/create-groups/create-groups.md)</span><span class="sxs-lookup"><span data-stu-id="94519-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="94519-133">Velg **Velg grupper for** å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.</span><span class="sxs-lookup"><span data-stu-id="94519-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-create-the-required-resources"></a><span data-ttu-id="94519-134">4. Opprett de nødvendige ressursene</span><span class="sxs-lookup"><span data-stu-id="94519-134">4. Create the required resources</span></span> 

<span data-ttu-id="94519-135">Utføring av de nødvendige oppgavene for å konfigurere hybrid Azure AD-sammenføyning har blitt forenklet ved bruk av cmdleten [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) som ble funnet i [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell-modulen. [](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="94519-135">Performing the required tasks to [configure hybrid Azure AD join](/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join) has been simplified through the use of the [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet found in the [SecMgmt](https://www.powershellgallery.com/packages/SecMgmt) PowerShell module.</span></span> <span data-ttu-id="94519-136">Når du starter denne cmdleten, opprettes og konfigureres det nødvendige koblingspunktet og gruppepolicyen for tjenesten.</span><span class="sxs-lookup"><span data-stu-id="94519-136">When you invoke this cmdlet it will create and configure the required service connection point and group policy.</span></span>

<span data-ttu-id="94519-137">Du kan installere denne modulen ved å aktivere følgende fra en forekomst av PowerShell:</span><span class="sxs-lookup"><span data-stu-id="94519-137">You can install this module by invoking the following from an instance of PowerShell:</span></span>

```powershell
Install-Module SecMgmt
```

> [!IMPORTANT]
> <span data-ttu-id="94519-138">Det anbefales at du installerer denne modulen på Windows server som kjører Azure AD Koble til.</span><span class="sxs-lookup"><span data-stu-id="94519-138">It is recommended that you install this module on the Windows Server running Azure AD Connect.</span></span>

<span data-ttu-id="94519-139">Hvis du vil opprette det nødvendige tjenestetilkoblingspunktet og gruppepolicyen, starter du cmdleten [Initialize-SecMgmtHybirdDeviceEnrollment.](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md)</span><span class="sxs-lookup"><span data-stu-id="94519-139">To create the required service connection point and group policy, you will invoke the  [Initialize-SecMgmtHybirdDeviceEnrollment](https://github.com/microsoft/secmgmt-open-powershell/blob/master/docs/help/Initialize-SecMgmtHybirdDeviceEnrollment.md) cmdlet.</span></span> <span data-ttu-id="94519-140">Du trenger den Microsoft 365 Business Premium administratorlegitimasjon når du utfører denne oppgaven.</span><span class="sxs-lookup"><span data-stu-id="94519-140">You will need your Microsoft 365 Business Premium global admin credentials when performing this task.</span></span> <span data-ttu-id="94519-141">Når du er klar til å opprette ressursene, kan du aktivere følgende:</span><span class="sxs-lookup"><span data-stu-id="94519-141">When you are ready to create the resources, invoke the following:</span></span>

```powershell
PS C:\> Connect-SecMgmtAccount
PS C:\> Initialize-SecMgmtHybirdDeviceEnrollment -GroupPolicyDisplayName 'Device Management'
```

<span data-ttu-id="94519-142">Den første kommandoen etablerer en tilkobling til Microsoft-skyen, og når du blir bedt om det, angir Microsoft 365 Business Premium den globale administratorlegitimasjonen.</span><span class="sxs-lookup"><span data-stu-id="94519-142">The first command will establish a connection with the Microsoft cloud, and when you are prompted, specify your Microsoft 365 Business Premium global admin credentials.</span></span>

## <a name="5-link-the-group-policy"></a><span data-ttu-id="94519-143">5. Koble gruppepolicyen</span><span class="sxs-lookup"><span data-stu-id="94519-143">5. Link the Group Policy</span></span>

1. <span data-ttu-id="94519-144">Høyreklikk plasseringen der du vil koble policyen, i konsollen for gruppepolicybehandling (GPMC), og velg Koble et eksisterende *gruppepolicyobjekt...* fra hurtigmenyen.</span><span class="sxs-lookup"><span data-stu-id="94519-144">In the Group Policy Management Console (GPMC), right-click on the location where you want to link the policy and select *Link an existing GPO...* from the context menu.</span></span>
2. <span data-ttu-id="94519-145">Velg policyen som ble opprettet i trinnet ovenfor, og klikk deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="94519-145">Select the policy created in the above step, then click **OK**.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="94519-146">Få de nyeste administrative malene</span><span class="sxs-lookup"><span data-stu-id="94519-146">Get the latest Administrative Templates</span></span>

<span data-ttu-id="94519-147">Hvis du ikke ser policyen Aktivere automatisk **MDM-registrering** ved hjelp av standard Azure AD-legitimasjon, kan det være fordi du ikke har ADMX installert for Windows 10, versjon 1803 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="94519-147">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, or later.</span></span> <span data-ttu-id="94519-148">Følg disse trinnene for å løse problemet (Merk: den nyeste MDM.admx er bakoverkompatibel):</span><span class="sxs-lookup"><span data-stu-id="94519-148">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1. <span data-ttu-id="94519-149">Last ned: [Administrative maler (ADMX) for Windows 10 oktober 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span><span class="sxs-lookup"><span data-stu-id="94519-149">Download: [Administrative Templates (.admx) for Windows 10 October 2020 Update (20H2)](https://www.microsoft.com/download/102157).</span></span>
2. <span data-ttu-id="94519-150">Installer pakken på en domenekontroller.</span><span class="sxs-lookup"><span data-stu-id="94519-150">Install the package on a Domain Controller.</span></span>
3. <span data-ttu-id="94519-151">Naviger, avhengig av administrative maler-versjonen til mappen: **C:\Programfiler (x86)\Microsoft Gruppepolicy\Windows 10 oktober 2020 Update (20H2)**.</span><span class="sxs-lookup"><span data-stu-id="94519-151">Navigate, depending on the Administrative Templates version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 October 2020 Update (20H2)**.</span></span>
4. <span data-ttu-id="94519-152">Gi nytt **navn til Policydefinisjoner-mappen** i banen ovenfor til **PolicyDefinitions**.</span><span class="sxs-lookup"><span data-stu-id="94519-152">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5. <span data-ttu-id="94519-153">Kopier **PolicyDefinitions-mappen** til sysvol-ressursen som standard plassert på **C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="94519-153">Copy the **PolicyDefinitions** folder to your SYSVOL share, by default located at **C:\Windows\SYSVOL\domain\Policies**.</span></span>
   - <span data-ttu-id="94519-154">Hvis du planlegger å bruke et sentralt policylager for hele domenet, legger du til innholdet i PolicyDefinitions der.</span><span class="sxs-lookup"><span data-stu-id="94519-154">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6. <span data-ttu-id="94519-155">Hvis du har flere domenekontrollere, venter du til SYSVOL replikerer for at policyene skal være tilgjengelige.</span><span class="sxs-lookup"><span data-stu-id="94519-155">In case you have several Domain Controllers, wait for SYSVOL to replicate for the policies to be available.</span></span> <span data-ttu-id="94519-156">Denne fremgangsmåten fungerer også for alle fremtidige versjoner av de administrative malene.</span><span class="sxs-lookup"><span data-stu-id="94519-156">This procedure will work for any future version of the Administrative Templates as well.</span></span>

<span data-ttu-id="94519-157">På dette tidspunktet skal du kunne se policyen Aktivere automatisk **MDM-registrering** ved hjelp av standard Azure AD-legitimasjon som er tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="94519-157">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

## <a name="related-content"></a><span data-ttu-id="94519-158">Beslektet innhold</span><span class="sxs-lookup"><span data-stu-id="94519-158">Related content</span></span>

<span data-ttu-id="94519-159">[Synkroniser domenebrukere Microsoft 365](manage-domain-users.md) (artikkel)</span><span class="sxs-lookup"><span data-stu-id="94519-159">[Synchronize domain users to Microsoft 365](manage-domain-users.md) (article)</span></span>\
<span data-ttu-id="94519-160">[Opprette en gruppe i administrasjonssenteret](../admin/create-groups/create-groups.md) (artikkel)</span><span class="sxs-lookup"><span data-stu-id="94519-160">[Create a group in the admin center](../admin/create-groups/create-groups.md) (article)</span></span>\
<span data-ttu-id="94519-161">[Opplæring: Konfigurere hybrid Azure Active Directory for administrerte domener](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (artikkel)</span><span class="sxs-lookup"><span data-stu-id="94519-161">[Tutorial: Configure hybrid Azure Active Directory join for managed domains](/azure/active-directory/devices/hybrid-azuread-join-managed-domains.md) (article)</span></span>