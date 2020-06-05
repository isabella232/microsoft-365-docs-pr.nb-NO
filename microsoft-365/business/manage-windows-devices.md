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
ms.openlocfilehash: 857651081fb10856d28dd419333ebef655388407
ms.sourcegitcommit: e6e704cbd9a50fc7db1e6a0cf5d3f8c6cbb94363
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/04/2020
ms.locfileid: "44564954"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a><span data-ttu-id="87571-103">Aktivere domeneblede Windows 10-enheter som skal administreres av Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="87571-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business Premium</span></span>

<span data-ttu-id="87571-104">Hvis organisasjonen bruker lokal Windows Server Active Directory, kan du konfigurere Microsoft 365 Business Premium til å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgangen til lokale ressurser som krever lokal godkjenning.</span><span class="sxs-lookup"><span data-stu-id="87571-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business Premium to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span>
<span data-ttu-id="87571-105">Hvis du vil konfigurere denne beskyttelsen, kan du implementere **Hybrid Azure AD sammenføyde enheter**.</span><span class="sxs-lookup"><span data-stu-id="87571-105">To set up this protection, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="87571-106">Disse enhetene er koblet til både den lokale Active Directory og Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="87571-106">These devices are joined to both your on-premises Active Directory and your Azure Active Directory.</span></span>

<span data-ttu-id="87571-107">Denne videoen beskriver fremgangsmåten for hvordan du konfigurerer dette for det vanligste scenariet, som også er beskrevet i trinnene som følger.</span><span class="sxs-lookup"><span data-stu-id="87571-107">This video describes the steps for how to set this up for the most common scenario, which is also detailed in the steps that follow.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a><span data-ttu-id="87571-108">Før du kommer i gang, må du sørge for at du fullfører disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="87571-108">Before you get started, make sure you complete these steps:</span></span>
- <span data-ttu-id="87571-109">Synkroniser brukere til Azure AD med Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="87571-109">Synchronize users to Azure AD with Azure AD Connect.</span></span>
- <span data-ttu-id="87571-110">Fullfør Azure AD Connect Organizational Unit (OU)-synkronisering.</span><span class="sxs-lookup"><span data-stu-id="87571-110">Complete Azure AD Connect Organizational Unit (OU) sync.</span></span>
- <span data-ttu-id="87571-111">Kontroller at alle domenebrukerne du synkroniserer, har lisenser til Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="87571-111">Make sure all the domain users you sync have licenses to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="87571-112">Se [Synkronisere domenebrukere til Microsoft](manage-domain-users.md) for fremgangsmåten.</span><span class="sxs-lookup"><span data-stu-id="87571-112">See [Synchronize domain users to Microsoft](manage-domain-users.md) for the steps.</span></span>

## <a name="1-verify-mdm-authority-in-intune"></a><span data-ttu-id="87571-113">1. Kontroller MDM-myndigheten i Intune</span><span class="sxs-lookup"><span data-stu-id="87571-113">1. Verify MDM Authority in Intune</span></span>

<span data-ttu-id="87571-114">Gå til portal.azure.com og øverst på siden søker du etter Intune.</span><span class="sxs-lookup"><span data-stu-id="87571-114">Go to portal.azure.com and on the top of the page search for Intune.</span></span>
<span data-ttu-id="87571-115">Velg **Enhetsregistrering** på Siden Microsoft Intune, og kontroller at **MDM-myndighet** er Intune på **Siden Microsoft** **Intune.**</span><span class="sxs-lookup"><span data-stu-id="87571-115">On the Microsoft Intune page, select **Device enrollment** and on the **Overview** page make sure **MDM authority** is **Intune**.</span></span>

