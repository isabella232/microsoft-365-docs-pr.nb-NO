---
title: Redigere eller angi innstillinger for programbeskyttelse for Windows 10-enheter
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
description: Lær hvordan du oppretter eller redigerer policyer for appbehandling og beskytter arbeidsfiler på brukernes personlige Windows 10-enheter.
ms.openlocfilehash: aa270c563e6bdce6fd48f8713d7db3ce23921925
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580018"
---
# <a name="set-or-edit-application-protection-settings-for-windows-10-devices"></a>Angi eller redigere innstillinger for programbeskyttelse for Windows 10-enheter

Denne artikkelen gjelder for Microsoft 365 Business Premium.

## <a name="edit-an-app-management-policy-for-windows-10"></a>Redigere en policy for appbehandling for Windows 10

1. Gå til administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .     
2. Velg Enheter policyer **til** \> **venstre.**
1. Velg en eksisterende policy for Windows-appen, og velg deretter **Rediger**.
1. Velg **Rediger** ved siden av en innstilling du vil endre, og velg deretter **Lagre**.

## <a name="create-an-app-management-policy-for-windows-10"></a>Opprette en policy for appbehandling for Windows 10

Hvis brukerne har personlige Windows 10-enheter der de utfører arbeidsoppgaver, kan du beskytte dataene dine på disse enhetene i tillegg.
  
1. Gå til administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> . 
2. Velg Legg til  enheter \> **policyer til** \> **venstre.**
3. Angi et unikt navn for denne policyen i **Legg til Policy**-ruten. 
4. Velg **Programbehandling for Windows 10** under **Policytype**.
5. Velg **Personlig eller**  Firmaeid under **Enhetstype**.
6. **Krypter arbeidsfiler** aktiveres automatisk. 
7. Sett **Forhindre brukere fra å kopiere bedriftsdata til personlige filer, og tvinge dem til å lagre arbeidsfiler til OneDrive for Business** til **På** hvis du ikke vil at brukerne skal lagre arbeidsfiler på PCen. 
9. Utvid **Gjenopprett data på Windows-enheter**. Vi anbefaler at du slår den **på**.
    Før du kan bla til plasseringen av Sertifikatet for datagjenopprettingsagent, må du først opprette ett. Hvis du vil ha instruksjoner, kan du se Opprette og [bekrefte et EFS-sertifikat (Encrypting File System) Data Recovery Agent (DRA).](/windows/security/information-protection/windows-information-protection/create-and-verify-an-efs-dra-certificate)
    
    Som standard blir arbeidsfiler kryptert ved hjelp av en hemmelig nøkkel som er lagret på enheten og knyttet til brukerens profil. Bare brukeren kan åpne og dekryptere filen. Men hvis en enhet mistes eller en bruker fjernes, kan en fil bli sittende fast i en kryptert tilstand. En administrator kan bruke datagjenopprettingsagentsertifikatet (DRA) til å dekryptere filen.
    
    ![Browse to Data Recovery Agent certificate.](../media/7d7d664f-b72f-4293-a3e7-d0fa7371366c.png)
  
10. Utvid **Beskytt flere nettverks-** og skyplasseringer hvis du vil legge til flere domener eller SharePoint Online-plasseringer for å sikre at filene i alle de oppførte appene er beskyttet. Hvis du trenger å angi mer enn ett element for hvert felt, kan du bruke semikolon (;) mellom elementene.
    
    ![Expand Protect additional network and cloud locations, and enter domains or SharePoint Online sites you own.](../media/7afaa0c7-ba53-456d-8c61-312c45e09625.png)
  
11. Bestem deretter **Hvem får disse innstillingene?** Hvis du ikke vil bruke den standard sikkerhetsgruppen **Alle brukere**, velger du **Endre** og deretter sikkerhetsgruppene som vil få disse innstillingene \> **Velg**.
12. Velg til slutt **Legg til** for å lagre policyen og tilordne den til enhetene.