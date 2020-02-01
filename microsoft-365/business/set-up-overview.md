---
title: Oversikt over oppsett
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Oversikt over konfigurasjonstrinnene for Microsoft 365 Business.
ms.openlocfilehash: 07cbd4fd187f78474783db848ac9b69068d2b44a
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2020
ms.locfileid: "41595069"
---
# <a name="overview-of-setup"></a>Oversikt over oppsett

Se en kort video om installasjonsprogrammet for Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Hvis du synes at denne videoen er nyttig, kan du se den [fullstendige opplæringsserien for små bedrifter og de som er nybegynnere i Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

De fleste konfigurasjonstrinnene kan gjøres i installasjonsveiviseren, men de andre alternativene vises også.

## <a name="step-1-add-your-domain-and-users"></a>Trinn 1: Legg til domenet og brukerne

   - **[Legg til domenet ditt](set-up.md#add-your-domain-to-personalize-sign-in)** (hvis du kjøpte domenet under [registrering](sign-up.md), er dette trinnet allerede gjort.)

    - **Legg til brukere**. Du kan legge til brukere på en av de tre måtene:
        - I [veiviseren](set-up.md#add-users-in-the-wizard).
        - Bruk katalogsynkronisering til å [legge til brukere ved hjelp av Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) hvis du har en lokal Active-katalog.
        - Du kan også [legge til brukere senere](add-users-m365b.md) i administrasjonssenteret.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Trinn 2: Konfigurere sikkerhetspolicyer og konfigurere enheter 

  - Bruk [installasjonsveiviseren](set-up.md#protect-your-organization) til å konfigurere enhetspolicyer. 
  - Du kan også legge til flere eller redigere dem senere i [administrasjonssenteret](view-policies-and-devices.md) og i [Intune-portalen](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Installasjonsveiviseren vil også definere grunnleggende innstillinger for trusselbeskyttelse og hindring av tap av data.
  
  I tillegg til sikkerhetsinnstillingene i installasjonsveiviseren kan du øke sikkerheten ved å legge til følgende innstillinger:

- **Beskyttelse mot beskyttelse mot beskyttelse mot skadelig programvare for e-**
- **ATP anti-phishing**
- **Exchange Online Archiving**
- **Azure Information Protection (Plan1**)

Hvis du vil komme i gang, kan du se [Øke trusselbeskyttelsen](increase-threat-protection.md) og [konfigurere samsvarsfunksjoner](set-up-compliance.md).

Se også [topp 10 måter å sikre Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for et veikart over anbefalte sikkerhetsfremgangsmåter.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Trinn 3: Konfigurere og administrere Windows 10-enheter

Når du har kjørt oppsettveiviseren, vil du ønske å proctect alle Windwos 10 datamaskiner i organisasjonen.
  
- Windows 10 Pro er en [forutsetning](pre-requisites-for-data-protection.md) for Microsoft 365 Business, men hvis du har Windows 7 Pro, Windows 8 Pro eller Windows 8.1 Pro, gir abonnementet deg rett til en [oppgradering til Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Følg trinnene i [sikre Windows 10-PCer](secure-win-10-pcs.md) for å definere policyer for Windows 10-enheter.

Når du blir med i en Windows 10-enhet i Azure AD, blir policyene du angir for Windows 10-datamaskiner, brukt på den. Hvis du vil ha mer informasjon, kan du se [Konfigurere Windows-enheter for Brukere av Microsoft 365 Business](set-up-windows-devices.md).

## <a name="step-4-install-office-365-business"></a>Trinn 4: Installere Office 365 Business
- Du kan installere Office automatisk i Windows-enhetene ved hjelp av [installasjonsveiviseren](set-up.md#deploy-office-365-client-apps).
- La brukere [installere Office-apper](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows og enheter.
     
## <a name="advanced"></a>Avansert
- **Bruk Autopilot til å konfigurere nye enheter**
            
     Du kan bruke [Windows Autopilot](add-autopilot-devices-and-profile.md) til å forhåndskonfigurere **nye** Windows 10-enheter for en bruker automatisk, men det kan være enklere å få en [partner](https://www.microsoft.com/solution-providers/search) som kan gjøre dette for deg. Du kan også gå til [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598), og be en skyteknologiekspert om å konfigurere nye enheter du kjøper.

- **Få tilgang til lokale ressurser**

     - Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business til å beskytte Windows 10-enheter, samtidig som du opprettholder tilgangtil lokale ressurser som krever lokal godkjenning. Følg trinnene i [Aktiver domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business](manage-windows-devices.md) for å konfigurere dette. Dette er den foretrukne metoden, og enheter i denne tilstanden kalles Hybrid Azure AD-tilknyttede enheter.

    - Hvis bedriften din har en lokal Active Directory som inneholder noen lokale ressurser (for eksempel fildelinger og skrivere), kan du gi Azure AD-tilknyttede enheter tilgang til disse ressursene ved å følge trinnene her: [Få tilgang til lokale ressurser fra en Azure AD-tilknyttet enhet i Microsoft 365 Business](access-resources.md).

## <a name="see-also"></a>Se også

[Opplæringsvideoer for Microsoft 365-bedrifter](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
