---
title: Konfigurere Windows enheter for Microsoft 365 Business Premium brukere
f1.keywords:
- CSH
ms.author: sharik
author: skjerland
manager: scotv
audience: Admin
ms.topic: article
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
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
- okr_smb
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Lær hvordan du konfigurerer Windows enheter som kjører Windows 10 Pro for Microsoft 365 Business Premium, slik at sentralisert administrasjon og sikkerhetskontroller aktiveres.
ms.openlocfilehash: 3e268d81ff6fb7113b7e0b0fe5d0545ff5c72b1e
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/06/2021
ms.locfileid: "52244780"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="70361-103">Konfigurere Windows enheter for Microsoft 365 Business Premium brukere</span><span class="sxs-lookup"><span data-stu-id="70361-103">Set up Windows devices for Microsoft 365 Business Premium users</span></span>

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a><span data-ttu-id="70361-104">Forutsetninger for å konfigurere Windows enheter for Microsoft 365 Business Premium brukere</span><span class="sxs-lookup"><span data-stu-id="70361-104">Prerequisites for setting up Windows devices for Microsoft 365 Business Premium users</span></span>

<span data-ttu-id="70361-105">Før du kan konfigurere Windows-enheter for Microsoft 365 Business Premium-brukere, må du kontrollere at alle Windows-enhetene kjører Windows 10 Pro, versjon 1703 (Creators Update).</span><span class="sxs-lookup"><span data-stu-id="70361-105">Before you can set up Windows devices for Microsoft 365 Business Premium users, make sure all the Windows devices are running Windows 10 Pro, version 1703 (Creators Update).</span></span> <span data-ttu-id="70361-106">Windows 10 Pro er en forutsetning for å distribuere Windows 10 Business, som er et sett med skytjenester og funksjoner for enhetsbehandling som utfyller Windows 10 Pro og aktiverer sentralisert administrasjon og sikkerhetskontroller for Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="70361-106">Windows 10 Pro is a prerequisite for deploying Windows 10 Business, which is a set of cloud services and device management capabilities that complement Windows 10 Pro and enable the centralized management and security controls of Microsoft 365 Business Premium.</span></span>
  
<span data-ttu-id="70361-107">Hvis du Windows enheter som kjører Windows 7 Pro, Windows 8 Pro eller Windows 8.1 Pro, gir Microsoft 365 Business Premium-abonnementet deg tilgang til en Windows 10 oppgradering.</span><span class="sxs-lookup"><span data-stu-id="70361-107">If you have Windows devices running Windows 7 Pro, Windows 8 Pro, or Windows 8.1 Pro, your Microsoft 365 Business Premium subscription entitles you to a Windows 10 upgrade.</span></span>
  
