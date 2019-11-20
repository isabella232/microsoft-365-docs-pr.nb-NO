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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Oversikt over konfigurasjonstrinnene for Microsoft 365 Business.
ms.openlocfilehash: 3447f06d031462a7bebc6f129238de9f0c5dee41
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/19/2019
ms.locfileid: "38721563"
---
# <a name="overview-of-setup"></a>Oversikt over oppsett

De fleste av trinnene i oppsettet kan gjøres i installasjonsveiviseren, men de andre alternativene er også oppført.

## <a name="step-1-add-your-domain-and-users"></a>Trinn 1: Legg til domenet og brukerne

   - **[Legg til domenet ditt](set-up.md#add-your-domain-to-personalize-sign-in)** (Hvis du kjøpte domenet under [registreringen](sign-up.md), er dette trinnet allerede gjort.)

    - **Legge til brukere**. Du kan legge til brukere på hvilken som helst av de tre måtene:
        - I [veiviseren](set-up.md#add-users-in-the-wizard).
        - Bruk katalogsynkronisering for å [legge til brukere ved hjelp av Azure ad-tilkobling](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) hvis du har en lokal Active Directory.
        - Du kan også [legge til brukere senere](add-users-m365b.md) i administrasjonssenteret.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Trinn 2: konfigurere sikkerhetspolicyer og konfigurere enheter 

  - Bruk [installasjonsveiviseren](set-up.md#protect-data-and-devices) til å konfigurere enhets-og sikkerhetspolicyer. 
  - Du kan også legge til flere eller redigere dem senere i [administrasjonssenteret](view-policies-and-devices.md) og i [Intune-portalen](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - I tillegg til sikkerhetsinnstillingene i installasjonsveiviseren kan du øke sikkerheten ved å legge til følgende innstillinger:

      - **Email malware beskyttelse**
      - **Avanserte trusselbeskyttelse (ATP) sikker linker**
      - **Sikre vedlegg i ATP**
      - **ATP anti-phishing**
      - **Exchange Online Archiving**
      - **Hindring av tap av data (DLP)**
      - **Azure informasjonsbeskyttelse (Plan1**)

          [Sett opp avanserte sikkerhetspolicyer](set-up-advanced-security.md)for å komme i gang med å se.

        Se også [topp 10 måter å sikre din Microsoft 365 Business](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for et veikart for beste sikkerhet praksis.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Trinn 3: konfigurere og administrere Windows 10-enheter

   Når du blir med i en Windows 10-enhet til Azure AD, blir policyene du konfigurerer i [trinn 2](#step-2-set-up-security-policies-and-configure-devices) , brukt på den.

   - Windows 10 Pro er en [forutsetning](pre-requisites-for-data-protection.md) for Microsoft 365 Business, men hvis du har Windows 7 Pro, Windows 8 Pro eller Windows 8,1 Pro, gir abonnementet deg rett til en [oppgradering til Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
    - Bruk [installasjonsveiviseren](set-up.md#protect-data-and-devices) til å konfigurere policyer for Windows 10-enheter.

## <a name="step-4-install-office-365-business"></a>Trinn 4: installere Office 365 Business
- Du kan installere Office automatisk i Windows-enheter ved hjelp av [installasjonsveiviseren](set-up.md#deploy-office-365-client-apps).
- La brukere [installere Office-apper](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows og enheter.
     
## <a name="advanced"></a>Avansert
- **Bruk autopilot til å konfigurere nye enheter**
            
     Du kan bruke [Windows autopilot](add-autopilot-devices-and-profile.md) til å forhånds konfigurere **nye** Windows 10-enheter for en bruker automatisk, men det kan være enklere å få en [partner](https://www.microsoft.com/solution-providers/search) som kan gjøre dette for deg. Du kan også gå til [Microsoft store](https://go.microsoft.com/fwlink/?linkid=874598)og be en ekspert på skyteknologi om å konfigurere nye enheter du kjøper.

- **Få tilgang til lokale ressurser**

     - Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business for å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgang til lokale ressurser som krever lokal godkjenning. Følg trinnene i [aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business](manage-windows-devices.md) for å konfigurere dette. Dette er den foretrukne metoden, og enheter i denne tilstanden kalles Hybrid Azure AD koblet enheter.

    - Hvis bedriften din har en lokal Active Directory som inneholder noen lokale ressurser (for eksempel delte filressurser og skrivere), kan du gi Azure AD-tilknyttede enheter tilgang til disse ressursene ved å følge fremgangsmåten her: [få tilgang til lokale ressurser fra en Azure ad-sammenkoblet enhet i Microsoft 365 Business](access-resources.md).

  