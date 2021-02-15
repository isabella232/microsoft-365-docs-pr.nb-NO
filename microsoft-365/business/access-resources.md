---
title: Få tilgang til lokale ressurser fra en enhet med Azure AD-tilgang i Microsoft 365 Business
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
description: Lær hvordan du får tilgang til lokale ressurser som bransjeapper, delte filressurser og skrivere fra en Windows 10-enhet som er koblet til Azure Active Directory.
ms.openlocfilehash: fc02fd30f41f25f52e653e750a6bdfd1bd7f800e
ms.sourcegitcommit: a62ac3c01ba700a51b78a647e2301f27ac437c5a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2021
ms.locfileid: "50233844"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Få tilgang til lokale ressurser fra en enhet med Azure AD-tilgang i Microsoft 365 Business Premium

Denne artikkelen gjelder for Microsoft 365 Business Premium.

Alle Windows 10-enheter som er med i Azure Active Directory, har tilgang til alle skybaserte ressurser, for eksempel Microsoft 365-apper, og kan beskyttes av Microsoft 365 Business Premium. Du kan også gi tilgang til lokale ressurser som bransjeapper (LOB), delte filressurser og skrivere. Hvis du vil tillate tilgang, [kan du bruke Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) til å synkronisere lokal Active Directory med Azure Active Directory. 

Hvis du vil ha mer informasjon, kan du [se Innføring i enhetsbehandling i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/device-management-introduction)
Trinnene oppsummeres også i avsnittene nedenfor.
 
## <a name="run-azure-ad-connect"></a>Kjør Azure AD Connect

Fullfør følgende trinn for å aktivere organisasjonens Azure AD-koblede enheter for å få tilgang til lokale ressurser.
  
1. Hvis du vil synkronisere brukere, grupper og kontakter fra lokal Active Directory til Azure Active Directory, kan du kjøre veiviseren for katalogsynkronisering og Azure AD Connect som beskrevet i Konfigurere katalogsynkronisering [for Office 365.](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization)
    
2. Når katalogsynkroniseringen er fullført, må du kontrollere at organisasjonens Windows 10-enheter er sammenføyd med Azure AD. Dette trinnet gjøres enkeltvis på hver Windows 10-enhet. Se [Konfigurere Windows-enheter for brukere av Microsoft 365 Business Premium](set-up-windows-devices.md) for mer informasjon. 
    
3. Når Windows 10-enhetene er med i Azure AD, må hver bruker starte enhetene sine på nytt og logge på med Microsoft 365 Business Premium-legitimasjonen. Alle enheter har nå også tilgang til lokale ressurser.
    
Ingen flere trinn er nødvendig for å få tilgang til lokale ressurser for Azure AD-sammenføyde enheter. Denne funksjonaliteten er innebygd i Windows 10. 

Hvis du har planer om å logge på AADJ-enheten annet enn passordmetoden, som for eksempel PIN/metrisk bio-metrisk via pålogging for WHFB-legitimasjon og deretter få tilgang til lokale ressurser (deler, skrivere). osv.), følg https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Hvis organisasjonen ikke er klar til å distribuere i den azure AD-sammenføyde enhetskonfigurasjonen som er beskrevet ovenfor, kan du vurdere å konfigurere konfigurasjon for enheten [Hybrid Azure AD Joined.](manage-windows-devices.md)
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Hensyn som må tas når du slår sammen Windows-enheter med Azure AD

Hvis Windows-enheten du ble med i Azure-AD sammen med, tidligere var sammenføyd med domenet eller i en arbeidsgruppe, kan du vurdere følgende begrensninger:
  
- Når en enhet med Azure AD blir med, opprettes en ny bruker uten å referere til en eksisterende profil. Profiler må overføres manuelt. En brukerprofil inneholder informasjon som favoritter, lokale filer, nettleserinnstillinger og Start-menyinnstillinger. Den beste fremgangsmåten er å finne et tredjepartsverktøy til å tilordne eksisterende filer og innstillinger til den nye profilen.

- Hvis enheten bruker gruppepolicyobjekter, kan det hende at enkelte [](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) gruppepolicyobjekter ikke har en tilsvarende konfigurasjonstjenesteleverandør (CSP) i Intune. Kjør [MMAT-verktøyet for](https://www.microsoft.com/download/details.aspx?id=45520) å finne sammenlignbare CSP-er for eksisterende GPO-er.

- Det kan hende at brukere ikke kan godkjenne til programmer som er avhengige av Active Directory-godkjenning. Evaluer den eldre appen, og vurder om mulig å oppdatere til en app som bruker moderne godkjapp.

- Søk etter Active Directory-skrivere vil ikke fungere. Du kan angi baner for direkte skriver for alle brukere, eller bruke [Universal Print.](https://aka.ms/UPDocs)
