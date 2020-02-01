---
title: Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Lær hvordan du aktiverer Microsoft 365 for å beskytte lokale Active Directory-tilknyttede Windows 10-enheter.
ms.openlocfilehash: 170703c7367f9c0e9cb4c10edbd81cb214aa1d3e
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593805"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business

Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business til å beskytte Windows 10-enheter, samtidig som du opprettholder tilgangtil lokale ressurser som krever lokal godkjenning.
Hvis du vil konfigurere denne beskyttelsen, kan du implementere **Hybrid Azure AD-sammenkoblede enheter**. Disse enhetene er koblet til både den lokale Active Directory og Azure Active Directory.

Denne videoen beskriver fremgangsmåten for hvordan du konfigurerer dette for det vanligste scenariet, som også er beskrevet i trinnene som følger.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="1-prepare-for-directory-synchronization"></a>1. Klargjør for katalogsynkronisering 

Før du synkroniserer brukere og datamaskiner fra det lokale Active Directory-domenet, kan du se [Klargjøre for katalogsynkronisering til Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Spesielt:

   - Kontroller at det ikke finnes noen duplikater i katalogen for følgende attributter: **e-post**, **proxyAddresses**og **userPrincipalName**. Disse verdiene må være unike, og eventuelle duplikater må fjernes.
   
   - Vi anbefaler at du konfigurerer **attributtet userPrincipalName** (UPN) for hver lokale brukerkonto slik at den samsvarer med den primære e-postadressen som tilsvarer den lisensierte Microsoft 365-brukeren. For eksempel: *mary.shelley@contoso.com* i stedet for *mary@contoso.local*
   
   - Hvis Active Directory-domenet slutter i et ikke-rutbart suffiks som *.local* eller *.lan*, i stedet for et internet routable suffiks som *.com* eller *.org*, justerer DU UPN-suffikset for de lokale brukerkontoene først som beskrevet i [Klargjøre et ikke-routable-domene for katalogsynkronisering](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Installer og konfigurer Azure AD Connect

Hvis du vil synkronisere brukere, grupper og kontakter fra den lokale Active Directory til Azure Active Directory, installerer du Azure Active Directory Connect og konfigurerer katalogsynkronisering. Se [Konfigurere katalogsynkronisering for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) for å finne ut mer.

> [!NOTE]
> Trinnene er nøyaktig de samme for Microsoft 365 Business. 

Når du konfigurerer alternativene for Azure AD Connect, anbefaler vi at du aktiverer **synkronisering av passord**, sømløs enkel **pålogging**og funksjonen for **passordskriving,** som også støttes i Microsoft 365 Business.

> [!NOTE]
> Det er noen flere trinn for passordwriteback utover avmerkingsboksen i Azure AD Connect. Hvis du vil ha mer informasjon, kan du se [Slik konfigurerer du passordwriteback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

## <a name="3-configure-hybrid-azure-ad-join"></a>3. Konfigurer Hybrid Azure AD Join

Før du aktiverer Windows 10-enheter som Hybrid Azure AD, må du kontrollere at du oppfyller følgende forutsetninger:

   - Du kjører den nyeste versjonen av Azure AD Connect.

   - Azure AD connect har synkronisert alle datamaskinobjektene til enhetene du vil være hybrid Azure AD sluttet. Hvis datamaskinobjektene tilhører bestemte organisasjonsenheter (OU), må du kontrollere at disse oUene også er angitt for synkronisering i Azure AD-tilkobling.

Hvis du vil registrere eksisterende domenetilknyttede Windows 10-enheter som Hybrid Azure AD ble koblet til, følger du fremgangsmåten i [opplæringen: Konfigurere hybrid Azure Active Directory-sammenføyning for administrerte domener](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Denne hybrid-aktiverer eksisterende lokale Active Directory sluttet Windows 10 datamaskiner og gjøre dem skyklar.
    
## <a name="4-enable-automatic-enrollment-for-windows-10"></a>4. Aktiver automatisk registrering for Windows 10

 Hvis du vil registrere Windows 10-enheter automatisk for administrasjon av mobilenheter i Intune, kan du se [Registrere en Windows 10-enhet automatisk ved hjelp av gruppepolicy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Du kan angi gruppepolicyen på lokalt datamaskinnivå, eller for masseoperasjoner, du kan bruke maler for gruppepolicybehandling og ADMX til å opprette denne gruppepolicyinnstillingen på domenekontrolleren.

## <a name="5-configure-seamless-single-sign-on"></a>5. Konfigurer sømløs enkel pålogging

  Sømløs SSO signerer automatisk brukere i Microsoft 365-skyressursene når de bruker firmadatamaskiner. Bare distribuer ett av de to gruppepolicyalternativene som er beskrevet i [Azure Active Directory Seamless Single Sign-On: Hurtigstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). **Alternativet Gruppepolicy** tillater ikke brukere å endre innstillingene sine, mens alternativet **Gruppepolicyinnstilling** angir verdiene, men lar dem også konfigureres.

## <a name="6-set-up-windows-hello-for-business"></a>6. Konfigurere Windows Hello for Bedrifter

 Windows Hello for Business erstatter passord med sterk tofaktorautentisering (2FA) for å logge på en lokal datamaskin. Den ene faktoren er et asymmetrisk nøkkelpar, og det andre er en PIN-kode eller annen lokal bevegelse, for eksempel fingeravtrykk eller ansiktsgjenkjenning hvis enheten støtter den. Vi anbefaler at du erstatter passord med 2FA og Windows Hello for Business der det er mulig.

Hvis du vil konfigurere Hybrid Windows Hello for Bedrifter, kan du se [hybridnøkkelklareringWindows Hello for Business Prerequisites](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Følg deretter instruksjonene i [Konfigurere innstillinger for hybrid Windows Hello for Business-nøkkelklarering](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
