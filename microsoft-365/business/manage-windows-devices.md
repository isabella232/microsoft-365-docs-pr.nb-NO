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
ms.openlocfilehash: 5cce4bc53f118560e31ad7e6048e4efcb49d662e
ms.sourcegitcommit: c0f769244d05ad019ea2307c38d5543d7b1e5afd
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992233"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business

Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business for å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgang til lokale ressurser som krever lokal godkjenning. Du kan konfigurere dette ved først å synkronisere Active Directory med Azure Active Directory, etterfulgt av å registrere Windows 10-enhetene med Azure AD og registrere dem for administrasjon av mobilenheter av Microsoft 365 Business.
Følgende video beskriver fremgangsmåten for hvordan du konfigurerer dette for det vanligste scenarioet.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Konfigurere enheter som er tilknyttet et domene, som skal administreres av Microsoft 365 Business

Hvis du vil konfigurere organisasjonens domenetilknyttede enheter til å dra nytte av funksjonene som tilbys av Azure Active Directory i tillegg til lokale Active Directory, kan du implementere **hybrid Azure ad koblet enheter**. Dette er enheter som er koblet både til den lokale Active Directory og Azure Active Directory. Hybrid Azure AD-enheter som er koblet til, kan beskyttes og administreres av Microsoft 365 Business. 
  
Følg fremgangsmåten nedenfor for å gjøre Windows 10-enhetene dine hybrid Azure AD koblet sammen og administrert av Microsoft 365 Business.
  
1. Hvis du vil synkronisere brukere, grupper og kontakter fra lokal Active Directory til Azure Active Directory, kjører du veiviseren for katalogsynkronisering og Azure Active Directory Connect som beskrevet i [Konfigurere katalogsynkronisering for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
    > [!NOTE]
    > Fremgangsmåten er nøyaktig den samme for Microsoft 365 Business. 
  
2. Før du fullfører trinn 3 for å aktivere Windows 10-enheter skal hybrid Azure AD ble med, må du kontrollere at du oppfyller følgende forutsetninger:

   - Du kjører den nyeste versjonen av Azure AD-tilkobling.

   - Azure AD-tilkobling har synkronisert alle datamaskinobjekter for enhetene du vil skal være hybrid Azure AD ble med. Hvis datamaskinobjektene tilhører bestemte organisasjonsenheter (OU), må du kontrollere at disse organisasjonsenhetene er angitt for synkronisering i Azure AD-tilkobling også.
    
3. Registrere eksisterende domenetilknyttede Windows 10-enheter for å være hybrid Azure AD ble med og registrere dem for administrasjon av mobile enheter ved Intune (Microsoft 365 Business):
    
4. Følg de trinnvise instruksjonene i [hvordan du konfigurerer hybrid Azure Active Directory-sammenkoblede enheter](https://go.microsoft.com/fwlink/p/?linkid=872870). Dette vil gjøre det mulig synkronisering av lokale Active Directory koblet til Windows 10-datamaskiner og gjøre dem Sky klar.
    
5. Hvis du vil registrere en Windows 10-enhet for administrasjon av mobile enheter, kan du se [registrere en Windows 10-enhet med Intune ved hjelp av en gruppe policy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instruksjoner. Du kan angi gruppepolicy på et lokalt datamaskinnivå eller for masseoperasjoner, kan du opprette denne gruppepolicyinnstillingen på serveren for domenekontrolleren.