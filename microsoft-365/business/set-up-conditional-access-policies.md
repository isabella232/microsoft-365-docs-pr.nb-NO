---
title: Definer policyer for betinget tilgang for Microsoft 365 kampanjer
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
search.appverid:
- BCS160
- MET150
- MOE150
description: Lær hvordan du setter opp betinget tilgang policyer for Microsoft 365 kampanjer.
ms.openlocfilehash: 7d8e1f16019d151478aae57b1593b0e0758e5b19
ms.sourcegitcommit: 7e46db0b35c188ee6a7b40ab3eb2d76ff6c101c5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/19/2019
ms.locfileid: "35086363"
---
# <a name="set-up-conditional-access-policies"></a>Definer policyer for betinget tilgang

[Betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) policyer legger substancial ekstra sikkerhet. Microsoft tilbyr et sett med planlagte betinget tilgang policyer som er anbefalt for alle kunder. Policyer for opprinnelig plan er et sett med forhåndsdefinerte policyer som beskytter organisasjoner mot mange vanlige angrep. Disse vanlige angrep kan inkludere passord Sprederen, replay og phishing.

Disse policyene krever at administratorer og brukere til å angi en annen form for godkjenning (kalt multifaktorautentisering eller MFA) når visse betingelser er oppfylt. For eksempel hvis en bruker er logger på fra et annet land, pålogging kan vurderes som risikabelt, og brukeren må angi en mer form for godkjenning. 

For øyeblikket omfatter planlagt policyene følgende:
- **Krever MFA for administratorer** , krever multifaktorautentisering for de mest privilegerte administrator-rollene, inkludert global administrator.
- **Sluttbrukeren beskyttelse** , krever multifaktorautentisering for brukere bare når en pålogging er risikabelt. 
- **Eldre blokk-godkjenning** – eldre klientprogrammer og noen nye apps ikke bruke godkjenningsprotokoller som er nyere, sikrere. Disse eldre programmer kan hoppe over policyer for betinget tilgang og få uautorisert tilgang til ditt miljø. Denne policyen blokkerer tilgang fra klienter som ikke støtter betinget tilgang. 
- **Krever MFA for servicestyring** – krever multifaktorautentisering for tilgang til verktøy for systemadministrasjon, inkludert Azure portal (hvor du konfigurere policyer for opprinnelig plan). 

Microsoft anbefaler at du aktiverer alle disse policyene for opprinnelig plan. Når disse policyene er aktivert, administratorer og brukere vil bli bedt om å registrere deg for Azure Multii-faktors autentifiseringsprosess.

Hvis du vil ha mer informasjon om disse policyene, kan du se [Hva er planlagt policyer](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)?


## <a name="set-up-baseline-policies"></a>Definer policyer for opprinnelig plan

1. Gå til [Azure portal](https://portal.azure.com), og naviger deretter til **Azure Active Directory** \> **Betinget tilgang**.
    
    Policyer for opprinnelig plan er oppført på siden. <br/> <br/>
    ![Side som viser en liste over planlagte policyer for betinget tilgang.](media/baslinepolicies.png)
1. Se følgende spesifikke instruksjoner for hver policy:

  - [Krev MFA for administratorer](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-administrators)
- [Reequire MFA for brukere](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-end-users)  
 - [Eldre blokk-godkjenning](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth)
  - [Krev MFA for servicestyring](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-azure)

Du kan definere mange flere policyer, som for eksempel at godkjente klientprogrammer. Se [Dokumentasjonen for betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/) for mer informasjon.