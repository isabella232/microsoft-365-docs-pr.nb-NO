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
ms.openlocfilehash: 1c939dec7229f02991b15f08c48f184efecaddb0
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913258"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Synkronisere domenebrukere til Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. Klargjøre for katalogsynkronisering 

Før du synkroniserer brukere og datamaskiner fra det lokale Active Directory-domenet, kan du se [Klargjøre for katalogsynkronisering til Microsoft 365.](../enterprise/prepare-for-directory-synchronization.md) Spesielt:

   - Kontroller at det ikke finnes duplikater i katalogen for følgende attributter: **e-post,** **proxyAddresses** og **userPrincipalName**. Disse verdiene må være unike, og eventuelle duplikater må fjernes.
   
   - Vi anbefaler at du konfigurerer **userPrincipalName-attributtet** (UPN) for hver lokale brukerkonto slik at den samsvarer med den primære e-postadressen som tilsvarer den lisensierte Microsoft 365-brukeren. For eksempel: *mary.shelley@contoso.com* i stedet *mary@contoso.local*
   
   - Hvis Active [Directory-domenet](../enterprise/prepare-a-non-routable-domain-for-directory-synchronization.md)slutter på et ikke-rutbart suffiks som *.local* eller *.lan*, i stedet for et suffiks som kan rutteres på Internett, for eksempel *.com* eller *.org,* justerer du UPN-suffikset for de lokale brukerkontoene først som beskrevet i Klargjøre et domene som ikke kan rutteres for katalogsynkronisering . 

Kjør **IdFix i** trinn fire (4) nedenfor, vil også sørge for at den lokale Active Directory er klar for katalogsynkronisering.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. Installere og konfigurere Azure AD Connect

Hvis du vil synkronisere brukere, grupper og kontakter fra den lokale Active Directory til Azure Active Directory, installerer du Azure Active Directory Connect og konfigurerer katalogsynkronisering. 

 1. Velg Oppsett [i](https://go.microsoft.com/fwlink/p/?linkid=2024339)  det venstre navigasjonsfeltet i administrasjonssenteret.

 2. Velg **Vis under** Synkroniser brukere fra **organisasjonens katalog** under Pålogging og sikkerhet . 

 3. Velg Kom i gang på siden **Synkroniser** brukere fra **organisasjonens** katalog.

 4. I det første trinnet kjører du IdFix-verktøyet for å klargjøre for katalogsynkronisering.

 5. Følg trinnene i veiviseren for å laste ned Azure AD Connect og bruke det til å synkronisere domenekontrollerte brukere til Microsoft 365.


Se [Konfigurere katalogsynkronisering for Microsoft 365 for](../enterprise/set-up-directory-synchronization.md) å finne ut mer.

Når du konfigurerer alternativene for Azure AD Connect, anbefaler vi at du  aktiverer Passordsynkronisering, Sømløs enkel pålogging og funksjonen for tilbakeskriving av passord, som også støttes i Microsoft 365 for bedrifter.

> [!NOTE]
> Det finnes noen flere trinn for tilbakeskriving av passord utover avmerkingsboksen i Azure AD Connect. Hvis du vil ha mer informasjon, kan du [se Slik konfigurerer du tilbakeskriving av passord](/azure/active-directory/authentication/howto-sspr-writeback). 

Hvis du også vil administrere domene-sammenføyde Windows 10-enheter, kan du se Aktivere domenekretserte [Windows 10-enheter](manage-windows-devices.md) som skal administreres av Microsoft 365 Business Premium for å konfigurere en hybrid Azure AD Join.