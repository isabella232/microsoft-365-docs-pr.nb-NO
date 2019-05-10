---
title: Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
description: Lær hvordan du aktiverer Microsoft 365 å beskytte lokale AD sammen Windows 10 enheter.
ms.openlocfilehash: 661e5bf8205a661eb4382b4bdd8fcf3a54ecc12f
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660345"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business"></a>Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business

Hvis organisasjonen bruker Windows Server Active Directory på lokaler, kan du definere Microsoft 365 Business til å beskytte Windows 10 enheter, samtidig som du har tilgang til lokale ressurser som krever lokal godkjenning. Du kan definere dette ved første synkronisering av Active Directory med Azure Active Directory, etterfulgt av registrering 10 Windows-enheter med Azure AD og melde deg dem for mobilenhet administrasjon av Microsoft 365 Business.
  
## <a name="set-up-domain-joined-devices-to-be-managed-by-microsoft-365-business"></a>Angi domenetilknyttede enheter skal administreres av Microsoft 365 Business

Hvis du vil konfigurere organisasjonens domenetilknyttede enheter til å dra nytte av mulighetene som gis av Azure Active Directory i tillegg til lokale Active Directory, kan du implementere **Hybrid Azure AD koblet enheter**. Dette er enheter som er koblet til både den lokale Active Directory og Azure Active Directory. Hybrid Azure AD koblet enheter kan beskyttet og administreres av Microsoft 365 Business. 
  
Fullfør fremgangsmåten nedenfor for å gjøre Windows 10 enheter Hybrid Azure AD sammen og administreres av Microsoft 365 Business.
  
1. For å synkronisere brukere, grupper og kontakter fra lokal Active Directory til Azure Active Directory, kan du kjøre veiviseren for synkronisering av katalog og Azure Active Directory koble som beskrevet i [konfigurere katalogsynkronisering for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
    > [!NOTE]
    > Trinnene er nøyaktig den samme for Microsoft 365 Business. 
  
2. Før du fullfører trinn 3 for å aktivere Windows 10 enheter skal være Hybrid Azure AD sammenføyd, må du kontrollere at du oppfyller følgende forutsetninger:

   - Du kjører den nyeste versjonen av Azure AD koble.

   - Koble Azure AD har synkronisert alle datamaskinobjekter for enhetene du vil skal være hybrid Azure AD sammen. Hvis objektene som datamaskinen hører til bestemte organisasjonsenheter (OU), og deretter kontrollerer disse organisasjonsenheter som er angitt for synkronisering i Azure AD koble også.
    
3. Registrere eksisterende domenetilknyttede Windows 10 enheter hybrid Azure AD JOIN og registrere dem for mobil enhet management ved Intune (Microsoft 365 Business):
    
4. Følg trinnvise instruksjoner om [hvordan du konfigurerer hybrid Azure Active Directory sammen enheter](https://go.microsoft.com/fwlink/p/?linkid=872870). Dette vil aktivere synkronisering av lokale Active Directory sammen Windows 10 datamaskiner og gjøre dem klar for sky.
    
5. Hvis du vil registrere en Windows 10 enhet for behandling av mobil enhet, kan du se [registrere en Windows 10 enhet med Intune ved hjelp av en gruppepolicy](https://go.microsoft.com/fwlink/p/?linkid=872871) for instruksjoner. Du kan angi gruppepolicyen på en lokal datamaskin eller for masseoperasjoner, kan du opprette denne innstillingen for gruppepolicy på domenet-kontrollerserver.