- <span data-ttu-id="87571-116">Hvis **MDM-myndighet** er **Ingen**, klikker du **MDM-myndigheten** for å sette den til **Intune**.</span><span class="sxs-lookup"><span data-stu-id="87571-116">If **MDM authority** is **None**, click the **MDM authority** to set it to **Intune**.</span></span>
- <span data-ttu-id="87571-117">Hvis **MDM-myndighet** er **Microsoft Office 365**, går du til **Enheter**  >  **Registrer enheter** og bruker dialogboksen Legg til **MDM-myndighet** til høyre for å legge til **Intune MDM-myndighet** (dialogboksen **Legg til MDM Authority** er bare tilgjengelig hvis **MDM Authority** er satt til Microsoft Office 365).</span><span class="sxs-lookup"><span data-stu-id="87571-117">If **MDM authority** is **Microsoft Office 365**,go to **Devices** > **Enroll devices** and use the **Add MDM authority** dialog on the right to add **Intune MDM** authority (the **Add MDM Authority** dialog is only available if the **MDM Authority** is set to Microsoft Office 365).</span></span>

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a><span data-ttu-id="87571-118">2. Kontroller at Azure AD er aktivert for sammenføyning av datamaskiner</span><span class="sxs-lookup"><span data-stu-id="87571-118">2. Verify Azure AD is enabled for joining computers</span></span>

