---
title: Angi beskyttelsesinnstillinger for Windows 10 PC-er
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Lær mer om standard og andre innstillinger som er tilgjengelige i Microsoft 365 Business å sikre Windows 10 enheter.
ms.openlocfilehash: ebfe5f59e544b67e5a4f2ecd990031e9221ff8e5
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982146"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a>Angi beskyttelsesinnstillinger for Windows 10 PC-er

## <a name="secure-windows-10-devices"></a>Sikre Windows 10-enheter

Se en video om hvordan du kan sikre Windows 10-enheter med Microsoft 365 Business:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. Logg deg på [Microsoft 365 Business](https://portal.office.com) med legitimasjon for globaladministrator. 
    
2. velg **Legg til policy** på **Enhetspolicyer**-kortet i administratorportalen.
    
    ![Device policies card in the admin center.](media/27c12b61-d112-4348-b557-4f3e46204797.png)
  
3. Angi et unikt navn for denne policyen på **Legg til policy**-ruten. 
    
4. Velg **Windows 10-enhetskonfigurasjon** under **Policytype**.
    
5. Utvid **Sikre Windows 10-enheter** \> konfigurer innstillingene slik du ønsker. Se [Tilgjengelige innstillinger](protection-settings-for-windows-10-pcs.md#bkmk_availablesettings) for mer informasjon. 
    
    Du kan til enhver tid bruke **Tilbakestill standardinnstillinger**-koblingen for å gå tilbake til standardinnstillingen. 
    
    ![Add policy pane with Windows 10 Device configuration selected](media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Bestem deretter **Hvem får disse innstillingene?** Hvis du ikke vil bruke den standard sikkerhetsgruppen **Alle brukere**, velg **Endre**, søk etter sikkerhetsgruppen som vil få disse innstillingene \> **Velg**.
    
7. Velg til slutt **Ferdig** for å lagre policyen og tilordne den til enhetene. 
    
## <a name="available-settings"></a>Tilgjengelige innstillinger

Som standard er alle innstillingene **På**. Følgende innstillinger er tilgjengelige.
  
Se [Hvordan tilordnes beskyttelsesfunksjoner i Microsoft 365 Business til Intune-innstillinger](map-protection-features-to-intune-settings.md) for mer informasjon. 
  
|||
|:-----|:-----|
|Innstilling  <br/> |Beskrivelse  <br/> |
|Beskytte PC mot virus og andre trusler ved hjelp av Windows Defender Antivirus  <br/> |Krever at Windows Defender Antivirus er slått på for å beskytte PC-er fra farene ved å være koblet til Internett.  <br/> |
|Beskytte PC-er fra nettbaserte trusler i Microsoft Edge  <br/> |Slår på innstillinger i Microsoft Edge som beskytter brukere mot skadelige nettsteder og nedlastinger.  <br/> |
|Bruk regler som kan redusere angrepsoverflaten til enhetene  <br/> |Når reduksjon av angrepsoverflater er aktivert, er det med på å blokkere handlinger og apper som vanligvis brukes av skadelig programvare til å infisere enheter. Denne innstillingen er bare tilgjengelig hvis Windows Defender Antivirus er satt til På. Se [Redusere angrepsoverflater](https://go.microsoft.com/fwlink/?linkid=870417) for mer informasjon.  <br/> |
|Beskytte mapper mot trusler, for eksempel løsepengevirus  <br/> |Denne innstillingen bruker kontrollert mappetilgang til å beskytte firmadata mot endringer ved mistenkelige eller skadelige programmer, for eksempel løsepengevirus. Denne typen programmer hindres i å gjøre endringer i beskyttede mapper. Denne innstillingen er bare tilgjengelig hvis Windows Defender Antivirus er satt til På. Se [Beskytte mapper med styrt mappetilgang](https://go.microsoft.com/fwlink/?linkid=870418) for mer informasjon.  <br/> |
|Hindre nettverkstilgang til potensielt skadelig innhold på Internett  <br/> |Bruk denne innstillingen til å blokkere utgående brukertilkoblinger til steder på Internett med lavt omdømme, som kan være vert for phishingsvindel, utnyttelse eller annet skadelig innhold. Denne innstillingen er bare tilgjengelig hvis Windows Defender Antivirus er satt til På. Se [Beskytte nettverket](https://go.microsoft.com/fwlink/?linkid=870419) for mer informasjon.  <br/> |
|Bruke BitLocker til å beskytte filer og mapper på PC-er mot uautorisert tilgang  <br/> |BitLocker beskytter dataene ved å kryptere harddiskene på datamaskinen og beskytter mot eksponering av dataene dersom en datamaskin mistes eller blir stjålet. Se [Vanlige spørsmål om Bitlocker](https://go.microsoft.com/fwlink/?linkid=871000) for mer informasjon.  <br/> |
|Tillat brukere å laste ned apper fra Microsoft Store  <br/> |Lar brukere laste ned og installere apper fra Microsoft Store. Apper inkluderer alt fra spill til produktivitetsverktøy, så vi lar denne innstillingen være **På**, men du kan slå den av for ekstra sikkerhet.  <br/> |
|Gi brukere tilgang til Cortana  <br/> |Cortana kan være svært nyttig! Hun kan aktivere eller deaktivere innstillinger for deg, gi beskrivelser og passe på at du er tidsnok til avtaler, så vi lar denne innstillingen være **På** som standard.  <br/> |
|Tillat brukere å motta Windows-tips og annonser fra Microsoft  <br/> |Tips for Windows kan være praktisk, samt orientere brukere når nye funksjoner utgis.  <br/> |
|Holde Windows 10-enheter oppdatert automatisk  <br/> |Sørger for at Windows 10-enheter automatisk mottar de nyeste oppdateringene.  <br/> |
|Slå av skjermen på enheten når den har vært inaktiv i en viss periode  <br/> |Sørger for at bedriftsdata er beskyttet dersom en bruker er inaktiv. Det kan hende en bruker jobber på et offentlig sted, som eksempelvis en kaffebar, går bort eller blir distrahert et øyeblikk og lar enheten være sårbar for tilfeldig innsyn. Denne innstillingen lar deg bestemme hvor lenge en bruker kan være inaktiv før skjermen slås av.  <br/> |
   
  

