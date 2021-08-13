---
title: Oversikt over oppsett
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
manager: scotv
audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Lær konfigurasjonstrinnene for Microsoft 365 Business Premium, fra å abonnere, legge til et domene og brukere, konfigurere sikkerhetspolicyer og mer.
ms.openlocfilehash: 7c09dca354781bf92f6bbecca0f3fb9875fb654515fe35c2f96cc780a894a764
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53803226"
---
# <a name="overview-of-setup"></a>Oversikt over oppsett

Se en kort video om Microsoft 365 Business Premium oppsett.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Hvis du synes at denne videoen er nyttig, kan du se den [fullstendige opplæringsserien for små bedrifter og de som er nybegynnere i Microsoft 365](../business-video/index.yml).

De fleste konfigurasjonstrinnene kan utføres i det veiledede oppsettet, men de andre alternativene er også oppført.

## <a name="step-1-add-your-domain-and-users"></a>Trinn 1: Legge til domenet og brukerne

   - **[Legg til domenet](set-up.md#add-your-domain-to-personalize-sign-in)** (hvis du kjøpte domenet under [registreringen,](sign-up.md)er dette trinnet allerede fullført.)

   - **Legg til brukere**. Du kan legge til brukere på en av de tre måtene:
        - I det [veiledede oppsettet](set-up.md#add-users-in-the-wizard).
        - Bruk katalogsynkronisering [til å legge til brukere](../enterprise/set-up-directory-synchronization.md) ved hjelp av Azure AD Koble til hvis du har en lokal Active Directory.
        - Du kan også [legge til brukere senere](../admin/add-users/add-users.md) i administrasjonssenteret.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Trinn 2: Konfigurere sikkerhetspolicyer og konfigurere enheter 

  - Bruk det [veiledede oppsettet til](set-up.md#protect-your-organization) å konfigurere enhetspolicyer. 
  - Du kan også legge til flere eller redigere dem senere i [administrasjonssenteret](view-policies-and-devices.md) og [i Intune-portalen.](/intune/tutorial-walkthrough-intune-portal)
  - Konfigurasjonsveiviseren konfigurerer også grunnleggende innstillinger for beskyttelse mot trusler og hindring av datatap.
  
  I tillegg til sikkerhetsinnstillingene i konfigurasjonsveiviseren kan du øke sikkerheten ved å legge til følgende innstillinger:

- **Beskyttelse mot skadelig e-post**
- **Anti-phishing i Defender for Office 365**
- **Exchange Online Archiving**
- **Azure Information Protection (Plan1**)

Hvis du vil komme i gang, kan du se [Øke trusselbeskyttelse](increase-threat-protection.md) [og konfigurere samsvarsfunksjoner](set-up-compliance.md).

Se også [de ti beste måtene å sikre Microsoft 365 Business Premium](/office365/admin/security-and-compliance/secure-your-business-data) for et veikart over anbefalte sikkerhetsrutiner.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Trinn 3: Konfigurere og administrere Windows 10 enheter

Når du har fullført den veiledede konfigurasjonen, bør du beskytte alle Windows 10 datamaskinene i organisasjonen.
  
- Windows 10 Pro er en forutsetning [for](pre-requisites-for-data-protection.md) Microsoft 365 Business Premium, men hvis du har Windows 7 Pro, Windows 8 Pro eller Windows 8.1 Pro, gir abonnementet deg rett til en oppgradering til [Windows 10 Pro](./upgrade-to-windows-pro-creators-update.md).
- Følg fremgangsmåten i sikre [Windows 10 PC-er](secure-win-10-pcs.md) for å konfigurere policyer for Windows 10 enheter.

Når du blir med Windows 10 en enhet til Azure AD, brukes policyene du har angitt for Windows 10 datamaskiner. Hvis du vil ha mer informasjon, [kan du se Konfigurere Windows enheter for Microsoft 365 brukere](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Trinn 4: Installere Microsoft 365 Apps for business
- Du kan automatisk installere Office på Windows enheter ved hjelp av [konfigurasjonsveiviseren](set-up.md#deploy-office-365-client-apps).
- La brukere [Office apper](/office365/admin/setup/install-applications) for Windows og enheter.
     
## <a name="advanced"></a>Avansert
- **Bruke Autopilot til å konfigurere nye enheter**
            
     Du kan [bruke Windows Autopilot](add-autopilot-devices-and-profile.md) til automatisk å forhåndskonfigurere nye **Windows 10-enheter** for en bruker, men det kan være enklere å få en [partner](https://www.microsoft.com/solution-providers/search) som kan gjøre dette for deg. Du kan også gå til [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), og be en ekspert på skyteknologi om å konfigurere nye enheter du kjøper.

- **Få tilgang til lokale ressurser**

     - Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business Premium til å beskytte Windows 10-enhetene, samtidig som du beholder tilgang til lokale ressurser som krever lokal godkjenning. Følg fremgangsmåten i [Aktivere domenekretserte](manage-windows-devices.md) Windows 10 enheter som skal administreres Microsoft 365 Business Premium å konfigurere dette. Dette er den foretrukne metoden, og enheter i denne tilstanden kalles Hybrid Azure AD-sammenføyde enheter.

    - Hvis bedriften har en lokal Active Directory som inneholder noen lokale ressurser (for eksempel delte filressurser og skrivere), kan du gi azure AD-sammenføyde enheter tilgang til disse ressursene ved å følge fremgangsmåten her: Få tilgang til lokale ressurser fra en Azure AD-sammenføyd enhet i [Microsoft 365 Business Premium](access-resources.md).

## <a name="related-content"></a>Beslektet innhold

[Microsoft 365 opplæringsvideoer for bedrifter](../business-video/index.yml) (koblingsside)