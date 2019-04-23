---
title: Angi innstillinger for programbeskyttelse for Windows 10-enheter
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- Win10AppPolicy
- O365E_Win10AppPolicy
- BCS365_Win10AppPolicy
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Lær hvordan du oppretter en policy for informasjonsbehandling av app og beskytte arbeidsfiler på Windows 10 enheter.
ms.openlocfilehash: 289c6a74f6ccb53f6a833612a7b4a5bcddd3ea56
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32278188"
---
# <a name="set-application-protection-settings-for-windows-10-devices"></a>Angi innstillinger for programbeskyttelse for Windows 10-enheter

## <a name="create-an-app-management-policy-for-windows-10"></a>Opprette en policy for appbehandling for Windows 10

Hvis brukerne har personlige Windows 10-enheter der de utfører arbeidsoppgaver, kan du beskytte dataene dine på disse enhetene i tillegg.
  
1. Logg på [administrasjonssenteret](https://go.microsoft.com/fwlink/p/?linkid=837890) med global admin-legitimasjon. Velg **Administrasjon**-flisen for å gå til administrasjonssenteret. 
    
2. Velg **enheter** på venstre nav, \> **policyer** \> **Legg til**.

3. Angi et unikt navn for denne policyen i **Legg til Policy**-ruten. 
    
4. Velg **Programbehandling for Windows 10** under **Policytype**.
    
5. Under ** Device type **, choose either **Personal** or **Company Owned**.
    
6. **Krypter arbeidsfiler** aktiveres automatisk. 
    
7. Sett **Forhindre brukere fra å kopiere bedriftsdata til personlige filer, og tvinge dem til å lagre arbeidsfiler til OneDrive for Business** til **På** hvis du ikke vil at brukerne skal lagre arbeidsfiler på PCen. 
    
8. Utvid **Administrer hvordan brukere får tilgang til Office-filer på enheter** \> konfigurer innstillingene slik du ønsker. **Administrer hvordan brukere får tilgang til Office-enheter på mobile enheter** er slått **Av** som standard, men det anbefales at du slår den **På** og godtar standardverdiene. Hvis du vil ha mer informasjon, kan du se [tilgjengelige innstillinger](#available-settings). 
    
    Du kan til enhver tid bruke **Tilbakestill standardinnstillinger**-koblingen for å gå tilbake til standardinnstillingen. 
    
9. Utvid **Gjenopprett data på Windows-enheter**, og det anbefales også at du slår den **På**.
    
    Før du kan bla til plasseringen av Sertifikatet for datagjenopprettingsagent, må du først opprette ett. For nærmere instruksjoner kan du se [Opprett og bekreft et sertifikat for datagjenopprettingsagent for EFS (Encrypting File System)](https://go.microsoft.com/fwlink/p/?linkid=853700).
    
    Som standard blir arbeidsfiler kryptert ved hjelp av en hemmelig nøkkel som er lagret på enheten og knyttet til brukerens profil. Bare brukeren kan åpne og dekryptere filen. Men hvis en enhet mistes eller en bruker fjernes, kan en fil bli sittende fast i en kryptert tilstand. En administrator kan bruke sertifikatet for datagjenopprettingsagenten til å dekryptere filen.
    
    ![Browse to Data Recovery Agent certificate.](media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Utvid **Beskytt ekstra nettverk og skyplasseringer** hvis du vil legge til flere domener eller SharePoint Online-områder, for å sikre at filene i alle oppførte apper blir beskyttet. Hvis du trenger å angi mer enn ett element for hvert felt, kan du bruke semikolon (;) mellom elementene. 
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Bestem deretter **Hvem får disse innstillingene?** Hvis du ikke vil bruke den standard sikkerhetsgruppen **Alle brukere**, velger du **Endre** og deretter sikkerhetsgruppene som vil få disse innstillingene \> **Velg**.
    
12. Velg til slutt **Legg til** for å lagre policyen og tilordne den til enhetene. 
    
## <a name="available-settings"></a>Tilgjengelige innstillinger

De følgende innstillingene er tilgjengelige for å administrere hvordan brukere får tilgang til Office-arbeidsfiler.
  
Hvis du vil ha mer informasjon, kan du se [Slik tilordnes beskyttelsesfunksjoner i Microsoft 365 Business til Intune-innstillinger](map-protection-features-to-intune-settings.md).
  
|**Innstilling**|**Beskrivelse**|
|:-----|:-----|
|Kreve en PIN-kode eller et fingeravtrykk for å få tilgang til Office-apper  <br/> |Hvis disse innstillingene er **På**, må brukere gi en annen form for godkjenning, i tillegg til brukernavn og passord, før de kan bruke Office-apper på mobilenheten.  <br/> |
|Tilbakestille PIN-kode når påloggingen mislykkes et visst antall ganger  <br/> |Hvis du vil forhindre at en uautorisert bruker tilfeldig gjetter en PIN-kode, tilbakestilles PIN-koden etter det antallet feiloppføringer du angir.  <br/> |
|Kreve at brukere logger seg på igjen etter at Office-apper har vært inaktive i  <br/> |Denne innstillingen bestemmer hvor lenge en bruker kan være inaktiv før de blir bedt om å logge seg på igjen.  <br/> |
   

