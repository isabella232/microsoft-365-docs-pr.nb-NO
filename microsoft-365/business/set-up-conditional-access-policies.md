---
title: Konfigurere policyer for betinget tilgang for Microsoft 365-kampanjer
f1.keywords:
- NOCSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
description: Finn ut hvordan du konfigurerer policyer for betinget tilgang for Microsoft 365-kampanjer for å legge til betydelig ekstra sikkerhet.
ms.openlocfilehash: 58ee760877ee2fd7e53ef9463242657ab66a2b6e
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/01/2020
ms.locfileid: "44470651"
---
# <a name="set-up-conditional-access-policies"></a>Definere policyer for betinget tilgang

Denne artikkelen gjelder for Microsoft 365 Business Premium.

[Policyer for betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) gir betydelig ekstra sikkerhet. Microsoft inneholder et sett med policyer for betinget tilgang for opprinnelig plan som anbefales for alle kunder. Grunnleggende policyer er et sett med forhåndsdefinerte policyer som bidrar til å beskytte organisasjoner mot mange vanlige angrep. Disse vanlige angrepene kan omfatte passordspray, reprise og phishing.

Disse policyene krever at administratorer og brukere angir en annen form for godkjenning (kalt multifaktorautentisering eller MFA) når visse betingelser er oppfylt. Hvis en bruker for eksempel logger på fra et annet land, kan påloggingen anses som risikabelt, og brukeren må gi en ekstra form for godkjenning. 

Retningslinjer for opprinnelig plan omfatter for øyeblikket følgende:
- **Krev MFA for administratorer** &ndash; Krever godkjenning med flere faktorer for de mest privilegerte administratorrollene, inkludert global administrator.
- **Beskyttelse mot sluttbrukere** &ndash; Krever godkjenning med flere faktorer bare for brukere når en pålogging er risikabel. 
- **Blokkere eldre godkjenning** &ndash; Eldre klientapper og enkelte nye apper bruker ikke nyere, sikrere godkjenningsprotokoller. Disse eldre appene kan omgå policyer for betinget tilgang og få uautorisert tilgang til miljøet ditt. Denne policyen blokkerer tilgang fra klienter som ikke støtter betinget tilgang. 
- **Krev MFA for serviceadministrasjon** &ndash; Krever godkjenning med flere faktorer for tilgang til administrasjonsverktøy, inkludert Azure-portalen (der du konfigurerer grunnleggende policyer). 

Microsoft anbefaler at du aktiverer alle disse policyene for opprinnelige plan. Når disse policyene er aktivert, blir administratorer og brukere bedt om å registrere seg for Azure Multii-Factor-godkjenning.

Hvis du vil ha mer informasjon om disse policyene, kan du se [Hva er policyer for opprinnelig plan](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Definere opprinnelige policyer

1. Gå til [Azure-portalen](https://portal.azure.com), og naviger deretter til **Betinget Azure Active** \> **Directory-tilgang**.
    
    De opprinnelige policyene er oppført på siden. <br/> <br/>
    ![Side som viser opprinnelige policyer for betinget tilgang.](../media/baslinepolicies.png)
1. Se følgende spesifikke instruksjoner for hver policy:

  - [Krev MFA for administratorer](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Krev MFA for brukere](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Blokkere eldre godkjenning](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Krev MFA for serviceadministrasjon](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Du kan konfigurere mange tilleggspolicyer, for eksempel kreve godkjente klientapper. Hvis du vil ha mer informasjon, kan du se [dokumentasjonen](https://docs.microsoft.com/azure/active-directory/conditional-access/)for betinget tilgang .
