---
title: Redigere eller angi innstillinger for program beskyttelse for Windows 10-enheter
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: 02e74022-44af-414b-9d74-0ebf5c2197f0
description: Lær hvordan du oppretter eller redigerer policyer for appbehandling og beskytter arbeids filer på brukernes personlige Windows 10-enheter.
ms.openlocfilehash: f85a59649e43c141b62091337b842a490d411833
ms.sourcegitcommit: abf63669daf12993ad3353e4b578f41c8910b20f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/27/2020
ms.locfileid: "47289203"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a>Angi eller redigere innstillinger for program beskyttelse for Windows 10-enheter

Denne artikkelen gjelder for Microsoft 365 Business Premium.

## <a name="edit-an-app-management-policy-for-windows-10"></a>Redigere en policy for app-behandling for Windows 10

1. Gå til administrasjons senteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. Velg **enhets** policyer i det venstre navigasjons feltet \> **Policies** .
1. Velg en eksisterende policy for Windows-apper, og **Rediger**deretter.
1. Velg **Rediger** ved siden av en innstilling du vil endre, og **Lagre**.

## <a name="create-an-app-management-policy-for-windows-10"></a>Opprette en policy for appbehandling for Windows 10

Hvis brukerne har personlige Windows 10-enheter der de utfører arbeidsoppgaver, kan du beskytte dataene dine på disse enhetene i tillegg.
  
1. Gå til administrasjons senteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. Velg **Devices** \> **Policies** \> **Legg til**enhets policyer i det venstre navigasjons feltet.
3. Angi et unikt navn for denne policyen i **Legg til Policy**-ruten. 
4. Velg **Programbehandling for Windows 10** under **Policytype**.
5. Velg enten **personlig** eller **firmaet som eies**under **enhets type**.
6. **Krypter arbeidsfiler** aktiveres automatisk. 
7. Sett **Forhindre brukere fra å kopiere bedriftsdata til personlige filer, og tvinge dem til å lagre arbeidsfiler til OneDrive for Business** til **På** hvis du ikke vil at brukerne skal lagre arbeidsfiler på PCen. 
9. Utvid **Gjenopprett data på Windows-enheter**. Vi anbefaler at du slår det **på**.
    Før du kan bla til plasseringen av Sertifikatet for datagjenopprettingsagent, må du først opprette ett. Hvis du vil ha instruksjoner, kan du se [opprette og bekrefte et EFS-sertifikat (Encrypting File System) for data gjenopprettings agent](https://go.microsoft.com/fwlink/p/?linkid=853700).
    
    Som standard blir arbeidsfiler kryptert ved hjelp av en hemmelig nøkkel som er lagret på enheten og knyttet til brukerens profil. Bare brukeren kan åpne og dekryptere filen. Men hvis en enhet mistes eller en bruker fjernes, kan en fil bli sittende fast i en kryptert tilstand. En administrator kan bruke DRA-sertifikatet (Data Recovery agent) til å dekryptere filen.
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Utvid **Beskytt flere nettverk og Sky plasseringer** hvis du vil legge til flere domener eller SharePoint Online-plasseringer for å sikre at filene i alle de oppførte appene er beskyttet. Hvis du trenger å angi mer enn ett element for hvert felt, kan du bruke semikolon (;) mellom elementene.
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Bestem deretter **Hvem får disse innstillingene?** Hvis du ikke vil bruke den standard sikkerhetsgruppen **Alle brukere**, velger du **Endre** og deretter sikkerhetsgruppene som vil få disse innstillingene \> **Velg**.
12. Velg til slutt **Legg til** for å lagre policyen og tilordne den til enhetene. 
