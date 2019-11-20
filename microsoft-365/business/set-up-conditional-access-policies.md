---
title: Definer policyer for betinget tilgang for Microsoft 365-kampanjer
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
- MOE150
description: Lær hvordan du konfigurerer policyer for betinget tilgang for Microsoft 365-kampanjer.
ms.openlocfilehash: aebdb733c2dd9a05947335ad4f151104d801568e
ms.sourcegitcommit: 6a413a65b8c2e10cea08f0a15635b28a1362a582
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/19/2019
ms.locfileid: "38718833"
---
# <a name="set-up-conditional-access-policies"></a>Definere policyer for betinget tilgang

Policyer for [betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) legger til betydelig ekstra sikkerhet. Microsoft tilbyr et sett med policyer for betinget tilgang som er anbefalt for alle kunder. Policyer for grunnlinje er et sett med forhåndsdefinerte policyer som bidrar til å beskytte organisasjoner mot mange vanlige angrep. Disse vanlige angrepene kan inkludere passord spray, Replay og phishing.

Disse policyene krever at administratorer og brukere angir en annen form for godkjenning (kalt multifaktor-godkjenning eller MFA) når visse betingelser er oppfylt. Hvis en bruker for eksempel logger på fra et annet land, kan påloggingen betraktes som risikabelt, og brukeren må angi en ekstra form for godkjenning. 

Policyer for opprinnelig plan inkluderer følgende:
- **Krev MFA for administratorer** &ndash; krever godkjenning med flere faktorer for de mest privilegerte administratorrollene, inkludert global administrator.
- **Sluttbruker beskyttelse** &ndash; krever multifaktorautentisering bare for brukere når en pålogging er risikabelt. 
- **Blokker** &ndash; eldre klientprogrammer og noen nye apper bruker ikke nyere, sikrere godkjenningsprotokoller. Disse eldre appene kan omgå policyer for betinget tilgang og få uautorisert tilgang til miljøet ditt. Denne policyen blokkerer tilgang fra klienter som ikke støtter betinget tilgang. 
- **Krev MFA for Service Management** &ndash; krever multifaktorautentisering for tilgang til administrasjonsverktøy, inkludert Azure Portal (der du konfigurerer policyer for opprinnelig plan). 

Microsoft anbefaler at du aktiverer alle disse grunnlinje policyene. Når disse policyene er aktivert, blir administratorer og brukere bedt om å registrere seg for Azure Multii-Factor-godkjenning.

Hvis du vil ha mer informasjon om disse policyene, kan du se [Hva er policyer for opprinnelig plan](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Definere policyer for opprinnelig plan

1. Gå til [Azure Portal](https://portal.azure.com), og naviger deretter til **Azure Active Directory** \> - **betinget tilgang**.
    
    De opprinnelige policyene er oppført på siden. <br/> <br/>
    ![Side som viser en liste over opprinnelige policyer for betinget tilgang.](media/baslinepolicies.png)
1. Se følgende spesifikke instruksjoner for hver policy:

  - [Krev MFA for administratorer](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Krev MFA for brukere](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Blokker eldre godkjenning](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Krev MFA for servicestyring](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Du kan definere mange tilleggs policyer, for eksempel å kreve godkjente klientprogrammer. Hvis du vil ha mer informasjon, se [dokumentasjonen for betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/).
