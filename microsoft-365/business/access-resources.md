---
title: Få tilgang til lokale ressurser fra en Azure AD-tilknyttet enhet i Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: M365-subscription-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Lær hvordan du får tilgang til lokale ressurser, for eksempel bransje programmer, delte fil ressurser og skrivere fra en Azure Active Directory-enhet som er koblet til Windows 10.
ms.openlocfilehash: 22edf0c23d6318e1f70bcb21b2cd697ea0a75da4
ms.sourcegitcommit: 849b365bd3eaa9f3c3a9ef9f5973ef81af9156fa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/16/2020
ms.locfileid: "49688237"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Få tilgang til lokale ressurser fra en Azure AD-tilknyttet enhet i Microsoft 365 Business Premium

Denne artikkelen gjelder for Microsoft 365 Business Premium.

Alle Windows 10-enheter som er koblet til Azure Active Directory, har tilgang til alle Sky BAS ert ressurser, for eksempel Microsoft 365-appene, og kan beskyttes av Microsoft 365 Business Premium. Du kan også tillate tilgang til lokale ressurser, for eksempel bransje programmer (LOB), delte fil ressurser og skrivere. Hvis du vil tillate tilgang, bruker du [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) til å synkronisere den lokale Active Directory-katalogen med Azure Active Directory. 

Hvis du vil ha mer informasjon, kan du se [innføring i enhets behandling i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
Fremgangs måten er også oppsummert i de følgende avsnittene.
 
## <a name="run-azure-ad-connect"></a>Kjøre Azure AD Connect

Følg Fremgangs måten nedenfor for å aktivere organisasjonens Azure AD-tilknyttede enheter for å få tilgang til lokale ressurser.
  
1. Hvis du vil synkronisere brukere, grupper og kontakter fra lokal Active Directory til Azure Active Directory, kan du kjøre vei viseren for katalog synkronisering og Azure AD Connect som beskrevet i [konfigurere katalog synkronisering for Office 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization).
    
2. Når katalog synkroniseringen er fullført, må du kontrollere at organisasjonens Windows 10-enheter er Azure-AD-koblet. Dette trinnet gjøres individuelt på hver Windows 10-enhet. Se [konfigurere Windows-enheter for Microsoft 365 Business Premium-brukere](set-up-windows-devices.md) hvis du vil ha mer informasjon. 
    
3. Når Windows 10-enhetene er Azure-AD-koblet, må hver bruker starte enhetene sine og logge på med Microsoft 365 Business Premium-legitimasjonen. Alle enheter har nå tilgang til lokale ressurser også.
    
Ingen flere trinn kreves for å få tilgang til lokale ressurser for Azure AD-tilknyttede enheter. Denne funksjonen er innebygd i Windows 10. 

Hvis du har planer om å logge på en annen AADJ-enhet enn passord metode, for eksempel PIN/bio-metrikk via WHFB legitimasjons pålogging og deretter få tilgang til lokale ressurser (aksjer, skrivere.. så videre), kom i gang https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Hvis organisasjonen ikke er klar til å distribuere i den Azure-AD-tilknyttede enhets konfigurasjonen som er beskrevet ovenfor, kan du vurdere å konfigurere [hybrid Azure ad-tilkoblet enhets konfigurasjon](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Betraktninger når du blir med i Windows-enheter til Azure AD

Hvis Windows-enheten du har koblet til Azure-AD, tidligere ble domene tilknyttet eller i en arbeids gruppe, bør du vurdere følgende begrensninger:
  
- Når en enhet Azure AD kobles sammen, oppretter den en ny bruker uten å referere til en eksisterende profil. Profiler må overføres manuelt. En bruker profil inneholder informasjon som favoritter, lokale filer, nett leser innstillinger og innstillinger for Start-menyen. En beste Fremgangs måte er å finne et tredje parts verktøy for å tilordne eksisterende filer og innstillinger til den nye profilen.

- Hvis enheten bruker gruppe policy objekter (GPO), kan det hende at enkelte GPOer ikke har en leverandør av tilsvarende [konfigurasjons tjeneste](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) i Intune. Kjør [MMAT-verktøyet](https://www.microsoft.com/download/details.aspx?id=45520) for å finne sammenlignbare CSPer for eksisterende GPOer.

- Brukere kan ikke godkjenne seg for programmer som er avhengige av Active Directory-godkjenning. Evaluer den eldre appen, og Vurder å oppdatere til en app som bruker moderne godkjenning, hvis mulig.

- Søk i Active Directory-skriveren vil ikke fungere. Du kan gi direkte filbaner til alle brukere eller bruke [universell utskrift](https://aka.ms/UPDocs).
