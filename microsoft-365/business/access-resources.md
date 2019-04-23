---
title: Access lokale ressurser fra en Azure AD-koblet enheten i Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Lær hvordan du får tilgang til lokale ressurser som linjen Business apps, delte filer og skrivere fra en Active Directory Azure sammen Windows 10 enhet.
ms.openlocfilehash: 212685bc229f519152e69b09d0a745bfac7a38cd
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32276885"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="510bd-103">Access lokale ressurser fra en Azure AD-koblet enheten i Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="510bd-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="510bd-104">Alle Windows 10 enheter som er Azure Active Directory sammen, har tilgang til alle sky-baserte ressurser som Office 365-apps og kan være beskyttet av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="510bd-104">Any Windows 10 device that is Azure Active Directory joined will have access to all cloud-based resources such as your Office 365 apps and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="510bd-105">Hvis du også tillate tilgang til lokale ressurser som linje av Business (LOB) apps, delte filer og skrivere, må du synkronisere lokale Active Directory med Azure Active Directory ved hjelp av [Azure AD-tilkobling](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="510bd-105">To also allow access to on-premises resources like Line Of Business (LOB) apps, file shares, and printers, you must synchronize your on-premises Active Directory with Azure Active Directory by using [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect).</span></span> <span data-ttu-id="510bd-106">Se [Innføring i Enhetsbehandling i Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) for å lære mer.</span><span class="sxs-lookup"><span data-stu-id="510bd-106">See [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) to learn more.</span></span> 
  
## <a name="run-azure-ad-connect"></a><span data-ttu-id="510bd-107">Kjør Azure AD koble</span><span class="sxs-lookup"><span data-stu-id="510bd-107">Run Azure AD Connect</span></span>

<span data-ttu-id="510bd-108">Bruk følgende fremgangsmåte for å aktivere organisasjonens Azure AD koblet enheter til å få tilgang til lokale ressurser.</span><span class="sxs-lookup"><span data-stu-id="510bd-108">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="510bd-109">Kjør veiviseren for Directory-synkronisering for å synkronisere brukere, grupper og kontakter fra lokal Active Directory til Azure Active Directory, og koble til Azure AD som beskrevet i [konfigurere katalogsynkronisering for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="510bd-109">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="510bd-110">Når directory-synkronisering er fullført, kontrollerer du at organisasjonens Windows 10 enheter er Azure AD sammen.</span><span class="sxs-lookup"><span data-stu-id="510bd-110">After the directory synchronization has completed, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="510bd-111">Dette trinnet utføres individuelt på hver Windows-10-enhet.</span><span class="sxs-lookup"><span data-stu-id="510bd-111">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="510bd-112">Se [konfigurere Windows-enheter for forretningsbrukere som Microsoft 365](set-up-windows-devices.md) for detaljer.</span><span class="sxs-lookup"><span data-stu-id="510bd-112">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="510bd-113">Når Windows 10 enhetene er koblet Azure AD, bør hver bruker omstart sine enheter og pålogging med legitimasjonen Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="510bd-113">Once the Windows 10 devices are Azure AD joined, each user should reboot their devices and login with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="510bd-114">Alle enheter har nå tilgang til lokale ressurser også.</span><span class="sxs-lookup"><span data-stu-id="510bd-114">All devices will now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="510bd-115">Det kreves ingen ekstra trinn for å få tilgang til lokale ressurser for Azure AD koblet enheter.</span><span class="sxs-lookup"><span data-stu-id="510bd-115">No additional steps are required to get access to on-premise resources for Azure AD joined devices.</span></span> <span data-ttu-id="510bd-116">Dette er innebygd funksjonalitet som er tilgjengelige i Windows-10.</span><span class="sxs-lookup"><span data-stu-id="510bd-116">This is built-in functionality available in Windows 10.</span></span> 
  
<span data-ttu-id="510bd-117">Hvis organisasjonen ikke er klar til å distribuere i Azure AD sammen enhetskonfigurasjonen som er beskrevet ovenfor, bør du vurdere å installere [Hybrid Azure AD JOIN enhetskonfigurasjon](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="510bd-117">If your organization is not ready to deploy in the Azure AD Joined Device Configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a><span data-ttu-id="510bd-118">Sikkerhetshensyn ved å sammenføye enhetene Windows Azure AD</span><span class="sxs-lookup"><span data-stu-id="510bd-118">Considerations when joining your Windows devices to Azure AD</span></span>

<span data-ttu-id="510bd-119">Hvis du er Azure AD å bli med i en Windows-enhet som tidligere er tilknyttet et domene eller i en arbeidsgruppe, må du ta hensyn til følgende begrensninger:</span><span class="sxs-lookup"><span data-stu-id="510bd-119">If you are Azure AD joining a Windows device that has previously been domain-joined or in a workgroup, you need to consider the following limitations:</span></span>
  
- <span data-ttu-id="510bd-120">Når en enhet Azure AD sammenføyninger, opprettes det en ny bruker uten refererer til en eksisterende profil.</span><span class="sxs-lookup"><span data-stu-id="510bd-120">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="510bd-121">Hvis du vil løse dette problemet, må profiler overføres manuelt.</span><span class="sxs-lookup"><span data-stu-id="510bd-121">To fix this, profiles need to be manually migrated.</span></span> <span data-ttu-id="510bd-122">En brukerprofil inneholder informasjon, for eksempel Favoritter, lokale filer, innstillinger, innstillinger for Start-menyen, osv. Beste fremgangsmåten er å finne et tredjepartsverktøy til å tilordne eksisterende filer og innstillinger til den nye profilen</span><span class="sxs-lookup"><span data-stu-id="510bd-122">A user profile contains information like favorites, local files, browser settings, Start menu settings, etc. A best approach is to find a third-party tool to map existing files and settings to the new profile</span></span>
    
- <span data-ttu-id="510bd-123">Hvis enheten bruker gruppe gruppepolicyobjekter (GPO), kanskje noen gruppepolicyobjekter har ikke en sammenlignbar [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) i Intune.</span><span class="sxs-lookup"><span data-stu-id="510bd-123">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="510bd-124">Kjør [MMAT-verktøyet](https://www.microsoft.com/download/details.aspx?id=45520) for å finne tilsvarende CSP for eksisterende gruppepolicyobjekter.</span><span class="sxs-lookup"><span data-stu-id="510bd-124">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span> 
    
- <span data-ttu-id="510bd-125">Brukere vil ikke kunne godkjenne til programmer som avhenger av Active Directory-autentisering.</span><span class="sxs-lookup"><span data-stu-id="510bd-125">Users will not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="510bd-126">Dette vurdere å bruke et eldre program og vurdere å oppdatere til et program som bruker moderne godkjenning hvis det er mulig å forholde seg til.</span><span class="sxs-lookup"><span data-stu-id="510bd-126">To deal with this evaluate using a legacy app and consider updating to an app that uses modern Auth if possible.</span></span>
    
- <span data-ttu-id="510bd-127">Active Directory-gjenkjenning for skriveren vil ikke fungere.</span><span class="sxs-lookup"><span data-stu-id="510bd-127">Active Directory printer discovery will not work.</span></span> <span data-ttu-id="510bd-128">Hvis du vil løse dette problemet, gir direkte skriverbaner for alle brukere eller dra nytte av [Hybrid sky utskrift](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="510bd-128">To fix this, provide direct printer paths for all users or leverage [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
    

