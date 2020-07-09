---
title: Synkronisere domenebrukere til Microsoft 365
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: sirkkuw
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Adm_O365
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
description: Synkroniser domenekontrollerte brukere med Microsoft 365 for bedrifter.
ms.openlocfilehash: af9cb7c9b2b639edc2375679a73ab41c4cf6de71
ms.sourcegitcommit: 5b769f74bcc76ac8d38aad815d1728824783cd9f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081907"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Synkronisere domenebrukere til Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. Klargjør for katalogsynkronisering 

Før du synkroniserer brukere og datamaskiner fra det lokale Active Directory-domenet, kan du se [Klargjøre for katalogsynkronisering til Microsoft 365](https://docs.microsoft.com/office365/enterprise/prepare-for-directory-synchronization). Spesielt:

   - Kontroller at det ikke finnes noen duplikater i katalogen for følgende attributter: **e-post**, **proxyAddresses**og **userPrincipalName**. Disse verdiene må være unike, og eventuelle duplikater må fjernes.
   
   - Vi anbefaler at du konfigurerer **attributtet userPrincipalName** (UPN) for hver lokal brukerkonto slik at den samsvarer med den primære e-postadressen som tilsvarer den lisensierte Microsoft 365-brukeren. For eksempel: *mary.shelley@contoso.com* i stedet for *mary@contoso.local*
   
   - Hvis Active Directory-domenet slutter i et ikke-rutbart suffiks som *.local* eller *.lan*, i stedet for et Internett-rutbart suffiks, for eksempel *.com* eller *.org*, justerer du UPN-suffikset for de lokale brukerkontoene først som beskrevet i [Klargjør et ikke-rutbart domene for katalogsynkronisering](https://docs.microsoft.com/office365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

**Kjør IdFix** i trinn fire (4) nedenfor, vil også sørge for at den lokale Active Directory er klar for dir-synkronisering.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Installere og konfigurere Azure AD Connect

Hvis du vil synkronisere brukere, grupper og kontakter fra den lokale Active Directory til Azure Active Directory, installerer du Azure Active Directory Connect og konfigurerer katalogsynkronisering. 

 1. Velg Oppsett i venstre navigasjonsenhet i administrasjonssenteret ved <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> å velge **Oppsett** i venstre navigasjonsenhet.

 2. Under **Pålogging og sikkerhet**velger du **Vis** under Synkroniser brukere **fra organisasjonens katalog**.

 3. Velg **Kom i gang**på siden Synkroniser brukere fra **organisasjonens katalog.**

 4. I det første trinnet kjøre IdFix-verktøyet for å forberede for Katalogsynkronisering.

 5. Følg trinnene i veiviseren for å laste ned Azure AD Connect og bruke den til å synkronisere domenekontrollerte brukere til Microsoft 365.


Se [Konfigurere katalogsynkronisering for Microsoft 365 for](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization) å finne ut mer.

Når du konfigurerer alternativene for Azure AD Connect, anbefaler vi at du aktiverer **synkronisering av passord**, **sømløs enkel pålogging**og funksjonen for **tilbakeskriving** av passord, som også støttes i Microsoft 365 for bedrifter.

> [!NOTE]
> Det er noen flere trinn for passord writeback utover avmerkingsboksen i Azure AD Connect. Hvis du vil ha mer informasjon, kan du se [Slik gjør du det: konfigurere passord writeback](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

Hvis du vil administrere domenet som er sammenkoblet med Windows 10-enheter også, kan du se [Aktivere domenet som er sammenkoblet med Windows 10-enheter, som skal administreres av Microsoft 365 Business Premium,](manage-windows-devices.md) til å konfigurere en hybrid Azure AD Join. 