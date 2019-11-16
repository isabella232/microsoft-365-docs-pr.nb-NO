---
title: Angi beskyttelsesinnstillinger for Windows 10 PC-er
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Lær om standardinnstillingene og andre innstillinger som er tilgjengelige i Microsoft 365 Business for å sikre Windows 10-enheter.
ms.openlocfilehash: 5d4bce02df1276dc9b284c7b0709c7dc26b0dbce
ms.sourcegitcommit: 8ca97fa879ae4ea44468be629d6c32b429efeeec
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/16/2019
ms.locfileid: "38676052"
---
# <a name="set-device-protection-settings-for-windows-10-pcs"></a>Angi beskyttelsesinnstillinger for Windows 10 PC-er

## <a name="secure-windows-10-devices"></a>Sikre Windows 10-enheter

Se en video om hvordan du kan sikre Windows 10-enheter med Microsoft 365 Business:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. Gå til administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>. 
    
2. I den venstre navigasjonsenheten velger **du enhets** \> **policyer** \> **Legg til**.
  
3. Angi et unikt navn for denne policyen på **Legg til policy**-ruten. 
    
4. Velg **Windows 10-enhetskonfigurasjon** under **Policytype**.
    
5. Utvid **Sikre Windows 10-enheter** \> konfigurer innstillingene slik du ønsker. Se [Tilgjengelige innstillinger](#available-settings) for mer informasjon. 
    
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
|Bruk regler som kan redusere angrepsoverflaten til enhetene  <br/> |Når reduksjon av angrepsoverflater er aktivert, er det med på å blokkere handlinger og apper som vanligvis brukes av skadelig programvare til å infisere enheter. Denne innstillingen er bare tilgjengelig hvis Windows Defender Antivirus er satt til På. Se [Redusere angrepsoverflater](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/exploit-protection) for mer informasjon.  <br/> |
|Beskytte mapper mot trusler, for eksempel løsepengevirus  <br/> |Denne innstillingen bruker kontrollert mappetilgang til å beskytte firmadata mot endringer ved mistenkelige eller skadelige programmer, for eksempel løsepengevirus. Denne typen programmer hindres i å gjøre endringer i beskyttede mapper. Denne innstillingen er bare tilgjengelig hvis Windows Defender Antivirus er satt til På. Se [Beskytt mapper med tilgang styrt mappe](https://docs.microsoft.com/configmgr/protect/deploy-use/create-deploy-exploit-guard-policy#bkmk_CFA) for å finne ut mer.  <br/> |
|Hindre nettverkstilgang til potensielt skadelig innhold på Internett  <br/> |Bruk denne innstillingen til å blokkere utgående brukertilkoblinger til steder på Internett med lavt omdømme, som kan være vert for phishingsvindel, utnyttelse eller annet skadelig innhold. Denne innstillingen er bare tilgjengelig hvis Windows Defender Antivirus er satt til På. Se [Beskytte nettverket](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/configure-real-time-protection-windows-defender-antivirus) for mer informasjon.  <br/> |
|Bruke BitLocker til å beskytte filer og mapper på PC-er mot uautorisert tilgang  <br/> |BitLocker beskytter dataene ved å kryptere harddiskene på datamaskinen og beskytter mot eksponering av dataene dersom en datamaskin mistes eller blir stjålet. Se [Vanlige spørsmål om Bitlocker](https://go.microsoft.com/fwlink/?linkid=871000) for mer informasjon.  <br/> |
|Tillat brukere å laste ned apper fra Microsoft Store  <br/> |Lar brukere laste ned og installere apper fra Microsoft Store. Apper inkluderer alt fra spill til produktivitetsverktøy, så vi lar denne innstillingen være **På**, men du kan slå den av for ekstra sikkerhet.  <br/> |
|Gi brukere tilgang til Cortana  <br/> |Cortana kan være svært nyttig! Hun kan aktivere eller deaktivere innstillinger for deg, gi beskrivelser og passe på at du er tidsnok til avtaler, så vi lar denne innstillingen være **På** som standard.  <br/> |
|Tillat brukere å motta Windows-tips og annonser fra Microsoft  <br/> |Tips for Windows kan være praktisk, samt orientere brukere når nye funksjoner utgis.  <br/> |
|Holde Windows 10-enheter oppdatert automatisk  <br/> |Sørger for at Windows 10-enheter automatisk mottar de nyeste oppdateringene.  <br/> |
|Slå av skjermen på enheten når den har vært inaktiv i en viss periode  <br/> |Sørger for at bedriftsdata er beskyttet dersom en bruker er inaktiv. En bruker kan jobbe på et offentlig sted, som for eksempel en kaffebar, går bort eller blir distrahert i et øyeblikk, og lar enheten være sårbar for tilfeldig innsyn. Denne innstillingen lar deg bestemme hvor lenge en bruker kan være inaktiv før skjermen slås av.  <br/> |
   
  

