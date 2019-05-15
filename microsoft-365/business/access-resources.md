---
title: Access lokale ressurser fra en Azure AD-koblet enheten i Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Lær hvordan du får tilgang til lokale ressurser som linjen Business apps, delte filer og skrivere fra en Active Directory Azure sammen Windows 10 enhet.
ms.openlocfilehash: fa3cf640e799feb81ff08c5b7b81d57f707e0152
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/15/2019
ms.locfileid: "34072034"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Access lokale ressurser fra en Azure AD-koblet enheten i Microsoft 365 Business

Alle Windows 10 enheter som er Azure Active Directory sammen, har tilgang til alle sky-baserte ressurser som Office 365-apps og kan være beskyttet av Microsoft 365 Business. Hvis du også tillate tilgang til lokale ressurser som linje av Business (LOB) apps, delte filer og skrivere, må du synkronisere lokale Active Directory med Azure Active Directory ved hjelp av [Azure AD-tilkobling](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). Se [Innføring i Enhetsbehandling i Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) for å lære mer. 
  
## <a name="run-azure-ad-connect"></a>Kjør Azure AD koble

Bruk følgende fremgangsmåte for å aktivere organisasjonens Azure AD koblet enheter til å få tilgang til lokale ressurser.
  
1. Kjør veiviseren for Directory-synkronisering for å synkronisere brukere, grupper og kontakter fra lokal Active Directory til Azure Active Directory, og koble til Azure AD som beskrevet i [konfigurere katalogsynkronisering for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Når directory-synkronisering er fullført, kontrollerer du at organisasjonens Windows 10 enheter er Azure AD sammen. Dette trinnet utføres individuelt på hver Windows-10-enhet. Se [konfigurere Windows-enheter for forretningsbrukere som Microsoft 365](set-up-windows-devices.md) for detaljer. 
    
3. Når Windows 10 enhetene er koblet Azure AD, bør hver bruker omstart sine enheter og pålogging med legitimasjonen Microsoft 365 Business. Alle enheter har nå tilgang til lokale ressurser også.
    
Det kreves ingen ekstra trinn for å få tilgang til lokale ressurser for Azure AD koblet enheter. Dette er innebygd funksjonalitet som er tilgjengelige i Windows-10. 
  
Hvis organisasjonen ikke er klar til å distribuere i Azure AD sammen enhetskonfigurasjonen som er beskrevet ovenfor, bør du vurdere å installere [Hybrid Azure AD JOIN enhetskonfigurasjon](manage-windows-devices.md).
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a>Sikkerhetshensyn ved å sammenføye enhetene Windows Azure AD

Hvis du er Azure AD å bli med i en Windows-enhet som tidligere er tilknyttet et domene eller i en arbeidsgruppe, må du ta hensyn til følgende begrensninger:
  
- Når en enhet Azure AD sammenføyninger, opprettes det en ny bruker uten refererer til en eksisterende profil. Hvis du vil løse dette problemet, må profiler overføres manuelt. En brukerprofil inneholder informasjon, for eksempel Favoritter, lokale filer, innstillinger, innstillinger for Start-menyen, osv. Beste fremgangsmåten er å finne et tredjepartsverktøy til å tilordne eksisterende filer og innstillinger til den nye profilen

- Hvis enheten bruker gruppe gruppepolicyobjekter (GPO), kanskje noen gruppepolicyobjekter har ikke en sammenlignbar [Configuration Service Provider](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) i Intune. Kjør [MMAT-verktøyet](https://www.microsoft.com/download/details.aspx?id=45520) for å finne tilsvarende CSP for eksisterende gruppepolicyobjekter.

- Brukere vil ikke kunne godkjenne til programmer som avhenger av Active Directory-autentisering. Dette vurdere å bruke et eldre program og vurdere å oppdatere til et program som bruker moderne godkjenning hvis det er mulig å forholde seg til.

- Active Directory-gjenkjenning for skriveren vil ikke fungere. Hvis du vil løse dette problemet, gir direkte skriverbaner for alle brukere eller dra nytte av [Hybrid sky utskrift](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
