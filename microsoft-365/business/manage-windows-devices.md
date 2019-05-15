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
description: Lær hvordan du aktiverer Microsoft 365 å beskytte lokale AD sammen Windows 10 enheter.
ms.openlocfilehash: af0e78ef6e79bfd612b11a16538e7afcd377ffb0
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/15/2019
ms.locfileid: "34071554"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="6828c-103">Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="6828c-103">Enable domain-joined Windows 10 devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="6828c-104">Hvis organisasjonen bruker Windows Server Active Directory på lokaler, kan du definere Microsoft 365 Business til å beskytte Windows 10 enheter, samtidig som du har tilgang til lokale ressurser som krever lokal godkjenning.</span><span class="sxs-lookup"><span data-stu-id="6828c-104">If your organization uses Windows Server Active Directory on-premises, you can set up Microsoft 365 Business to protect your Windows 10 devices, while still maintaining access to on-premises resources that require local authentication.</span></span> <span data-ttu-id="6828c-105">Du kan definere dette ved første synkronisering av Active Directory med Azure Active Directory, etterfulgt av registrering 10 Windows-enheter med Azure AD og melde deg dem for mobilenhet administrasjon av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="6828c-105">You can set this up by first synchronizing your Active Directory with Azure Active Directory, followed by registering the Windows 10 devices with Azure AD and enrolling them for mobile device management by Microsoft 365 Business.</span></span>
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a><span data-ttu-id="6828c-106">Angi domenetilknyttede enheter skal administreres av Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="6828c-106">Set up domain-joined devices to be managed by Microsoft 365 Business</span></span>

<span data-ttu-id="6828c-107">Hvis du vil konfigurere organisasjonens domenetilknyttede enheter til å dra nytte av mulighetene som gis av Azure Active Directory i tillegg til lokale Active Directory, kan du implementere **Hybrid Azure AD koblet enheter**.</span><span class="sxs-lookup"><span data-stu-id="6828c-107">To set up your organization's domain-joined devices to benefit from the capabilities provided by Azure Active Directory in addition to on-premises Active Directory, you can implement **Hybrid Azure AD joined devices**.</span></span> <span data-ttu-id="6828c-108">Dette er enheter som er koblet til både den lokale Active Directory og Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6828c-108">These are devices that are joined both to your on-premises Active Directory and your Azure Active Directory.</span></span> <span data-ttu-id="6828c-109">Hybrid Azure AD koblet enheter kan beskyttet og administreres av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="6828c-109">Hybrid Azure AD joined devices can be protected and managed by Microsoft 365 Business.</span></span> 
  
<span data-ttu-id="6828c-110">Fullfør fremgangsmåten nedenfor for å gjøre Windows 10 enheter Hybrid Azure AD sammen og administreres av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="6828c-110">Complete the steps below to make your Windows 10 devices Hybrid Azure AD joined and managed by Microsoft 365 Business.</span></span>
  
1. <span data-ttu-id="6828c-111">For å synkronisere brukere, grupper og kontakter fra lokal Active Directory til Azure Active Directory, kan du kjøre veiviseren for synkronisering av katalog og Azure Active Directory koble som beskrevet i [konfigurere katalogsynkronisering for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="6828c-111">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure Active Directory Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="6828c-112">Trinnene er nøyaktig den samme for Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="6828c-112">The steps are exactly the same for Microsoft 365 Business.</span></span> 
  
2. <span data-ttu-id="6828c-113">Før du fullfører trinn 3 for å aktivere Windows 10 enheter skal være Hybrid Azure AD sammenføyd, må du kontrollere at du oppfyller følgende forutsetninger:</span><span class="sxs-lookup"><span data-stu-id="6828c-113">Before you complete step 3 to enable Windows 10 devices to be Hybrid Azure AD joined, you need to make sure that you meet the following prerequisites:</span></span>

   - <span data-ttu-id="6828c-114">Du kjører den nyeste versjonen av Azure AD koble.</span><span class="sxs-lookup"><span data-stu-id="6828c-114">You are running the latest version of Azure AD connect.</span></span>

   - <span data-ttu-id="6828c-115">Koble Azure AD har synkronisert alle datamaskinobjekter for enhetene du vil skal være hybrid Azure AD sammen.</span><span class="sxs-lookup"><span data-stu-id="6828c-115">Azure AD connect has synchronized all the computer objects of the devices you want to be hybrid Azure AD joined.</span></span> <span data-ttu-id="6828c-116">Hvis objektene som datamaskinen hører til bestemte organisasjonsenheter (OU), og deretter kontrollerer disse organisasjonsenheter som er angitt for synkronisering i Azure AD koble også.</span><span class="sxs-lookup"><span data-stu-id="6828c-116">If the computer objects belong to specific organizational units (OU), then make sure these OUs are set for synchronization in Azure AD connect as well.</span></span>
    
3. <span data-ttu-id="6828c-117">Registrere eksisterende domenetilknyttede Windows 10 enheter hybrid Azure AD JOIN og registrere dem for mobil enhet management ved Intune (Microsoft 365 Business):</span><span class="sxs-lookup"><span data-stu-id="6828c-117">Register existing domain-joined Windows 10 devices to be hybrid Azure AD Joined and enroll them for mobile device management by Intune (Microsoft 365 Business):</span></span>
    
4. <span data-ttu-id="6828c-118">Følg trinnvise instruksjoner om [hvordan du konfigurerer hybrid Azure Active Directory sammen enheter](https://go.microsoft.com/fwlink/p/?linkid=872870).</span><span class="sxs-lookup"><span data-stu-id="6828c-118">Follow the step by step instructions in [How to configure hybrid Azure Active Directory joined devices](https://go.microsoft.com/fwlink/p/?linkid=872870).</span></span> <span data-ttu-id="6828c-119">Dette vil aktivere synkronisering av lokale Active Directory sammen Windows 10 datamaskiner og gjøre dem klar for sky.</span><span class="sxs-lookup"><span data-stu-id="6828c-119">This will enable the synchronization of your on-premises Active Directory joined Windows 10 computers and make them cloud ready.</span></span>
    
5. <span data-ttu-id="6828c-120">Hvis du vil registrere en Windows 10 enhet for behandling av mobil enhet, kan du se [registrere en Windows 10 enhet med Intune ved hjelp av en gruppepolicy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instruksjoner.</span><span class="sxs-lookup"><span data-stu-id="6828c-120">In order to enroll a Windows 10 device for mobile device management, see [Enroll a Windows 10 device with Intune by using a Group Policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instructions.</span></span> <span data-ttu-id="6828c-121">Du kan angi gruppepolicyen på en lokal datamaskin eller for masseoperasjoner, kan du opprette denne innstillingen for gruppepolicy på domenet-kontrollerserver.</span><span class="sxs-lookup"><span data-stu-id="6828c-121">You can set the Group Policy at a local computer level or for bulk operations, you can create this group policy setting on your domain controller server.</span></span>