- <span data-ttu-id="87571-119">Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> på, og velg **Azure Active Directory** (velg Vis alle hvis Azure Active Directory ikke er synlig) i listen over **administrasjonssentre.**</span><span class="sxs-lookup"><span data-stu-id="87571-119">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select **Azure Active Directory** (select Show all if Azure Active Directory is not visible) in the **Admin centers** list.</span></span> 
- <span data-ttu-id="87571-120">Gå til **Azure Active Directory** i **administrasjonssenteret**for Azure Active Directory , velg **Enheter** og deretter **Enhetsinnstillinger**.</span><span class="sxs-lookup"><span data-stu-id="87571-120">In the **Azure Active Directory admin center**, go to **Azure Active Directory** , choose **Devices** and then **Device settings**.</span></span>
- <span data-ttu-id="87571-121">Kontroller at**brukere kan koble enheter til Azure AD** er aktivert</span><span class="sxs-lookup"><span data-stu-id="87571-121">Verify**Users may join devices to Azure AD** is enabled</span></span> 
    1. <span data-ttu-id="87571-122">Hvis du vil aktivere alle brukere, setter du til **Alle**.</span><span class="sxs-lookup"><span data-stu-id="87571-122">To enable all users, set to **All**.</span></span>
    2. <span data-ttu-id="87571-123">Hvis du vil aktivere bestemte brukere, setter du til **Valgt** for å aktivere en bestemt gruppe brukere.</span><span class="sxs-lookup"><span data-stu-id="87571-123">To enable specific users, set to **Selected** to enable a specific group of users.</span></span>
        - <span data-ttu-id="87571-124">Legg til de ønskede domenebrukerne som er synkronisert i Azure AD i en [sikkerhetsgruppe](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="87571-124">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        - <span data-ttu-id="87571-125">Velg **Velg grupper** for å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.</span><span class="sxs-lookup"><span data-stu-id="87571-125">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a><span data-ttu-id="87571-126">3. Kontroller at Azure AD er aktivert for MDM</span><span class="sxs-lookup"><span data-stu-id="87571-126">3. Verify Azure AD is enabled for MDM</span></span>

- <span data-ttu-id="87571-127">Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> på, og velg **Endepunktsbehandler**t (velg **Vis alt** hvis **Endpoint Manager** ikke er synlig)</span><span class="sxs-lookup"><span data-stu-id="87571-127">Go to the admin center at <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a>  and select select **Endpoint Managemen**t (select **Show all** if **Endpoint Manager** is not visible)</span></span>
- <span data-ttu-id="87571-128">Gå til **Enheter**Automatisk registrering av Windows **Microsoft Endpoint Manager admin center**  >  **Windows**  >  **Windows-registrering**  >  **Automatic Enrollment**i administrasjonssenteret for Microsoft Endpoint Manager .</span><span class="sxs-lookup"><span data-stu-id="87571-128">In the **Microsoft Endpoint Manager admin center**, go to **Devices** > **Windows** > **Windows Enrollment** > **Automatic Enrollment**.</span></span>
- <span data-ttu-id="87571-129">Kontroller at MDM-brukeromfang er aktivert.</span><span class="sxs-lookup"><span data-stu-id="87571-129">Verify MDM user scope is enabled.</span></span>

    1. <span data-ttu-id="87571-130">Hvis du vil registrere alle datamaskiner, kan du sette til **Alle** for å registrere alle brukerdatamaskiner som er koblet til Azure AD og nye datamaskiner når brukerne legger til en arbeidskonto i Windows.</span><span class="sxs-lookup"><span data-stu-id="87571-130">To enroll all computers, set to **All** to automatically enroll all user computers that are joined to Azure AD and new computers  when the users add a work account to Windows.</span></span>
    2. <span data-ttu-id="87571-131">Sett til **Noen** for å registrere datamaskinene til en bestemt gruppe brukere.</span><span class="sxs-lookup"><span data-stu-id="87571-131">Set to **Some** to enroll the computers of a specific group of users.</span></span>
        -  <span data-ttu-id="87571-132">Legg til de ønskede domenebrukerne som er synkronisert i Azure AD i en [sikkerhetsgruppe](../admin/create-groups/create-groups.md).</span><span class="sxs-lookup"><span data-stu-id="87571-132">Add the desired domain users synced in Azure AD to a [security group](../admin/create-groups/create-groups.md).</span></span>
        -  <span data-ttu-id="87571-133">Velg **Velg grupper** for å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.</span><span class="sxs-lookup"><span data-stu-id="87571-133">Choose **Select groups** to enable MDM user scope for that security group.</span></span>

## <a name="4-set-up-service-connection-point-scp"></a><span data-ttu-id="87571-134">4. Konfigurere tjenestetilkoblingspunkt (SCP)</span><span class="sxs-lookup"><span data-stu-id="87571-134">4. Set up Service connection point (SCP)</span></span>

<span data-ttu-id="87571-135">Disse trinnene er forenklet fra [å konfigurere hybrid azure AD-sammenføyning](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span><span class="sxs-lookup"><span data-stu-id="87571-135">These steps are simplified from [configure hybrid azure AD join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join).</span></span> <span data-ttu-id="87571-136">For å fullføre trinnene må du bruke Azure AD Connect og Microsoft 365 Business Premium globale administrator og Active Directory admin passord.</span><span class="sxs-lookup"><span data-stu-id="87571-136">To complete the steps you need to use Azure AD Connect and your Microsoft 365 Business Premium global admin and Active Directory admin passwords.</span></span>

1.  <span data-ttu-id="87571-137">Start Azure AD Connect, og velg deretter **Konfigurer**.</span><span class="sxs-lookup"><span data-stu-id="87571-137">Start Azure AD Connect, and then select **Configure**.</span></span>
2.  <span data-ttu-id="87571-138">Velg **Konfigurer enhetsalternativer på**Flere **oppgaver-siden,** og velg deretter **Neste**.</span><span class="sxs-lookup"><span data-stu-id="87571-138">On the **Additional tasks**  page, select **Configure device options**, and then select **Next**.</span></span>
3.  <span data-ttu-id="87571-139">Velg **Neste**på **Oversikt-siden.**</span><span class="sxs-lookup"><span data-stu-id="87571-139">On the **Overview** page, select **Next**.</span></span>
4.  <span data-ttu-id="87571-140">Angi legitimasjonen til en global administrator for Microsoft 365 Business Premium på siden **Koble til Azure AD.**</span><span class="sxs-lookup"><span data-stu-id="87571-140">On the **Connect to Azure AD** page, enter the credentials of a global administrator for Microsoft 365 Business Premium.</span></span>
5.  <span data-ttu-id="87571-141">Velg **Konfigurer Hybrid Azure AD-sammenføyning på**siden **Enhetsalternativer,** og velg deretter **Neste**.</span><span class="sxs-lookup"><span data-stu-id="87571-141">On the **Device options** page, select **Configure Hybrid Azure AD join**, and then select **Next**.</span></span>
6.  <span data-ttu-id="87571-142">Fullfør **SCP** følgende trinn for hver skog der du vil at Azure AD Connect skal konfigurere SCP, fullføre følgende trinn for hver skog der du vil at Azure AD Connect skal konfigurere SCP, fullføre følgende trinn, og velg deretter **Neste:**</span><span class="sxs-lookup"><span data-stu-id="87571-142">On the **SCP** page, for each forest where you want Azure AD Connect to configure the SCP, complete the following steps, and then select **Next**:</span></span>
    - <span data-ttu-id="87571-143">Merk av i boksen ved siden av skogsnavnet.</span><span class="sxs-lookup"><span data-stu-id="87571-143">Check the box beside the forest name.</span></span> <span data-ttu-id="87571-144">Skogen skal være ad-domenenavnet ditt.</span><span class="sxs-lookup"><span data-stu-id="87571-144">The forest should be your AD domain name.</span></span>
    - <span data-ttu-id="87571-145">Åpne rullegardinlisten under **Godkjenningstjeneste-kolonnen,** og velg samsvarende domenenavn (det bør bare være ett alternativ).</span><span class="sxs-lookup"><span data-stu-id="87571-145">Under the **Authentication Service** column, open the dropdown and select matching domain name (there should only be one only option).</span></span>
    - <span data-ttu-id="87571-146">Velg **Legg til** for å angi legitimasjonen for domeneadministrator.</span><span class="sxs-lookup"><span data-stu-id="87571-146">Select **Add** to enter the domain administrator credentials.</span></span>  
7.  <span data-ttu-id="87571-147">Velg bare Windows 10 eller senere domenet som er sammenkoblet på siden **Enhetsoperativsystemer.**</span><span class="sxs-lookup"><span data-stu-id="87571-147">On the **Device operating systems** page, select Windows 10 or later domain-joined devices only.</span></span>
8.  <span data-ttu-id="87571-148">Velg **Konfigurer**på siden **Klar til å konfigurere.**</span><span class="sxs-lookup"><span data-stu-id="87571-148">On the **Ready to configure** page, select **Configure**.</span></span>
9.  <span data-ttu-id="87571-149">Velg **Avslutt**på siden **Konfigurasjon fullført.**</span><span class="sxs-lookup"><span data-stu-id="87571-149">On the **Configuration complete** page, select **Exit**.</span></span>


## <a name="5-create-a-gpo-for-intune-enrollment--admx-method"></a><span data-ttu-id="87571-150">5. Opprett et gruppepolicyobjekt for Intune-registrering – ADMX-metoden</span><span class="sxs-lookup"><span data-stu-id="87571-150">5. Create a GPO for Intune Enrollment – ADMX method</span></span>

<span data-ttu-id="87571-151">Bruke. ADMX-malfilen.</span><span class="sxs-lookup"><span data-stu-id="87571-151">Use .ADMX template file.</span></span>

1.  <span data-ttu-id="87571-152">Logg deg på AD-server, søk og åpne **Gruppepolicybehandling**for Server  >  **Manager-verktøy**  >  **Group Policy Management**.</span><span class="sxs-lookup"><span data-stu-id="87571-152">Log on to AD server, search and open **Server Manager** > **Tools** > **Group Policy Management**.</span></span>
2.  <span data-ttu-id="87571-153">Velg domenenavnet ditt under **Domener,** og høyreklikk **Gruppepolicyobjekter** for å velge **Ny**.</span><span class="sxs-lookup"><span data-stu-id="87571-153">Select your domain name under **Domains** and right-click **Group Policy Objects** to select **New**.</span></span>
3.  <span data-ttu-id="87571-154">Gi det nye gruppepolicyobjektet et navn, for eksempel "*Cloud_Enrollment*" og velg deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="87571-154">Give the new GPO an name, for example “*Cloud_Enrollment*” and then select **OK**.</span></span>
4.  <span data-ttu-id="87571-155">Høyreklikk det nye Gruppepolicyobjektet under **Gruppepolicyobjekter,** og velg **Rediger**.</span><span class="sxs-lookup"><span data-stu-id="87571-155">Right-click the new GPO under **Group Policy Objects** and select **Edit**.</span></span>
5.  <span data-ttu-id="87571-156">I **redigeringsprogrammet for gruppepolicybehandling**går du til Administrative maler for **Computer Configuration**  >  **Policies**  >  **datamaskinkonfigurasjonspolicyer**  >  **Windows-komponenter**  >  **MDM**.</span><span class="sxs-lookup"><span data-stu-id="87571-156">In the **Group Policy Management Editor**, go to **Computer Configuration** > **Policies** > **Administrative Templates** > **Windows Components** > **MDM**.</span></span>
6. <span data-ttu-id="87571-157">Høyreklikk **Aktiver automatisk MDM-registrering ved hjelp av standard Azure AD-legitimasjon,** og velg deretter **Aktivert**  >  **OK**.</span><span class="sxs-lookup"><span data-stu-id="87571-157">Right-click **Enable automatic MDM enrollment using default Azure AD credentials** and then select **Enabled** > **OK**.</span></span> <span data-ttu-id="87571-158">Lukk redigeringsvinduet.</span><span class="sxs-lookup"><span data-stu-id="87571-158">Close the editor window.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="87571-159">Hvis du ikke ser policyen **Aktiver automatisk MDM-registrering ved hjelp av standard Azure AD-legitimasjon**, kan du se [Få de nyeste administrative malene](#get-the-latest-administrative-templates).</span><span class="sxs-lookup"><span data-stu-id="87571-159">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, see [Get the latest Administrative Templates](#get-the-latest-administrative-templates).</span></span>

## <a name="6-deploy-the-group-policy"></a><span data-ttu-id="87571-160">6. Distribuere gruppepolicyen</span><span class="sxs-lookup"><span data-stu-id="87571-160">6. Deploy the Group Policy</span></span>

1.  <span data-ttu-id="87571-161">I Serverbehandling, under **Domener** > gruppepolicyobjekter, velger du Gruppepolicyobjektene fra trinn 3 ovenfor, for eksempel "Cloud_Enrollment".</span><span class="sxs-lookup"><span data-stu-id="87571-161">In the Server Manager, under **Domains** > Group Policy objects, select the GPO from Step 3 above, for example “Cloud_Enrollment”.</span></span>
2.  <span data-ttu-id="87571-162">Velg **Omfang-fanen** for gruppepolicyobjektet.</span><span class="sxs-lookup"><span data-stu-id="87571-162">Select the **Scope** tab for your GPO.</span></span>
3.  <span data-ttu-id="87571-163">Høyreklikk koblingen til domenet under **Koblinger**i kategorien Omfang i gruppepolicyobjektet.</span><span class="sxs-lookup"><span data-stu-id="87571-163">In the GPO’s Scope tab, right-click the link to the domain under **Links**.</span></span>
4.  <span data-ttu-id="87571-164">Velg **Fremtving** for å distribuere Gruppepolicyobjektet og deretter **OK** i bekreftelsesskjermbildet.</span><span class="sxs-lookup"><span data-stu-id="87571-164">Select **Enforced** to deploy the GPO and then **OK** in the confirmation screen.</span></span>

## <a name="get-the-latest-administrative-templates"></a><span data-ttu-id="87571-165">Få de nyeste administrative malene</span><span class="sxs-lookup"><span data-stu-id="87571-165">Get the latest Administrative Templates</span></span>

<span data-ttu-id="87571-166">Hvis du ikke ser policyen **Aktiver automatisk MDM-registrering ved hjelp av standard Azure AD-legitimasjon**, kan det skyldes at du ikke har ADMX installert for Windows 10, versjon 1803, versjon 1809 eller versjon 1903.</span><span class="sxs-lookup"><span data-stu-id="87571-166">If you do not see the policy **Enable automatic MDM enrollment using default Azure AD credentials**, it may be because you don’t have the ADMX installed for Windows 10, version 1803, version 1809, or version 1903.</span></span> <span data-ttu-id="87571-167">Hvis du vil løse problemet, følger du denne fremgangsmåten (Merk: Den nyeste MDM.admx er bakoverkompatibel):</span><span class="sxs-lookup"><span data-stu-id="87571-167">To fix the issue, follow these steps (Note: the latest MDM.admx is backwards compatible):</span></span>

1.  <span data-ttu-id="87571-168">Last ned: [Administrative maler (ADMX) for Windows 10 mai 2019 Oppdatering (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span><span class="sxs-lookup"><span data-stu-id="87571-168">Download: [Administrative Templates (.admx) for Windows 10 May 2019 Update (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).</span></span>
2.  <span data-ttu-id="87571-169">Installere pakken på den primære domenekontrolleren (PDC).</span><span class="sxs-lookup"><span data-stu-id="87571-169">Install the package on the Primary Domain Controller (PDC).</span></span>
3.  <span data-ttu-id="87571-170">Naviger, avhengig av hvilken versjon til mappen: **C:\Programfiler (x86)\Microsoft gruppepolicy\Windows 10 Mai 2019 Oppdatering (1903) v3**.</span><span class="sxs-lookup"><span data-stu-id="87571-170">Navigate, depending on the version to the folder: **C:\Program Files (x86)\Microsoft Group Policy\Windows 10 May 2019 Update (1903) v3**.</span></span>
4.  <span data-ttu-id="87571-171">Gi nytt navn til **policydefinisjoner-mappen** i banen ovenfor til **PolicyDefinitions**.</span><span class="sxs-lookup"><span data-stu-id="87571-171">Rename the **Policy Definitions** folder in the above path to **PolicyDefinitions**.</span></span>
5.  <span data-ttu-id="87571-172">Kopier **PolicyDefinitions-mappen** til **C:\Windows\SYSVOL\domain\Policies**.</span><span class="sxs-lookup"><span data-stu-id="87571-172">Copy **PolicyDefinitions** folder to **C:\Windows\SYSVOL\domain\Policies**.</span></span> 
    -   <span data-ttu-id="87571-173">Hvis du planlegger å bruke et sentralt policylager for hele domenet, legger du til innholdet i PolicyDefinitions der.</span><span class="sxs-lookup"><span data-stu-id="87571-173">If you plan to use a central policy store for your entire domain, add the contents of PolicyDefinitions there.</span></span>
6.  <span data-ttu-id="87571-174">Start den primære domenekontrolleren på nytt for at policyen skal være tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="87571-174">Restart the Primary Domain Controller for the policy to be available.</span></span> <span data-ttu-id="87571-175">Denne prosedyren vil fungere for alle fremtidige versjoner også.</span><span class="sxs-lookup"><span data-stu-id="87571-175">This procedure will work for any future version as well.</span></span>

<span data-ttu-id="87571-176">På dette tidspunktet bør du kunne se policyen **Aktiver automatisk MDM-registrering ved hjelp av standard Azure AD-legitimasjon** tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="87571-176">At this point you should be able to see the policy **Enable automatic MDM enrollment using default Azure AD credentials** available.</span></span>

