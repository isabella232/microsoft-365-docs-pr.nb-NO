---
title: Få tilgang til lokale ressurser fra en Azure AD-sammenkoblet enhet i Microsoft 365 Business
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
description: Lær hvordan du får tilgang til lokale ressurser som line of Business-apper, delte filressurser og skrivere fra en Azure Active Directory som er koblet til Windows 10-enheten.
ms.openlocfilehash: ab9049e78617372463b8446dc8f8bc0089d8c117
ms.sourcegitcommit: 91ff1d4339f0f043c2b43997d87d84677c79e279
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2019
ms.locfileid: "36981665"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Få tilgang til lokale ressurser fra en Azure AD-sammenkoblet enhet i Microsoft 365 Business

Alle Windows 10-enheter som er koblet til Azure Active Directory, vil ha tilgang til alle skybaserte ressurser, for eksempel Office 365-appene dine, og kan beskyttes av Microsoft 365 Business. Hvis du også vil gi tilgang til lokale ressurser som line of Business (LOB) apps, delte filressurser og skrivere, må du synkronisere lokale Active Directory med Azure Active Directory ved hjelp av [Azure ad-tilkobling](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). Følgende video beskriver fremgangsmåten for hvordan du konfigurerer dette for det vanligste scenarioet.
 
> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]

Se [innføring i Enhetsbehandling i Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction) for å finne ut mer.
Trinnene oppsummeres også i avsnittene nedenfor.

## <a name="run-azure-ad-connect"></a>Kjør Azure AD-tilkobling

Fullfør fremgangsmåten nedenfor for å aktivere organisasjonens Azure AD ble enheter for å få tilgang til lokale ressurser.
  
1. Hvis du vil synkronisere brukere, grupper og kontakter fra lokal Active Directory til Azure Active Directory, kjører du veiviseren for katalogsynkronisering og koble til Azure AD som beskrevet i [Konfigurere katalogsynkronisering for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Når katalogsynkroniseringen er fullført, må du kontrollere at organisasjonens Windows 10-enheter er Azure AD-tilknyttet. Dette trinnet gjøres individuelt på hver Windows 10-enhet. Se [konfigurere Windows-enheter for Microsoft 365 Business-brukere](set-up-windows-devices.md) for mer informasjon. 
    
3. Når Windows 10-enhetene er Azure AD-medlem, bør hver bruker starte enhetene sine på nytt og logge på med Microsoft 365 Business-legitimasjonen. Alle enheter vil nå også ha tilgang til lokale ressurser.
    
Ingen flere trinn er nødvendig for å få tilgang til lokale ressurser for Azure AD koblet enheter. Dette er innebygd funksjonalitet som er tilgjengelig i Windows 10. 
  
Hvis organisasjonen ikke er klar til å distribuere i Azure AD sammenkoblet enhet-konfigurasjon som er beskrevet ovenfor, kan du vurdere å konfigurere [hybrid Azure ad sammenkoblet enhetskonfigurasjon](manage-windows-devices.md).
  
### <a name="considerations-when-joining-your-windows-devices-to-azure-ad"></a>Betraktninger når du kobler Windows-enheter til Azure AD

Hvis du er Azure AD bli med en Windows-enhet som tidligere har vært tilknyttet domenet eller i en arbeidsgruppe, må du vurdere følgende begrensninger:
  
- Når en enhet Azure AD blir med, oppretter den en ny bruker uten å referere til en eksisterende profil. For å fikse dette må profilene migreres manuelt. En brukerprofil inneholder informasjon som favoritter, lokale filer, nettleserinnstillinger, innstillinger for Start-menyen osv. Den beste tilnærmingen er å finne et tredjepartsverktøy for å tilordne eksisterende filer og innstillinger til den nye profilen

- Hvis enheten brukergruppe policy objekter (GPO), kan noen GPOer ikke ha en sammenlignbar [Konfigurasjonstjeneste leverandør](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) i Intune. Kjør [MMAT-verktøyet](https://www.microsoft.com/download/details.aspx?id=45520) for å finne sammenlignbare CSPer for eksisterende gruppepolicyobjekter.

- Brukere vil ikke kunne godkjennes av programmer som er avhengige av Active Directory-godkjenning. For å håndtere dette evaluere ved hjelp av en eldre app og vurdere å oppdatere til en app som bruker moderne Auth hvis mulig.

- Gjenkjenning av Active Directory-skriveren vil ikke fungere. Hvis du vil løse dette problemet, kan du angi direkte skriver baner for alle brukere eller utnytte [hybrid Cloud print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
