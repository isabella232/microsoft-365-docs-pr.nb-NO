---
title: Redigere eller opprette innstillinger for enhets beskyttelse for Windows 10-PC-er
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: bd66c26c-73a4-45a8-8642-3ea4ee7cd89d
description: Lær om innstillinger som er tilgjengelige i Microsoft 365 for bedrifter, for å sikre Windows 10-enheter.
ms.openlocfilehash: bd992113403c7134fb32bc6cced5bf216843241b
ms.sourcegitcommit: abf63669daf12993ad3353e4b578f41c8910b20f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/27/2020
ms.locfileid: "47289159"
---
# <a name="edit-or-create-device-protection-settings-for-windows-10-pcs"></a>Redigere eller opprette innstillinger for enhets beskyttelse for Windows 10-PC-er

Denne artikkelen gjelder for Microsoft 365 Business Premium.

Når du har konfigurert standard innstillingene for Windows-beskyttelse på konfigurasjons siden, kan du legge til nye som gjelder for enten alle brukere eller et sett med brukere. Du kan også redigere hvilke som helst av dem du har opprettet.

## <a name="create-protection-settings-for-windows-10-devices"></a>Opprette beskyttelses innstillinger for Windows 10-enheter

Vise en video om hvordan du kan sikre Windows 10-enheter med Microsoft 365 Business Premium:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/a5734146-620a-4cec-8618-536b3ca37972?autoplay=false]
  
1. Gå til administrasjons senteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. Velg **Devices** \> **Policies** \> **Legg til**enhets policyer i det venstre navigasjons feltet.
3. Angi et unikt navn for denne policyen på **Legg til policy**-ruten. 
4. Velg **Windows 10-enhetskonfigurasjon** under **Policytype**.
5. Utvid **Sikre Windows 10-enheter** \> konfigurer innstillingene slik du ønsker. Hvis du vil ha mer informasjon, kan du se [tilgjengelige innstillinger](#available-settings). 
    
    Du kan til enhver tid bruke **Tilbakestill standardinnstillinger**-koblingen for å gå tilbake til standardinnstillingen. 
    
    ![Add policy pane with Windows 10 Device configuration selected](../media/fa9e2dc2-7eae-4c96-af34-765a1f641ecf.png)
  
6. Bestem deretter **Hvem får disse innstillingene?** Hvis du ikke vil bruke den standard sikkerhetsgruppen **Alle brukere**, velg **Endre**, søk etter sikkerhetsgruppen som vil få disse innstillingene \> **Velg**.
7. Velg til slutt **Ferdig** for å lagre policyen og tilordne den til enhetene. 

## <a name="edit-windows-10-protection-settings"></a>Rediger innstillinger for beskyttelse mot Windows 10
 
1. Gå til administrasjons senteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. Velg **enhets** policyer i det venstre navigasjons feltet \> **Policies** .
1. Velg en eksisterende Windows-enhets policy, og **Rediger**deretter.
1. Velg **Rediger** ved siden av en innstilling du vil endre, og **Lagre**.

## <a name="available-settings"></a>Tilgjengelige innstillinger

Som standard er alle innstillingene **På**. Følgende innstillinger er tilgjengelige.
  
Hvis du vil ha mer informasjon, kan du se [Hvordan fungerer beskyttelses funksjoner i Microsoft 365 Premium Map til Intune-innstillinger](map-protection-features-to-intune-settings.md). 
  
|||
|:-----|:-----|
|Innstilling  <br/> |Beskrivelse  <br/> |
|Beskytte PC mot virus og andre trusler ved hjelp av Windows Defender Antivirus  <br/> |Krever at Windows Defender Antivirus er slått på for å beskytte PC-er fra farene ved å være koblet til Internett.  <br/> |
|Beskytte PC-er fra nettbaserte trusler i Microsoft Edge  <br/> |Slår på innstillinger i Microsoft Edge som beskytter brukere mot skadelige nettsteder og nedlastinger.  <br/> |
|Bruk regler som kan redusere angrepsoverflaten til enhetene  <br/> |Når reduksjon av angrepsoverflater er aktivert, er det med på å blokkere handlinger og apper som vanligvis brukes av skadelig programvare til å infisere enheter. Denne innstillingen er bare tilgjengelig hvis Windows Defender Antivirus er satt til På. Se [Redusere angrepsoverflater](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/exploit-protection) for mer informasjon.  <br/> |
|Beskytte mapper mot trusler, for eksempel løsepengevirus  <br/> |Denne innstillingen bruker kontrollert mappetilgang til å beskytte firmadata mot endringer ved mistenkelige eller skadelige programmer, for eksempel løsepengevirus. Denne typen programmer hindres i å gjøre endringer i beskyttede mapper. Denne innstillingen er bare tilgjengelig hvis Windows Defender Antivirus er satt til På. Se [beskytte mapper med kontrollert mappe tilgang](https://docs.microsoft.com/mem/configmgr/protect/deploy-use/create-deploy-exploit-guard-policy#bkmk_CFA) for å lære mer.  <br/> |
|Hindre nettverkstilgang til potensielt skadelig innhold på Internett  <br/> |Bruk denne innstillingen til å blokkere utgående bruker tilkoblinger til Internett-plasseringer med et lavt omdømme som kan være vert for svindel forsøk, utnyttelser eller annen skadelig innhold. Denne innstillingen er bare tilgjengelig hvis Windows Defender antivirus er satt til **på**. Hvis du vil ha mer informasjon, kan du se [Beskytt nettverket ditt](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/configure-real-time-protection-windows-defender-antivirus).  <br/> |
|Bruke BitLocker til å beskytte filer og mapper på PC-er mot uautorisert tilgang  <br/> |BitLocker beskytter dataene ved å kryptere harddiskene på datamaskinen og beskytter mot eksponering av dataene dersom en datamaskin mistes eller blir stjålet. Du finner mer informasjon i [vanlige spørsmål om BitLocker](https://go.microsoft.com/fwlink/?linkid=871000).  <br/> |
|Tillat brukere å laste ned apper fra Microsoft Store  <br/> |Lar brukere laste ned og installere apper fra Microsoft Store. Apper inkluderer alt fra spill til produktivitetsverktøy, så vi lar denne innstillingen være **På**, men du kan slå den av for ekstra sikkerhet.  <br/> |
|Gi brukere tilgang til Cortana  <br/> |Cortana kan være svært nyttig! Cortana kan aktivere eller deaktivere innstillingene for deg, gi vei beskrivelser og kontrollere at du er på tide for avtaler, slik at vi beholder **denne innstillingen som** standard.  <br/> |
|Tillat brukere å motta Windows-tips og annonser fra Microsoft  <br/> |Tips for Windows kan være praktisk, samt orientere brukere når nye funksjoner utgis.  <br/> |
|Holde Windows 10-enheter oppdatert automatisk  <br/> |Sørger for at Windows 10-enheter automatisk mottar de nyeste oppdateringene.  <br/> |
|Slå av skjermen på enheten når den har vært inaktiv i en viss periode  <br/> |Sørger for at bedriftsdata er beskyttet dersom en bruker er inaktiv. En bruker kan jobbe på et offentlig sted, som for eksempel en kaffebar, går bort eller blir distrahert i et øyeblikk, og lar enheten være sårbar for tilfeldig innsyn. Denne innstillingen lar deg bestemme hvor lenge en bruker kan være inaktiv før skjermen slås av.  <br/> |
