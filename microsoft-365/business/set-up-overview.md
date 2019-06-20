---
title: Oversikt over oppsett
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Oversikt over satt opp trinnene for Microsoft 365 Business.
ms.openlocfilehash: ae7ed0aab36a6e759e0f0c1fbc3d3183273a284e
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/15/2019
ms.locfileid: "35086354"
---
# <a name="overview-of-setup"></a>Oversikt over oppsett

Det meste av den er satt opp trinnene kan gjøres i installasjonsveiviseren, men de andre alternativene er også oppført.


## <a name="step-1-add-your-domain-and-users"></a>Trinn 1: Legge til domenet og brukere

   - **[Legg til domenet ditt](set-up.md#add-your-domain-to-personalize-sign-in)** (Hvis du kjøpte domenet ditt ved å [registrere deg](sign-up.md), dette trinnet er allerede har gjort.)

    - **Legg til brukere**. Du kan gjøre dette på en av tre måter:
        - I [veiviseren](set-up.md#add-users-in-the-wizard).
        - Bruk katalogsynkronisering for å [legge til brukere ved hjelp av Azure AD-tilkobling](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) Hvis du har en lokale Active directory.
        - Du kan også [legge til senere brukere](add-users-m365b.md) i administrasjonssenteret.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Trinn 2: Konfigurere sikkerhetspolicyer og konfigurere enheter 

  - Bruke [veiviseren for installasjon](set-up.md#set-up-security-policies-and-device-configurations) til å konfigurere enheten og sikkerhetspolicy. 
  - Du kan også legge til flere eller redigere dem senere i [administrasjonssenteret](view-policies-and-devices.md) og [Intune portal](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - I tillegg til sikkerhetsinnstillingene i veiviseren, kan du øke sikkerheten ved å legge til følgende innstillinger:

      - **Beskyttelse mot skadelig programvare for e-post**
      - **Avanserte Threat Protection (ATP) sikre koblinger**
      - **ATP-Safe vedlegg**
      - **ATP anti-phishing**
      - **Exchange Online Archiving**
      - **Data tap forebygging (DLP)**
      - **Azure informasjonsbeskyttelse (Plan1**)

          Å komme i gang, kan du se [konfigurere avanserte sikkerhetspolicyer](set-up-advanced-security.md).

        Se også [topp 10 måter å sikre bedriften din Microsoft-365](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for et veikart for gode fremgangsmåter for sikkerhet.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Trinn 3: Konfigurere og administrere Windows 10 enheter

   Når du slår sammen en enhet for Windows 10 Azure AD, policyene du har angitt i [trinn 2](#step-2-set-up-security-policies-and-configure-devices) , brukes den.

   - Windows 10 Pro er en [forutsetning](pre-requisites-for-data-protection.md) for Microsoft 365 Business, men hvis du har Windows 7 Pro, Windows 8 Pro eller Windows 8.1 Pro, abonnementet sikrer deg en [oppgradering til Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
    - Bruk [veiviseren](set-up.md#set-up-security-policies-and-device-configurations) til å konfigurere policyer for Windows 10 enheter.

## <a name="stes-4-install-office-365-business"></a>Stes 4: Installere Office 365-Business
- Du kan installere Office automatisk i Windows-enheter ved hjelp av [installasjonsveiviseren](set-up.md#deploy-office-365-client-apps).
- Automatisk [installerer Office](auto-install-or-uninstall-office.md) fra administrasjonssenteret.
- La brukere [installere Office-programmer](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows og enheter.
     
## <a name="advanced"></a>Avansert
- **Bruk Autopilot til å definere nye enheter**
            
     Du kan bruke [Windows Autopilot](add-autopilot-devices-and-profile.md) å automatisk forhåndskonfigurere **nye** Windows 10 enheter for en bruker, men det kan være enklere å få en [partner](https://www.microsoft.com/solution-providers/search) som kan gjøre dette for deg. Du kan også gå til [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) og be om en sky teknologi ekspert definere nye enheter du kjøpe for deg.

- **Få tilgang til lokale ressurser**

     - Hvis organisasjonen bruker Windows Server Active Directory på lokaler, kan du definere Microsoft 365 Business til å beskytte Windows 10 enheter, samtidig som du har tilgang til lokale ressurser som krever lokal godkjenning. Følg trinnene i [aktivere domenetilknyttede Windows 10 enheter som skal administreres av Microsoft 365 Business](manage-windows-devices.md) å sette opp dette. Dette er den foretrukne metoden og enheter i denne tilstanden kalles Hybrid Azure AD koblet enheter.

    - Hvis firmaet har en lokal Active Directory, som inneholder noen lokale ressurser (for eksempel delte filer og skrivere), kan du gi din Azure AD-koblet enheter tilgang til disse ressursene ved å følge fremgangsmåten her: [Access lokale ressurser fra en Azure AD-koblet enheten i Microsoft 365 Business](access-resources.md).

  