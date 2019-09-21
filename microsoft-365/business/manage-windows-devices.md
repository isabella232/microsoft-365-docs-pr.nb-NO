---
title: Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: 9b4de218-f1ad-41fa-a61b-e9e8ac0cf993
description: Lær hvordan du aktiverer Microsoft 365 for å beskytte lokale AD ble koblet til Windows 10-enheter.
ms.openlocfilehash: 9bfd540c0ff113762485f62707f1975ff53accc4
ms.sourcegitcommit: 1162d676b036449ea4220de8a6642165190e3398
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068109"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business

Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business for å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgang til lokale ressurser som krever lokal godkjenning. Du kan konfigurere dette ved først å synkronisere Active Directory med Azure Active Directory, etterfulgt av å registrere Windows 10-enhetene med Azure AD og registrere dem for administrasjon av mobilenheter av Microsoft 365 Business.
Følgende video beskriver fremgangsmåten for hvordan du konfigurerer dette for det vanligste scenarioet.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Konfigurere enheter som er tilknyttet et domene, som skal administreres av Microsoft 365 Business

Hvis du vil konfigurere organisasjonens domenetilknyttede enheter til å dra nytte av funksjonene som tilbys av Azure Active Directory i tillegg til lokale Active Directory, kan du implementere **hybrid Azure ad koblet enheter**. Dette er enheter som er koblet både til den lokale Active Directory og Azure Active Directory. Hybrid Azure AD-enheter som er koblet til, kan beskyttes og administreres av Microsoft 365 Business. 
  
Følg fremgangsmåten nedenfor for å gjøre Windows 10-enhetene dine hybrid Azure AD koblet sammen og administrert av Microsoft 365 Business.
  
1. **Klargjøre for katalogsynkronisering**: før du synkroniserer brukere og datamaskiner fra det lokale Active Directory-domenet, må du se [klargjøre for katalogsynkronisering til Office 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Spesielt:

   - Kontroller at det ikke finnes duplikater i katalogen for følgende attributter: **mail**, **physicalDeliveryOfficeName**og **userPrincipalName**. Disse verdiene må være unike, og alle duplikater bør fjernes..
   
   - Vi anbefaler at attributtet **userPrincipalName** (UPN) for hver lokale brukerkonto er konfigurert til å samsvare med den primære e-postadressen som tilsvarer den lisensierte Microsoft 365-brukeren. For eksempel **Mary.Shelley@contoso.com** i stedet for **Mary @ contoso. local**
   
   - Hvis Active Directory-domenet slutter på en ikke-rutes suffiks som **. local** eller **. LAN**, i stedet for et Internett rutes suffiks som **. com** eller **. org**, må du justere UPN-suffikset for de lokale brukerkontoene først som beskrevet i [Klargjør et domene som ikke skal rutes for katalogsynkronisering](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

2. **Installere og konfigurere Azure ad-tilkobling**: Hvis du vil synkronisere brukere, grupper og kontakter fra den lokale Active Directory til Azure Active Directory, kjører du veiviseren for katalogsynkronisering fra Azure Active Directory-tilkobling. Se [Konfigurere katalogsynkronisering for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) for å finne ut mer.
    
    > [!NOTE]
    > Fremgangsmåten er nøyaktig den samme for Microsoft 365 Business. 
    
Når du konfigurerer alternativene for Azure AD-tilkobling, anbefaler vi at du aktiverer **synkronisering av passord** og **sømløs enkel pålogging**, i tillegg til funksjonen for **passord writeback** , som også støttes i Microsoft 365 Business.

> [!NOTE]
> Det er noen ekstra trinn for passord writeback utover avmerkingsboksen i Azure AD-tilkobling. Se [How-to: konfigurere passord writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 
     
3. **Konfigurere hybrid Azure ad sammenføyning**: før du aktiverer Windows 10-enheter til å være hybrid Azure ad ble med, må du kontrollere at du oppfyller følgende forutsetninger:

   - Du kjører den nyeste versjonen av Azure AD-tilkobling.

   - Azure AD-tilkobling har synkronisert alle datamaskinobjekter for enhetene du vil skal være hybrid Azure AD ble med. Hvis datamaskinobjektene tilhører bestemte organisasjonsenheter (OU), må du kontrollere at disse organisasjonsenhetene er angitt for synkronisering i Azure AD-tilkobling også.

Hvis du vil registrere eksisterende domenetilknyttede Windows 10-enheter som hybrid Azure AD ble med, følger du fremgangsmåten i [opplæringen: konfigurere hybrid Azure Active Directory-sammenføyning for administrerte domener](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). Dette vil hybrid-aktivere din eksisterende lokale Active Directory sluttet Windows 10 datamaskiner og gjøre dem Sky klar.
    
4. **Aktiver automatisk registrering for Windows 10**: Hvis du vil registrere Windows 10-enheter for mobilenhetsbehandling automatisk i Intune, kan du se [registrere en Windows 10-enhet automatisk ved hjelp av gruppe policy](https://docs.microsoft.com/windows/client-management/mdm/enroll-a-windows-10-device-automatically-using-group-policy). Du kan angi gruppepolicy på et lokalt datamaskinnivå, eller for masseoperasjoner, kan du opprette denne gruppepolicyinnstillingen på domenekontrolleren ved hjelp av Group Policy Management Console og ADMX-maler.

5. **Konfigurer sømløs enkel pålogging**: sømløs SSO vil automatisk logge brukere inn i deres Microsoft 365 skyressurser når de bruker bedriftens datamaskiner. Distribuer enkelt ett av de to gruppe policy alternativene som er beskrevet i [Azure Active Directory sømløs enkel pålogging: hurtigst Start](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-2-enable-the-feature). Alternativet **Gruppepolicy** tillater ikke at brukere endrer innstillingene, mens alternativet **gruppepolicyinnstilling** angir verdiene, men lar dem også konfigureres av brukeren.

6. **Konfigurere Windows Hello for bedrifter**: Windows Hello for Business erstatter passord med sterk totrinnsverifisering (2FA) for å logge på en lokal datamaskin. Én faktor er et asymmetrisk nøkkelpar, og det andre er en PIN-kode eller annen lokal bevegelse, for eksempel fingeravtrykk eller ansiktsgjenkjenning, hvis enheten støtter det. Vi anbefaler at du erstatter passord med 2FA og Windows Hello for bedrifter der det er mulig.

Hvis du vil konfigurere hybrid Windows Hello for bedrifter, kan du se gjennom [hybrid nøkkel klarering Windows Hello for Business forutsetninger](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-trust-prereqs). Følg deretter instruksjonene for å [konfigurere innstillinger for nøkkel klarering for hybrid Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-key-whfb-settings). 
