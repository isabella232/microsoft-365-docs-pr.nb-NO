---
title: Aktivere domene-sammenføyde Windows 10-enheter som skal administreres av Microsoft 365 for bedrifter
f1.keywords:
- NOCSH
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Lær hvordan du aktiverer Microsoft 365 til å beskytte lokale Active-Directory-tilkoblede Windows 10-enheter med bare noen få trinn.
ms.openlocfilehash: 7bfe5da8701a17712fa249eac99a22b8d5a1b2d1
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471051"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Aktivere domeneblede Windows 10-enheter som skal administreres av Microsoft 365 Business Premium

Hvis organisasjonen bruker lokal Windows Server Active Directory, kan du konfigurere Microsoft 365 Business Premium til å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgangen til lokale ressurser som krever lokal godkjenning.
Hvis du vil konfigurere denne beskyttelsen, kan du implementere **Hybrid Azure AD sammenføyde enheter**. Disse enhetene er koblet til både den lokale Active Directory og Azure Active Directory.

Denne videoen beskriver fremgangsmåten for hvordan du konfigurerer dette for det vanligste scenariet, som også er beskrevet i trinnene som følger.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Klargjør for katalogsynkronisering 

Før du synkroniserer brukere og datamaskiner fra det lokale Active Directory-domenet, kan du se [Klargjøre for katalogsynkronisering til Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Spesielt:

   - Kontroller at det ikke finnes noen duplikater i katalogen for følgende attributter: **e-post**, **proxyAddresses**og **userPrincipalName**. Disse verdiene må være unike, og eventuelle duplikater må fjernes.
   
   - Vi anbefaler at du konfigurerer **attributtet userPrincipalName** (UPN) for hver lokal brukerkonto slik at den samsvarer med den primære e-postadressen som tilsvarer den lisensierte Microsoft 365-brukeren. For eksempel: *mary.shelley@contoso.com* i stedet for *mary@contoso.local*
   
   - Hvis Active Directory-domenet slutter i et ikke-rutbart suffiks som *.local* eller *.lan*, i stedet for et Internett-rutbart suffiks, for eksempel *.com* eller *.org*, justerer du UPN-suffikset for de lokale brukerkontoene først som beskrevet i [Klargjør et ikke-rutbart domene for katalogsynkronisering](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Installere og konfigurere Azure AD Connect

Hvis du vil synkronisere brukere, grupper og kontakter fra den lokale Active Directory til Azure Active Directory, installerer du Azure Active Directory Connect og konfigurerer katalogsynkronisering. Se [Konfigurere katalogsynkronisering for Office 365 for](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) å finne ut mer.

> [!NOTE]
> Fremgangsmåten er nøyaktig den samme for Microsoft 365 for bedrifter. 

Når du konfigurerer alternativene for Azure AD Connect, anbefaler vi at du aktiverer **synkronisering av passord**, **sømløs enkel pålogging**og funksjonen for **tilbakeskriving** av passord, som også støttes i Microsoft 365 for bedrifter.

> [!NOTE]
> Det er noen flere trinn for passord writeback utover avmerkingsboksen i Azure AD Connect. Hvis du vil ha mer informasjon, kan du se [Slik gjør du det: konfigurere passord writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Konfigurer Hybrid Azure AD-sammenføyning

Før du aktiverer At Windows 10-enheter skal være Hybrid Azure AD koblet til, må du kontrollere at du oppfyller følgende forutsetninger:

   - Du kjører den nyeste versjonen av Azure AD Connect.

   - Azure AD connect har synkronisert alle datamaskinobjektene til enhetene du vil være hybrid Azure AD som er koblet sammen. Hvis datamaskinobjektene tilhører bestemte organisasjonsenheter (OU), må du kontrollere at disse OUene er angitt for synkronisering i Azure AD-tilkobling også.

Hvis du vil registrere eksisterende domenetilknyttede Windows 10-enheter som Hybrid Azure AD ble med, følger du fremgangsmåten i [opplæringen: Konfigurere hybrid Azure Active Directory-sammenføyning for administrerte domener](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Denne hybrid-aktiverer eksisterende lokale Active Directory sammenføyde Windows 10-datamaskiner og gjør dem skyklare.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Aktivere automatisk registrering for Windows 10

 Hvis du vil registrere Windows 10-enheter automatisk for administrasjon av mobilenheter i Intune, kan du se [Registrere en Windows 10-enhet automatisk ved hjelp av gruppepolicy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Du kan angi gruppepolicyen på lokalt datamaskinnivå, eller for masseoperasjoner, kan du bruke group Policy Management Console og ADMX-maler til å opprette denne gruppepolicyinnstillingen på domenekontrolleren.

## <a name="5-configure-seamless-single-sign-on"></a>5. Konfigurer sømløs enkel pålogging

  Sømløs SSO logger automatisk brukere inn i Microsoft 365-skyressursene når de bruker bedriftsdatamaskiner. Bare distribuer ett av de to gruppepolicyalternativene som er beskrevet i [Azure Active Directory Seamless Single Sign-On: Hurtigstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). **Gruppepolicyalternativet** tillater ikke brukere å endre innstillingene sine, mens alternativet **Gruppepolicyinnstillinger** angir verdiene, men også lar dem konfigureres.

## <a name="6-set-up-windows-hello-for-business"></a>6. Konfigurere Windows Hello for bedrifter

 Windows Hello for Business erstatter passord med sterk tofaktorautentisering (2FA) for å logge på en lokal datamaskin. En faktor er et asymmetrisk nøkkelpar, og det andre er en PIN-kode eller annen lokal bevegelse, for eksempel fingeravtrykk eller ansiktsgjenkjenning hvis enheten støtter den. Vi anbefaler at du erstatter passord med 2FA og Windows Hello for Business der det er mulig.

Hvis du vil konfigurere Hybrid Windows Hello for bedrifter, kan du se [gjennom Hybrid Nøkkel klarering Windows Hello for Business Forutsetninger](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Følg deretter instruksjonene i [Konfigurere innstillinger for viktig klarering av Hybrid Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
