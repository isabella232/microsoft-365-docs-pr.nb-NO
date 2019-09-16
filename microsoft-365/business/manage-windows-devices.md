---
title: Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Lær hvordan du aktiverer Microsoft 365 for å beskytte lokale AD ble koblet til Windows 10-enheter.
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992233"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="78ae0-103">Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="78ae0-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="78ae0-104">Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business for å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgang til lokale ressurser som krever lokal godkjenning.</span><span class="sxs-lookup"><span data-stu-id="78ae0-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="78ae0-105">Du kan konfigurere dette ved først å synkronisere Active Directory med Azure Active Directory, etterfulgt av å registrere Windows 10-enhetene med Azure AD og registrere dem for administrasjon av mobilenheter av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="78ae0-105">You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
<span data-ttu-id="78ae0-106">Følgende video beskriver fremgangsmåten for hvordan du konfigurerer dette for det vanligste scenarioet.</span><span class="sxs-lookup"><span data-stu-id="78ae0-106">The following video details the steps for how to set this up for the most common scenario.</span></span>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="78ae0-107">Konfigurere enheter som er tilknyttet et domene, som skal administreres av Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="78ae0-107">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="78ae0-108">Hvis du vil konfigurere organisasjonens domenetilknyttede enheter til å dra nytte av funksjonene som tilbys av Azure Active Directory i tillegg til lokale Active Directory, kan du implementere **hybrid Azure ad koblet enheter**.</span><span class="sxs-lookup"><span data-stu-id="78ae0-108">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="78ae0-109">Dette er enheter som er koblet både til den lokale Active Directory og Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="78ae0-109">These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory.</span></span> <span data-ttu-id="78ae0-110">Hybrid Azure AD-enheter som er koblet til, kan beskyttes og administreres av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="78ae0-110">Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business.</span></span> 
  
<span data-ttu-id="78ae0-111">Følg fremgangsmåten nedenfor for å gjøre Windows 10-enhetene dine hybrid Azure AD koblet sammen og administrert av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="78ae0-111">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="78ae0-112">Hvis du vil synkronisere brukere, grupper og kontakter fra lokal Active Directory til Azure Active Directory, kjører du veiviseren for katalogsynkronisering og Azure Active Directory Connect som beskrevet i [Konfigurere katalogsynkronisering for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="78ae0-112">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="78ae0-113">Fremgangsmåten er nøyaktig den samme for Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="78ae0-113">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="78ae0-114">Før du fullfører trinn 3 for å aktivere Windows 10-enheter skal hybrid Azure AD ble med, må du kontrollere at du oppfyller følgende forutsetninger:</span><span class="sxs-lookup"><span data-stu-id="78ae0-114">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="78ae0-115">Du kjører den nyeste versjonen av Azure AD-tilkobling.</span><span class="sxs-lookup"><span data-stu-id="78ae0-115">You are running the latest version of Azure AD connect.</span></span>

   - <span data-ttu-id="78ae0-116">Azure AD-tilkobling har synkronisert alle datamaskinobjekter for enhetene du vil skal være hybrid Azure AD ble med.</span><span class="sxs-lookup"><span data-stu-id="78ae0-116">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="78ae0-117">Hvis datamaskinobjektene tilhører bestemte organisasjonsenheter (OU), må du kontrollere at disse organisasjonsenhetene er angitt for synkronisering i Azure AD-tilkobling også.</span><span class="sxs-lookup"><span data-stu-id="78ae0-117">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="78ae0-118">Registrere eksisterende domenetilknyttede Windows 10-enheter for å være hybrid Azure AD ble med og registrere dem for administrasjon av mobile enheter ved Intune (Microsoft 365 Business):</span><span class="sxs-lookup"><span data-stu-id="78ae0-118">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="78ae0-119">Følg de trinnvise instruksjonene i [hvordan du konfigurerer hybrid Azure Active Directory-sammenkoblede enheter](https://go.microsoft.com/fwlink/p/?linkid=872870).</span><span class="sxs-lookup"><span data-stu-id="78ae0-119">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870).</span></span> <span data-ttu-id="78ae0-120">Dette vil gjøre det mulig synkronisering av lokale Active Directory koblet til Windows 10-datamaskiner og gjøre dem Sky klar.</span><span class="sxs-lookup"><span data-stu-id="78ae0-120">This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="78ae0-121">Hvis du vil registrere en Windows 10-enhet for administrasjon av mobile enheter, kan du se [registrere en Windows 10-enhet med Intune ved hjelp av en gruppe policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instruksjoner.</span><span class="sxs-lookup"><span data-stu-id="78ae0-121">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions.</span></span> <span data-ttu-id="78ae0-122">Du kan angi gruppepolicy på et lokalt datamaskinnivå eller for masseoperasjoner, kan du opprette denne gruppepolicyinnstillingen på serveren for domenekontrolleren.</span><span class="sxs-lookup"><span data-stu-id="78ae0-122">You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span>