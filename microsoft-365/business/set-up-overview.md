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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Lær installasjonstrinnene for Microsoft 365 Business Premium, fra å abonnere, til å legge til et domene og brukere, til å konfigurere sikkerhetspolicyer og mer.
ms.openlocfilehash: a808ae5761c1bc5706966a3f7de95f96f8f7c8c8
ms.sourcegitcommit: e5bc49f0a25954d008b6cc09c2b98bb7bfe1aa2f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/18/2020
ms.locfileid: "44785816"
---
# <a name="overview-of-setup"></a>Oversikt over oppsett

Se en kort video om Microsoft 365 Business Premium-oppsett.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Hvis du synes at denne videoen er nyttig, kan du se den [fullstendige opplæringsserien for små bedrifter og de som er nybegynnere i Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

De fleste installasjonstrinnene kan gjøres i installasjonsveiviseren, men de andre alternativene er også oppført.

## <a name="step-1-add-your-domain-and-users"></a>Trinn 1: Legg til domenet og brukerne

   - **[Legg til domenet ditt](set-up.md#add-your-domain-to-personalize-sign-in)** (hvis du kjøpte domenet under [registrering,](sign-up.md)er dette trinnet allerede gjort.)

   - **Legge til brukere**. Du kan legge til brukere på en av de tre måtene:
        - I [veiviseren](set-up.md#add-users-in-the-wizard).
        - Bruk katalogsynkronisering til å [legge til brukere ved hjelp av Azure AD Connect](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) hvis du har en lokal Active-katalog.
        - Du kan også [legge til brukere senere](add-users-m365b.md) i administrasjonssenteret.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Trinn 2: Konfigurere sikkerhetspolicyer og konfigurere enheter 

  - Bruk [installasjonsveiviseren](set-up.md#protect-your-organization) til å konfigurere enhetspolicyer. 
  - Du kan også legge til flere eller redigere dem senere i [administrasjonssenteret](view-policies-and-devices.md) og i [Intune-portalen](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Installasjonsveiviseren vil også konfigurere grunnleggende innstillinger for trusselbeskyttelse og datatapsforhindring.
  
  I tillegg til sikkerhetsinnstillingene i installasjonsveiviseren kan du øke sikkerheten ved å legge til følgende innstillinger:

- **Beskyttelse mot skadelig programvare via e-post**
- **ATP anti-phishing**
- **Exchange Online Archiving**
- **Azure Informasjonsbeskyttelse (Plan1**)

Du kommer i gang ved å se [øke trusselbeskyttelsen](increase-threat-protection.md) og [konfigurere samsvarsfunksjoner](set-up-compliance.md).

Se også [topp 10 måter å sikre Microsoft 365 Business Premium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) på for et veikart over anbefalte sikkerhetspraksiser.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Trinn 3: Konfigurere og administrere Windows 10-enheter

Når du har kjørt veiviseren for oppsett, vil du ønske å proctect alle Windwos 10 datamaskiner i organisasjonen.
  
- Windows 10 Pro er en [forutsetning](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, men hvis du har Windows 7 Pro, Windows 8 Pro eller Windows 8.1 Pro, gir abonnementet deg rett til en [oppgradering til Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Følg trinnene i [sikre Windows 10-PCer](secure-win-10-pcs.md) for å konfigurere policyer for Windows 10-enheter.

Når du blir med en Windows 10-enhet til Azure AD, blir policyene du angir for Windows 10-datamaskiner, brukt på den. Hvis du vil ha mer informasjon, kan du se [Konfigurere Windows-enheter for Microsoft 365-brukere](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Trinn 4: Installere Microsoft 365 Apps for business
- Du kan installere Office automatisk på Windows-enhetene ved hjelp av [installasjonsveiviseren](set-up.md#deploy-office-365-client-apps).
- La brukere [installere Office-apper](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows og enheter.
     
## <a name="advanced"></a>Avansert
- **Bruke Autopilot til å konfigurere nye enheter**
            
     Du kan bruke [Windows Autopilot](add-autopilot-devices-and-profile.md) til å forhåndskonfigurere **nye** Windows 10-enheter for en bruker automatisk, men det kan være enklere å få en [partner](https://www.microsoft.com/solution-providers/search) som kan gjøre dette for deg. Du kan også gå til [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598)og be en skyteknologiekspert om å konfigurere nye enheter du kjøper.

- **Få tilgang til lokale ressurser**

     - Hvis organisasjonen bruker lokal Windows Server Active Directory, kan du konfigurere Microsoft 365 Business Premium til å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgangen til lokale ressurser som krever lokal godkjenning. Følg trinnene i [Aktiver domenet som er sammenkoblet til Windows 10-enheter som skal administreres av Microsoft 365 Business Premium](manage-windows-devices.md) for å konfigurere dette. Dette er den foretrukne metoden, og enheter i denne tilstanden kalles Hybrid Azure AD sammenføyde enheter.

    - Hvis bedriften din har en lokal Active Directory som inneholder noen lokale ressurser (for eksempel delte filressurser og skrivere), kan du gi Azure AD-tilkoblede enheter tilgang til disse ressursene ved å følge fremgangsmåten her: [Få tilgang til lokale ressurser fra en Azure AD-tilknyttet enhet i Microsoft 365 Business Premium](access-resources.md).

## <a name="see-also"></a>Se også

[Opplæringsvideoer for Microsoft 365 for bedrifter](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
