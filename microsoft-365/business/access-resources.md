---
title: Få tilgang til lokale ressurser fra en Azure AD-sammenkoblet enhet i Microsoft 365 Business
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
description: Lær hvordan du får tilgang til lokale ressurser som bransjeapper, filressurser og skrivere fra en Azure Active Directory-tilknyttet Windows 10-enhet.
ms.openlocfilehash: 9615ecc9469992d3e5a7479f4799c610db11fb41
ms.sourcegitcommit: 2d664a95b9875f0775f0da44aca73b16a816e1c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/01/2020
ms.locfileid: "44471255"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Få tilgang til lokale ressurser fra en Azure AD-tilknyttet enhet i Microsoft 365 Business Premium

Denne artikkelen gjelder for Microsoft 365 Business Premium.

Alle Windows 10-enheter som er Azure Active Directory-koblet til, har tilgang til alle skybaserte ressurser, for eksempel Microsoft 365-appene dine, og kan beskyttes av Microsoft 365 Business Premium. Du kan også gi tilgang til lokale ressurser som lob-apper, filressurser og skrivere. Hvis du vil gi tilgang, kan du bruke [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) til å synkronisere den lokale Active Directory med Azure Active Directory. 

Hvis du vil ha mer informasjon, kan du se [Innføring i enhetsbehandling i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
Trinnene summeres også i avsnittene nedenfor.

> [!IMPORTANT]
> Denne fremgangsmåten gjelder bare for OAuth og NTLM. Kerberos støttes ikke.
 
## <a name="run-azure-ad-connect"></a>Kjør Azure AD Connect

Fullfør følgende trinn for å aktivere organisasjonens Azure AD-sammenkoblede enheter for å få tilgang til lokale ressurser.
  
1. Hvis du vil synkronisere brukere, grupper og kontakter fra lokale Active Directory til Azure Active Directory, kjører du veiviseren for katalogsynkronisering og Azure AD Connect som beskrevet i [Konfigurere katalogsynkronisering for Office 365](https://docs.microsoft.com/office365/enterprise/set-up-directory-synchronization).
    
2. Når katalogsynkroniseringen er fullført, må du kontrollere at organisasjonens Windows 10-enheter er Azure AD som er koblet sammen. Dette trinnet gjøres individuelt på hver Windows 10-enhet. Se [Konfigurere Windows-enheter for Microsoft 365 Business Premium-brukere](set-up-windows-devices.md) hvis du vil ha mer informasjon. 
    
3. Når Windows 10-enhetene er Azure AD slått sammen, må hver bruker starte enhetene på nytt og logge på med Microsoft 365 Business Premium-legitimasjonen. Alle enheter har nå også tilgang til lokale ressurser.
    
Ingen flere trinn er nødvendig for å få tilgang til lokale ressurser for Azure AD sammenføyde enheter. Denne funksjonaliteten er innebygd i Windows 10. 

Hvis du har planer om å logge inn på AADJ-enheten annet enn passordmetoden Som PIN /Bio-metrisk via WHFB-pålogging og deretter få tilgang til lokale ressurser (delinger, skrivere.. osv.), vennligst følghttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Hvis organisasjonen ikke er klar til å distribueres i Azure AD-konfigurasjonen som er sammenkoblet, som er beskrevet ovenfor, kan du vurdere å konfigurere [konfigurasjonen for Hybrid Azure AD-sammenføyde enheter](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Vurderinger når du blir med Windows-enheter til Azure AD

Hvis Windows-enheten du azure-AD ble med i, tidligere var domenet til eller i en arbeidsgruppe, bør du vurdere følgende begrensninger:
  
- Når en enhet Azure AD blir med, oppretter den en ny bruker uten å referere til en eksisterende profil. Profiler må overføres manuelt. En brukerprofil inneholder informasjon som favoritter, lokale filer, nettleserinnstillinger og Innstillinger for Start-menyen. En best tilnærming er å finne et tredjepartsverktøy for å tilordne eksisterende filer og innstillinger til den nye profilen.

- Hvis enheten bruker gruppepolicyobjekter (GPO), kan det hende at noen gruppepolicyobjekter ikke har en sammenlignbar [konfigurasjonstjenesteleverandør](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) i Intune. Kjør [MMAT-verktøyet](https://www.microsoft.com/download/details.aspx?id=45520) for å finne sammenlignbare CSPer for eksisterende gruppepolicyobjekter.

- Brukere kan ikke godkjenne til programmer som er avhengige av Active Directory-godkjenning. Evaluer den eldre appen og vurder å oppdatere til en app som bruker moderne Auth, hvis mulig.

- Active Directory-skrivergjenkjenning fungerer ikke. Du kan angi direkte skriverbaner for alle brukere eller bruke [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
