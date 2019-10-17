---
title: Få tilgang til lokale ressurser fra en Azure AD-sammenkoblet enhet i Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Lær hvordan du får tilgang til lokale ressurser som line of Business-apper, delte filressurser og skrivere fra en Azure Active Directory som er koblet til Windows 10-enheten.
ms.openlocfilehash: 92e8ccb99dfece7687c25db84b81fc7bc7158d71
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/17/2019
ms.locfileid: "37574682"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a><span data-ttu-id="c940a-103">Få tilgang til lokale ressurser fra en Azure AD-sammenkoblet enhet i Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="c940a-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business</span></span>

<span data-ttu-id="c940a-104">Alle Windows 10-enheter som er koblet til Azure Active Directory, vil ha tilgang til alle skybaserte ressurser, for eksempel Office 365-appene dine, og kan beskyttes av Microsoft 365 Business.</span><span class="sxs-lookup"><span data-stu-id="c940a-104">Any Windows 10 device that is Azure Active Directory joined will have access to all cloud-based resources such as your Office 365 apps and can be protected by Microsoft 365 Business.</span></span> <span data-ttu-id="c940a-105">Hvis du også vil gi tilgang til lokale ressurser som line of Business (LOB) apps, delte filressurser og skrivere, må du synkronisere lokale Active Directory med Azure Active Directory ved hjelp av [Azure ad-tilkobling](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="c940a-105">To also allow access to on-premises resources like Line Of Business (LOB) apps, file shares, and printers, you must synchronize your on-premises Active Directory with Azure Active Directory by using [Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect).</span></span> 

<span data-ttu-id="c940a-106">Se [innføring i Enhetsbehandling i Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) for å finne ut mer.</span><span class="sxs-lookup"><span data-stu-id="c940a-106">See [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) to learn more.</span></span>
<span data-ttu-id="c940a-107">Trinnene oppsummeres også i avsnittene nedenfor.</span><span class="sxs-lookup"><span data-stu-id="c940a-107">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="c940a-108">Kjør Azure AD-tilkobling</span><span class="sxs-lookup"><span data-stu-id="c940a-108">Run Azure AD Connect</span></span>

<span data-ttu-id="c940a-109">Fullfør fremgangsmåten nedenfor for å aktivere organisasjonens Azure AD ble enheter for å få tilgang til lokale ressurser.</span><span class="sxs-lookup"><span data-stu-id="c940a-109">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>
  
1. <span data-ttu-id="c940a-110">Hvis du vil synkronisere brukere, grupper og kontakter fra lokal Active Directory til Azure Active Directory, kjører du veiviseren for katalogsynkronisering og koble til Azure AD som beskrevet i [Konfigurere katalogsynkronisering for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span><span class="sxs-lookup"><span data-stu-id="c940a-110">To synchronize your users, groups and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).</span></span>
    
2. <span data-ttu-id="c940a-111">Når katalogsynkroniseringen er fullført, må du kontrollere at organisasjonens Windows 10-enheter er Azure AD-tilknyttet.</span><span class="sxs-lookup"><span data-stu-id="c940a-111">After the directory synchronization has completed, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="c940a-112">Dette trinnet gjøres individuelt på hver Windows 10-enhet.</span><span class="sxs-lookup"><span data-stu-id="c940a-112">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="c940a-113">Se [konfigurere Windows-enheter for Microsoft 365 Business-brukere](set-up-windows-devices.md) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="c940a-113">See [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md) for details.</span></span> 
    
3. <span data-ttu-id="c940a-114">Når Windows 10-enhetene er Azure AD-medlem, bør hver bruker starte enhetene sine på nytt og logge på med Microsoft 365 Business-legitimasjonen.</span><span class="sxs-lookup"><span data-stu-id="c940a-114">Once the Windows 10 devices are Azure AD joined, each user should reboot their devices and login with their Microsoft 365 Business credentials.</span></span> <span data-ttu-id="c940a-115">Alle enheter vil nå også ha tilgang til lokale ressurser.</span><span class="sxs-lookup"><span data-stu-id="c940a-115">All devices will now have access to on-premises resources as well.</span></span>
    
<span data-ttu-id="c940a-116">Ingen flere trinn er nødvendig for å få tilgang til lokale ressurser for Azure AD koblet enheter.</span><span class="sxs-lookup"><span data-stu-id="c940a-116">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="c940a-117">Dette er innebygd funksjonalitet som er tilgjengelig i Windows 10.</span><span class="sxs-lookup"><span data-stu-id="c940a-117">This is built-in functionality available in Windows 10.</span></span> 
  
<span data-ttu-id="c940a-118">Hvis organisasjonen ikke er klar til å distribuere i Azure AD sammenkoblet enhet-konfigurasjon som er beskrevet ovenfor, kan du vurdere å konfigurere [hybrid Azure ad sammenkoblet enhetskonfigurasjon](manage-windows-devices.md).</span><span class="sxs-lookup"><span data-stu-id="c940a-118">If your organization is not ready to deploy in the Azure AD Joined Device Configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a><span data-ttu-id="c940a-119">Betraktninger når du kobler Windows-enheter til Azure AD</span><span class="sxs-lookup"><span data-stu-id="c940a-119">Considerations when joining your Windows devices to Azure AD</span></span>

<span data-ttu-id="c940a-120">Hvis du er Azure AD bli med en Windows-enhet som tidligere har vært tilknyttet domenet eller i en arbeidsgruppe, må du vurdere følgende begrensninger:</span><span class="sxs-lookup"><span data-stu-id="c940a-120">If you are Azure AD joining a Windows device that has previously been domain-joined or in a workgroup, you need to consider the following limitations:</span></span>
  
- <span data-ttu-id="c940a-121">Når en enhet Azure AD blir med, oppretter den en ny bruker uten å referere til en eksisterende profil.</span><span class="sxs-lookup"><span data-stu-id="c940a-121">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="c940a-122">For å fikse dette må profilene migreres manuelt.</span><span class="sxs-lookup"><span data-stu-id="c940a-122">To fix this, profiles need to be manually migrated.</span></span> <span data-ttu-id="c940a-123">En brukerprofil inneholder informasjon som favoritter, lokale filer, nettleserinnstillinger, innstillinger for Start-menyen osv. Den beste tilnærmingen er å finne et tredjepartsverktøy for å tilordne eksisterende filer og innstillinger til den nye profilen</span><span class="sxs-lookup"><span data-stu-id="c940a-123">A user profile contains information like favorites, local files, browser settings, Start menu settings, etc. A best approach is to find a third-party tool to map existing files and settings to the new profile</span></span>

- <span data-ttu-id="c940a-124">Hvis enheten brukergruppe policy objekter (GPO), kan noen GPOer ikke ha en sammenlignbar [Konfigurasjonstjeneste leverandør](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) i Intune.</span><span class="sxs-lookup"><span data-stu-id="c940a-124">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="c940a-125">Kjør [MMAT-verktøyet](https://www.microsoft.com/download/details.aspx?id=45520) for å finne sammenlignbare CSPer for eksisterende gruppepolicyobjekter.</span><span class="sxs-lookup"><span data-stu-id="c940a-125">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="c940a-126">Brukere vil ikke kunne godkjennes av programmer som er avhengige av Active Directory-godkjenning.</span><span class="sxs-lookup"><span data-stu-id="c940a-126">Users will not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="c940a-127">For å håndtere dette evaluere ved hjelp av en eldre app og vurdere å oppdatere til en app som bruker moderne Auth hvis mulig.</span><span class="sxs-lookup"><span data-stu-id="c940a-127">To deal with this evaluate using a legacy app and consider updating to an app that uses modern Auth if possible.</span></span>

- <span data-ttu-id="c940a-128">Gjenkjenning av Active Directory-skriveren vil ikke fungere.</span><span class="sxs-lookup"><span data-stu-id="c940a-128">Active Directory printer discovery will not work.</span></span> <span data-ttu-id="c940a-129">Hvis du vil løse dette problemet, kan du angi direkte skriver baner for alle brukere eller utnytte [hybrid Cloud print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span><span class="sxs-lookup"><span data-stu-id="c940a-129">To fix this, provide direct printer paths for all users or leverage [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).</span></span>
