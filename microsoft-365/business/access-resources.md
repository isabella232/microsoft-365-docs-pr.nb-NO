---
title: Få tilgang til lokale ressurser fra en Azure AD-sammenføyd enhet i Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Lær hvordan du får tilgang til lokale ressurser, for eksempel bransjeapper, delte filressurser og skrivere fra en Azure Active Directory koblet til Windows 10 enhet.
ms.openlocfilehash: 72b3c5ae538cad24fc12e25717dedccb2fdc9017
ms.sourcegitcommit: 4fb1226d5875bf5b9b29252596855a6562cea9ae
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/08/2021
ms.locfileid: "52843326"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a><span data-ttu-id="7fa3c-103">Få tilgang til lokale ressurser fra en Azure AD-sammenføyd enhet i Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="7fa3c-103">Access on-premises resources from an Azure AD-joined device in Microsoft 365 Business Premium</span></span>

<span data-ttu-id="7fa3c-104">Denne artikkelen gjelder for Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-104">This article applies to Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="7fa3c-105">Alle Windows 10 som er Azure Active Directory har tilgang til alle skybaserte ressurser, for eksempel Microsoft 365-appene, og kan beskyttes av Microsoft 365 Business Premium.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-105">Any Windows 10 device that is Azure Active Directory joined has access to all cloud-based resources, such as your Microsoft 365 apps, and can be protected by Microsoft 365 Business Premium.</span></span> <span data-ttu-id="7fa3c-106">Du kan også gi tilgang til lokale ressurser, for eksempel bransjeapper (LOB), delte filressurser og skrivere.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-106">You can also allow access to on-premises resources like line of business (LOB) apps, file shares, and printers.</span></span> <span data-ttu-id="7fa3c-107">Hvis du vil tillate tilgang, bruker [du Azure AD Koble til](/azure/active-directory/connect/active-directory-aadconnect) til å synkronisere den lokale Active Directory med Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-107">To allow access, use [Azure AD Connect](/azure/active-directory/connect/active-directory-aadconnect) to synchronize your on-premises Active Directory with Azure Active Directory.</span></span>

<span data-ttu-id="7fa3c-108">Hvis du vil ha mer informasjon, kan du se Innføring i [enhetsbehandling i Azure Active Directory](/azure/active-directory/device-management-introduction).</span><span class="sxs-lookup"><span data-stu-id="7fa3c-108">To learn more, see [Introduction to device management in Azure Active Directory](/azure/active-directory/device-management-introduction).</span></span>
<span data-ttu-id="7fa3c-109">Trinnene oppsummeres også i avsnittene nedenfor.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-109">The steps are also summarized in the following sections.</span></span>

## <a name="run-azure-ad-connect"></a><span data-ttu-id="7fa3c-110">Kjør Azure AD-Koble til</span><span class="sxs-lookup"><span data-stu-id="7fa3c-110">Run Azure AD Connect</span></span>

<span data-ttu-id="7fa3c-111">Fullfør følgende trinn for å aktivere organisasjonens Azure AD-sammenføyde enheter for å få tilgang til lokale ressurser.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-111">Complete the following steps to enable your organization's Azure AD joined devices to access on-premises resources.</span></span>

1. <span data-ttu-id="7fa3c-112">Hvis du vil synkronisere brukere, grupper og kontakter fra lokale Active Directory til Azure Active Directory, kjører du veiviseren for katalogsynkronisering og Azure AD Koble til som beskrevet i Konfigurere katalogsynkronisering [for Office 365](../enterprise/set-up-directory-synchronization.md).</span><span class="sxs-lookup"><span data-stu-id="7fa3c-112">To synchronize your users, groups, and contacts from local Active Directory into Azure Active Directory, run the Directory synchronization wizard and Azure AD Connect as described in [Set up directory synchronization for Office 365](../enterprise/set-up-directory-synchronization.md).</span></span>

2. <span data-ttu-id="7fa3c-113">Når katalogsynkroniseringen er fullført, må du kontrollere at organisasjonens Windows 10 er Azure AD sammenføyd.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-113">After the directory synchronization is complete, make sure your organization's Windows 10 devices are Azure AD joined.</span></span> <span data-ttu-id="7fa3c-114">Dette trinnet gjøres enkeltvis på hver Windows 10 enhet.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-114">This step is done individually on each Windows 10 device.</span></span> <span data-ttu-id="7fa3c-115">Se [Konfigurere Windows for Microsoft 365 Business Premium for mer](set-up-windows-devices.md) informasjon.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-115">See [Set up Windows devices for Microsoft 365 Business Premium users](set-up-windows-devices.md) for details.</span></span>

3. <span data-ttu-id="7fa3c-116">Når enhetene Windows 10 Azure AD, må hver bruker starte enhetene på nytt og logge på med Microsoft 365 Business Premium legitimasjon.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-116">Once the Windows 10 devices are Azure AD joined, each user must reboot their devices and sign in with their Microsoft 365 Business Premium credentials.</span></span> <span data-ttu-id="7fa3c-117">Alle enheter har nå også tilgang til lokale ressurser.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-117">All devices now have access to on-premises resources as well.</span></span>