<span data-ttu-id="70361-108">Hvis du vil ha mer informasjon om hvordan du oppgraderer Windows-enheter til Windows 10 Pro Creators Update, følger du fremgangsmåten i dette emnet: [Oppgradere Windows-enheter til Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span><span class="sxs-lookup"><span data-stu-id="70361-108">For more information on how to upgrade Windows devices to Windows 10 Pro Creators Update, follow the steps in this topic: [Upgrade Windows devices to Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).</span></span>
  
<span data-ttu-id="70361-109">Se [Kontrollere at enheten er koblet til Azure AD](#verify-the-device-is-connected-to-azure-ad) for å bekrefte at du har oppgraderingen, eller for å sikre at oppgraderingen fungerte.</span><span class="sxs-lookup"><span data-stu-id="70361-109">See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to verify you have the upgrade, or to make sure the upgrade worked.</span></span>

<span data-ttu-id="70361-110">Se en kort video om hvordan du kobler Windows til Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="70361-110">Watch a short video about connecting Windows to Microsoft 365.</span></span><br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

<span data-ttu-id="70361-111">Hvis du synes at denne videoen er nyttig, kan du se den [fullstendige opplæringsserien for små bedrifter og de som er nybegynnere i Microsoft 365](../business-video/index.yml).</span><span class="sxs-lookup"><span data-stu-id="70361-111">If you found this video helpful, check out the [complete training series for small businesses and those new to Microsoft 365](../business-video/index.yml).</span></span>
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a><span data-ttu-id="70361-112">Slå sammen Windows 10-enheter med organisasjonens Azure AD</span><span class="sxs-lookup"><span data-stu-id="70361-112">Join Windows 10 devices to your organization's Azure AD</span></span>

<span data-ttu-id="70361-113">Når alle Windows-enheter i organisasjonen enten har blitt oppgradert til Windows 10 Pro Creators Update eller allerede kjører Windows 10 Pro Creators Update, kan du bli med i disse enhetene til organisasjonens Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="70361-113">When all Windows devices in your organization have either been upgraded to Windows 10 Pro Creators Update or are already running Windows 10 Pro Creators Update, you can join these devices to your organization's Azure Active Directory.</span></span> <span data-ttu-id="70361-114">Når enhetene er koblet til, oppgraderes de automatisk til Windows 10 Business, som er en del av Microsoft 365 Business Premium abonnementet.</span><span class="sxs-lookup"><span data-stu-id="70361-114">Once the devices are joined, they'll be automatically upgraded to Windows 10 Business, which is part of your Microsoft 365 Business Premium subscription.</span></span>
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a><span data-ttu-id="70361-115">Hvis du har en helt ny eller nylig oppgradert Windows 10 Pro-enhet</span><span class="sxs-lookup"><span data-stu-id="70361-115">For a brand new, or newly upgraded, Windows 10 Pro device</span></span>

<span data-ttu-id="70361-116">Hvis du har en helt ny enhet som kjører Windows 10 Pro Creators Update eller en enhet som ble oppgradert til Windows 10 Pro Creators Update, men ikke har gått gjennom konfigurasjon for Windows 10-enheter, følger du disse trinnene.</span><span class="sxs-lookup"><span data-stu-id="70361-116">For a brand new device running Windows 10 Pro Creators Update, or for a device that was upgraded to Windows 10 Pro Creators Update but has not gone through Windows 10 device setup, follow these steps.</span></span>
  
1. <span data-ttu-id="70361-117">Gå gjennom konfigurasjonen for Windows 10-enheter frem til **Hvordan vil du konfigurere?**-siden.</span><span class="sxs-lookup"><span data-stu-id="70361-117">Go through Windows 10 device setup until you get to the **How would you like to set up?** page.</span></span> 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. <span data-ttu-id="70361-119">Her velger du **Konfigurer for en organisasjon, og** deretter skriver du inn brukernavnet og passordet for Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="70361-119">Here, choose **Set up for an organization** and then enter your username and password for Microsoft 365 Business Premium.</span></span> 
    
3. <span data-ttu-id="70361-120">Fullfør konfigurasjonen for Windows 10-enheter.</span><span class="sxs-lookup"><span data-stu-id="70361-120">Finish Windows 10 device setup.</span></span>
    
   <span data-ttu-id="70361-p103">Når du er ferdig, vil brukeren bli koblet til organisasjonens Azure AD. Se [Kontroller at enheten er koblet til Azure AD](#verify-the-device-is-connected-to-azure-ad) for å være sikker.</span><span class="sxs-lookup"><span data-stu-id="70361-p103">Once you're done, the user will be connected to your organization's Azure AD. See [Verify the device is connected to Azure AD](#verify-the-device-is-connected-to-azure-ad) to make sure.</span></span> 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a><span data-ttu-id="70361-123">Hvis du har en enhet som allerede er konfigurert og kjører Windows 10 Pro</span><span class="sxs-lookup"><span data-stu-id="70361-123">For a device already set up and running Windows 10 Pro</span></span>

 <span data-ttu-id="70361-124">**Koble brukere til Azure AD:**</span><span class="sxs-lookup"><span data-stu-id="70361-124">**Connect users to Azure AD:**</span></span>
  
1. <span data-ttu-id="70361-125">I brukerens Windows-PC som kjører Windows 10 Pro, versjon 1703 (Creators Update) (se [forhåndskrav](pre-requisites-for-data-protection.md)), klikk på Windows-logoen og deretter på Innstillinger-ikonet.</span><span class="sxs-lookup"><span data-stu-id="70361-125">In your user's Windows PC, that is running Windows 10 Pro, version 1703 (Creators Update) (see [pre-requisites](pre-requisites-for-data-protection.md)), click the Windows logo, and then the Settings icon.</span></span>
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. <span data-ttu-id="70361-127">Gå til **Kontoer** i **Innstillinger**.</span><span class="sxs-lookup"><span data-stu-id="70361-127">In **Settings**, go to **Accounts**.</span></span>
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. <span data-ttu-id="70361-129">Klikk på **Tilgang jobb eller skole**\> på **Din informasjon**-side.</span><span class="sxs-lookup"><span data-stu-id="70361-129">On **Your info** page, click **Access work or school** \> **Connect**.</span></span>
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. <span data-ttu-id="70361-131">Velg **Legg denne enheten til Azure Active Directory** under **Alternative handlinger** på **Konfigurer en arbeids- eller skolekonto** -dialogboksen.</span><span class="sxs-lookup"><span data-stu-id="70361-131">On the **Set up a work or school account** dialog, under **Alternate actions**, choose **Join this device to Azure Active Directory**.</span></span>
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. <span data-ttu-id="70361-133">Skriv inn **jobb-** eller skolekontoen neste på siden La oss få deg logget \> **på.**</span><span class="sxs-lookup"><span data-stu-id="70361-133">On the **Let's get you signed in** page, enter your work or school account \> **Next**.</span></span>
  
   <span data-ttu-id="70361-134">Skriv inn **passordet** Logg på på Skriv inn \> **passord-siden.**</span><span class="sxs-lookup"><span data-stu-id="70361-134">On the **Enter password** page, enter your password \> **Sign in**.</span></span>
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. <span data-ttu-id="70361-136">Kontroller at **informasjonen er** riktig på kontroller at dette er organisasjonens side, og velg Bli **med**.</span><span class="sxs-lookup"><span data-stu-id="70361-136">On the **Make sure this is your organization** page, verify that the information is correct, and choose **Join**.</span></span>
  
   <span data-ttu-id="70361-137">På **You're all set!**</span><span class="sxs-lookup"><span data-stu-id="70361-137">On the **You're all set!**</span></span> <span data-ttu-id="70361-138">side, chosse **Done**.</span><span class="sxs-lookup"><span data-stu-id="70361-138">page, chosse **Done**.</span></span>
  
   ![Velg Bli med på skjermen Kontroller at dette er organisasjonen](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
<span data-ttu-id="70361-140">Hvis du har lastet opp filer til OneDrive for Business, synkroniser dem tilbake.</span><span class="sxs-lookup"><span data-stu-id="70361-140">If you uploaded files to OneDrive for Business, sync them back down.</span></span> <span data-ttu-id="70361-141">Hvis du brukte et tredjepartsverktøy til å overføre profil og filer, synkroniserer du også disse til den nye profilen.</span><span class="sxs-lookup"><span data-stu-id="70361-141">If you used a third-party tool to migrate profile and files, also sync those to the new profile.</span></span>
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a><span data-ttu-id="70361-142">Kontroller at enheten er koblet til Azure AD</span><span class="sxs-lookup"><span data-stu-id="70361-142">Verify the device is connected to Azure AD</span></span>

<span data-ttu-id="70361-143">Hvis du vil bekrefte synkroniseringsstatusen, går du til **jobb- eller skolesiden i** **Innstillinger** og velger området Tilkoblet **_** _ for å vise knappene \<organization name\> **Informasjon** og **Koble fra**.</span><span class="sxs-lookup"><span data-stu-id="70361-143">To verify your sync status, on the **Access work or school** page in **Settings**, select the **Connected to** _ \<organization name\> _ area to expose the buttons **Info** and **Disconnect**.</span></span> <span data-ttu-id="70361-144">Velg **Informasjon for** å få synkroniseringsstatusen.</span><span class="sxs-lookup"><span data-stu-id="70361-144">Choose **Info** to get your synchronization status.</span></span> 
  
<span data-ttu-id="70361-145">Velg **Synkroniser på** Synkroniseringsstatus-siden **for** å få de nyeste policyene for administrasjon av mobilenheter til PC-en.</span><span class="sxs-lookup"><span data-stu-id="70361-145">On the **Sync status** page, choose **Sync** to get the latest mobile device management policies onto the PC.</span></span>
  
<span data-ttu-id="70361-146">Hvis du vil begynne å Microsoft 365 Business Premium kontoen, går  du til startknappen Windows, høyreklikker det gjeldende kontobildet, og deretter **bytter du konto**.</span><span class="sxs-lookup"><span data-stu-id="70361-146">To start using the Microsoft 365 Business Premium account, go to the Windows **Start** button, right-click your current account picture, and then **Switch account**.</span></span> <span data-ttu-id="70361-147">Logg på ved hjelp av organisasjons e-post og passord.</span><span class="sxs-lookup"><span data-stu-id="70361-147">Sign in by using your organization email and password.</span></span>
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a><span data-ttu-id="70361-149">Kontroller at PC-en er oppgradert til Windows 10 Business</span><span class="sxs-lookup"><span data-stu-id="70361-149">Verify the PC is upgraded to Windows 10 Business</span></span>

<span data-ttu-id="70361-150">Kontroller at Azure AD-Windows 10 er oppgradert til Windows 10 Business som en del av Microsoft 365 Business Premium abonnementet.</span><span class="sxs-lookup"><span data-stu-id="70361-150">Verify that your Azure AD joined Windows 10 devices are upgraded to Windows 10 Business as part of your Microsoft 365 Business Premium subscription.</span></span>
  
1. <span data-ttu-id="70361-151">Gå til **Innstillinger** \> **System** \> **Om**.</span><span class="sxs-lookup"><span data-stu-id="70361-151">Go to **Settings** \> **System** \> **About**.</span></span>
    
2. <span data-ttu-id="70361-152">Kontroller at **Versjon** viser **Windows 10 Business**.</span><span class="sxs-lookup"><span data-stu-id="70361-152">Confirm that the **Edition** shows **Windows 10 Business**.</span></span>
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a><span data-ttu-id="70361-154">Neste trinn</span><span class="sxs-lookup"><span data-stu-id="70361-154">Next steps</span></span>

<span data-ttu-id="70361-155">Hvis du vil konfigurere mobile enheter, kan du se Konfigurere mobile enheter [for Microsoft 365 Business Premium](set-up-mobile-devices.md)- Hvis du vil angi policyer for beskyttelse av enheter eller appbeskyttelse, kan du se Administrere Microsoft 365 [for bedrifter](manage.md).</span><span class="sxs-lookup"><span data-stu-id="70361-155">To set up your mobile devices, see [Set up mobile devices for Microsoft 365 Business Premium users](set-up-mobile-devices.md), To set device protection or app protection policies, see [Manage Microsoft 365 for business](manage.md).</span></span>
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a><span data-ttu-id="70361-156">Hvis du vil ha mer informasjon om hvordan du konfigurerer og bruker Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="70361-156">For more on setting up and using Microsoft 365 Business Premium</span></span>

[<span data-ttu-id="70361-157">Microsoft 365 opplæringsvideoer for bedrifter</span><span class="sxs-lookup"><span data-stu-id="70361-157">Microsoft 365 for business training videos</span></span>](../business-video/index.yml)
