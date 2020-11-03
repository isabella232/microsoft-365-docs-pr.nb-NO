---
title: Synkronisere domene brukere til Microsoft 365
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
description: Synkronisere domene kontrollerte brukere med Microsoft 365 for bedrifter.
ms.openlocfilehash: b40a995a1723808d2fd171c534e9131a891840ba
ms.sourcegitcommit: e56894917d2aae05705c3b9447388d10e2156183
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/03/2020
ms.locfileid: "48841363"
---
# <a name="synchronize-domain-users-to-microsoft-365"></a>Synkronisere domene brukere til Microsoft 365

## <a name="1-prepare-for-directory-synchronization"></a>1. klargjøre for katalog synkronisering 

Før du synkroniserer brukere og data maskiner fra det lokale Active Directory-domenet, kan du se gjennom [klargjør for katalog synkronisering til Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/prepare-for-directory-synchronization). Spesielt:

   - Kontroller at det ikke finnes duplikater i katalogen for følgende attributter: **e-post** , **proxyAddresses** og **userPrincipalName**. Disse verdiene må være unike, og eventuelle duplikater må fjernes.
   
   - Vi anbefaler at du konfigurerer **userPrincipalName** -attributtet (UPN) for hver lokale bruker konto til å samsvare med den primære e-postadressen som tilsvarer den lisensierte Microsoft 365-brukeren. For eksempel: *Mary.Shelley@contoso.com* i stedet for *Mary@contoso. lokal*
   
   - Hvis Active Directory-domenet slutter på et ikke-rutbart suffiks, for eksempel *lokal* eller *LAN* , i stedet for et Internett-omrutende suffiks, som for eksempel *. com* eller *. org* , justerer du UPN-suffikset for de lokale bruker kontoene først som beskrevet i [klargjøre et ikke-rutbart domene for katalog synkronisering](https://docs.microsoft.com/microsoft-365/enterprise/prepare-a-non-routable-domain-for-directory-synchronization). 

**Kjør-IdFix** i trinn fire (4) nedenfor sørger også for at den lokale Active Directory er klar for katalog synkronisering.

## <a name="2-install-and-configure-azure-ad-connect"></a>2. installere og konfigurere Azure AD Connect

Hvis du vil synkronisere brukere, grupper og kontakter fra den lokale Active Directory til Azure Active Directory, må du installere Azure Active Directory Connect og konfigurere katalog synkronisering. 

 1. I [administrasjons senteret](https://go.microsoft.com/fwlink/p/?linkid=2024339)velger du **Oppsett** i det venstre navigasjons feltet.

 2. Under **pålogging og sikkerhet** velger du **Vis**  under **Synkroniser brukere fra organisasjonens katalog**.

 3. Velg **kom i gang** på siden **synkroniserings brukere fra din organisasjons katalog** .

 4. I det første trinnet Kjør IdFix-verktøyet for å klargjøre for katalog synkronisering.

 5. Følg trinnene i vei viseren for å laste ned Azure AD Connect og bruke den til å synkronisere domene kontrollerte brukere til Microsoft 365.


Se [konfigurere katalog synkronisering for Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) for å finne ut mer.

Når du konfigurerer alternativene for Azure AD Connect, anbefaler vi at du aktiverer **passord synkronisering** , **sømløs enkel pålogging** og funksjonen for **passord bakgrunns skriving** , som også støttes i Microsoft 365 for Business.

> [!NOTE]
> Det finnes noen tilleggs trinn for bakgrunns skriving for passord utover avmerkings boksen i Azure AD Connect. Hvis du vil ha mer informasjon, kan du se [How-to: Configure Password bakgrunns skriving](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-writeback). 

Hvis du også vil administrere domene tilknyttede Windows 10-enheter, kan du se [aktivere domene tilknyttede Windows 10-enheter for å administreres av Microsoft 365 Business Premium](manage-windows-devices.md) for å konfigurere en hybrid Azure ad-kobling. 