<span data-ttu-id="7fa3c-118">Ingen ekstra trinn er nødvendig for å få tilgang til lokale ressurser for Azure AD-sammenføyde enheter.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-118">No additional steps are required to get access to on-premises resources for Azure AD joined devices.</span></span> <span data-ttu-id="7fa3c-119">Denne funksjonaliteten er innebygd i Windows 10.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-119">This functionality is built into Windows 10.</span></span>

<span data-ttu-id="7fa3c-120">Hvis du har planer om å logge på AADJ-enheten annet enn passordmetode, for eksempel PIN/Bio-metrisk via WHFB-pålogging og deretter få tilgang til lokale ressurser (aksjer, skrivere og så videre), følger du [denne artikkelen](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="7fa3c-120">If you have plans to login to the AADJ device other than password method Like PIN/Bio-metric via WHFB credential login and then access on-premise resources (shares, printers, etc.), please follow [this article](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="7fa3c-121">Hvis organisasjonen ikke er klar til å distribuere i konfigurasjonen av azure AD-sammenføyde enheter som er beskrevet ovenfor, bør du vurdere å konfigurere konfigurasjon av [hybrid Azure AD-sammenføyd enhet.](manage-windows-devices.md)</span><span class="sxs-lookup"><span data-stu-id="7fa3c-121">If your organization isn't ready to deploy in the Azure AD joined device configuration described above, consider setting up [Hybrid Azure AD Joined device configuration](manage-windows-devices.md).</span></span>

### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a><span data-ttu-id="7fa3c-122">Hensyn når du blir med Windows til Azure AD</span><span class="sxs-lookup"><span data-stu-id="7fa3c-122">Considerations when you join Windows devices to Azure AD</span></span>

<span data-ttu-id="7fa3c-123">Hvis enheten Windows Azure-AD ble med i tidligere domene, ble med i eller i en arbeidsgruppe, bør du vurdere følgende begrensninger:</span><span class="sxs-lookup"><span data-stu-id="7fa3c-123">If the Windows device that you Azure-AD joined was previously domain-joined or in a workgroup, consider the following limitations:</span></span>

- <span data-ttu-id="7fa3c-124">Når en enhet Azure AD blir med, opprettes en ny bruker uten å referere til en eksisterende profil.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-124">When a device Azure AD joins, it creates a new user without referencing an existing profile.</span></span> <span data-ttu-id="7fa3c-125">Profiler må overføres manuelt.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-125">Profiles must be manually migrated.</span></span> <span data-ttu-id="7fa3c-126">En brukerprofil inneholder informasjon som favoritter, lokale filer, nettleserinnstillinger og Start-menyinnstillinger.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-126">A user profile contains information like favorites, local files, browser settings, and Start menu settings.</span></span> <span data-ttu-id="7fa3c-127">Den beste fremgangsmåten er å finne et tredjepartsverktøy for å tilordne eksisterende filer og innstillinger til den nye profilen.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-127">A best approach is to find a third-party tool to map existing files and settings to the new profile.</span></span>

- <span data-ttu-id="7fa3c-128">Hvis enheten bruker gruppepolicyobjekter (GPO), kan det hende [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) at enkelte gruppepolicyobjekter ikke har en sammenlignbar konfigurasjonstjenesteleverandør (CSP) i Intune.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-128">If the device is using Group Policy Objects (GPO), some GPOs may not have a comparable [Configuration Service Provider](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) in Intune.</span></span> <span data-ttu-id="7fa3c-129">Kjør [MMAT-verktøyet for](https://www.microsoft.com/download/details.aspx?id=45520) å finne sammenlignbare CSP-er for eksisterende gruppepolicyobjekter.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-129">Run the [MMAT tool](https://www.microsoft.com/download/details.aspx?id=45520) to find comparable CSPs for existing GPOs.</span></span>

- <span data-ttu-id="7fa3c-130">Brukere kan kanskje ikke godkjenne til programmer som er avhengige av Active Directory-godkjenning.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-130">Users might not be able to authenticate to applications that depend on Active Directory authentication.</span></span> <span data-ttu-id="7fa3c-131">Evaluer den eldre appen, og vurder om mulig å oppdatere til en app som bruker moderne Auth.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-131">Evaluate the legacy app and consider updating to an app that uses modern Auth, if possible.</span></span>

- <span data-ttu-id="7fa3c-132">Active Directory-skriveroppdagelse fungerer ikke.</span><span class="sxs-lookup"><span data-stu-id="7fa3c-132">Active Directory printer discovery won't work.</span></span> <span data-ttu-id="7fa3c-133">Du kan angi direkte skriverbaner for alle brukere eller bruke [Universal Print](/universal-print/).</span><span class="sxs-lookup"><span data-stu-id="7fa3c-133">You can provide direct printer paths for all users or use [Universal Print](/universal-print/).</span></span>

### <a name="related-articles"></a><span data-ttu-id="7fa3c-134">Relaterte artikler</span><span class="sxs-lookup"><span data-stu-id="7fa3c-134">Related Articles</span></span>

[<span data-ttu-id="7fa3c-135">Forutsetninger for Azure AD-Koble til</span><span class="sxs-lookup"><span data-stu-id="7fa3c-135">Prerequisites for Azure AD Connect</span></span>](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
