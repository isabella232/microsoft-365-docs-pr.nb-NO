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
description: Lær om konfigurasjons trinnene for Microsoft 365 Business Premium, fra å abonnere, legge til et domene og brukere, for å konfigurere sikkerhets policyer og mer.
ms.openlocfilehash: 46370166a9d5e8c9308b8947513e631c159f0b86
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842134"
---
# <a name="overview-of-setup"></a>Oversikt over oppsett

Se en kort video om Microsoft 365 Business Premium-oppsett.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

Hvis du synes at denne videoen er nyttig, kan du se den [fullstendige opplæringsserien for små bedrifter og de som er nybegynnere i Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

De fleste konfigurasjons trinnene kan gjøres i veilednings oppsettet, men de andre alternativene er også oppført.

## <a name="step-1-add-your-domain-and-users"></a>Trinn 1: legge til domenet og brukerne

   - **[Legg til domenet](set-up.md#add-your-domain-to-personalize-sign-in)** (Hvis du kjøpte domenet under [registreringen](sign-up.md), er dette trinnet allerede gjort.)

   - **Legge til brukere**. Du kan legge til brukere på en av de tre måtene:
        - I [veg leiings konfigurasjonen](set-up.md#add-users-in-the-wizard).
        - Bruk katalog synkronisering til å [legge til brukere ved hjelp av Azure ad Connect](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) hvis du har en lokal Active Directory.
        - Du kan også [legge til brukere senere](add-users-m365b.md) i administrasjons senteret.
## <a name="step-2-set-up-security-policies-and-configure-devices"></a>Trinn 2: konfigurere sikkerhets policyer og konfigurere enheter 

  - Bruk [veiledende oppsett](set-up.md#protect-your-organization) til å konfigurere enhets policyer. 
  - Du kan også legge til flere eller redigere dem senere i [administrasjons senteret](view-policies-and-devices.md) og i [Intune-portalen](https://docs.microsoft.com/intune/tutorial-walkthrough-intune-portal).
  - Installasjons vei viseren vil også konfigurere grunnleggende trussel beskyttelse og innstillinger for hindring av tap av data.
  
  I tillegg til sikkerhets innstillingene i installasjons vei viseren kan du øke sikkerheten ved å legge til følgende innstillinger:

- **Beskyttelse mot skadelig program vare**
- **Anti-phishing i Defender for Office 365**
- **Exchange Online Archiving**
- **Azure Information Protection (Plan1** )

Hvis du vil komme i gang, kan du se [øke trussel beskyttelse](increase-threat-protection.md) og [konfigurere samsvars funksjoner](set-up-compliance.md).

Se også [de 10 beste metodene for å sikre Microsoft 365 Business Premium](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for et vei kart over de beste sikkerhets rutinene.

## <a name="step-3-set-up-and-manage-windows-10-devices"></a>Trinn 3: konfigurere og administrere Windows 10-enheter

Når du har fullført det veiledende oppsettet, vil du beskytte alle Windows 10-datamaskinene i organisasjonen.
  
- Windows 10 Pro er en [forutsetning](pre-requisites-for-data-protection.md) for Microsoft 365 Business Premium, men hvis du har Windows 7 Pro, Windows 8 Pro eller Windows 8,1 Pro, gir abonnementet deg en [oppgradering til Windows 10 Pro](https://docs.microsoft.com/microsoft-365/business/upgrade-to-windows-pro-creators-update).
- Følg Fremgangs måten i [sikre Windows 10-PCer](secure-win-10-pcs.md) for å konfigurere policyer for Windows 10-enheter.

Når du blir med i en Windows 10-enhet til Azure AD, blir policyene du angir for Windows 10-datamaskiner, brukt på den. Hvis du vil ha mer informasjon, kan du se [konfigurere Windows-enheter for Microsoft 365-brukere](set-up-windows-devices.md).

## <a name="step-4-install-microsoft-365-apps-for-business"></a>Trinn 4: installere Microsoft 365-apper for bedrifter
- Du kan installere Office automatisk i Windows-enheter ved hjelp av [konfigurasjons vei viseren](set-up.md#deploy-office-365-client-apps).
- La brukere [installere Office-apper](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows og enheter.
     
## <a name="advanced"></a>Avansert
- **Bruke autopiloten til å konfigurere nye enheter**
            
     Du kan bruke [Windows autopilot](add-autopilot-devices-and-profile.md) til automatisk å forhånds kon figurer **nye** Windows 10-enheter for en bruker, men det kan være enklere å få en [partner](https://www.microsoft.com/solution-providers/search) som kan gjøre dette for deg. Du kan også gå til [Microsoft store](https://go.microsoft.com/fwlink/?linkid=874598)og spørre en sky teknologi ekspert for å konfigurere nye enheter som du kjøper.

- **Få tilgang til lokale ressurser**

     - Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business Premium til å beskytte Windows 10-enhetene, samtidig som du fortsatt har tilgang til lokale ressurser som krever lokal godkjenning. Følg trinnene i [Aktiver domene tilknyttede Windows 10-enheter for å administreres av Microsoft 365 Business Premium](manage-windows-devices.md) for å konfigurere dette. Dette er den foretrukne metoden, og enheter i denne tilstanden kalles Hybrid Azure AD-tilknyttede enheter.

    - Hvis virksomheten har en lokal Active Directory som inneholder noen lokale ressurser (for eksempel delte fil ressurser og skrivere), kan du gi Azure AD-tilknyttede enheter tilgang til disse ressursene ved å følge Fremgangs måten nedenfor: [få tilgang til lokale ressurser fra en Azure ad-tilknyttet enhet i Microsoft 365 Business Premium](access-resources.md).

## <a name="see-also"></a>Se også

[Opplærings videoer for Microsoft 365 for bedrifter](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
