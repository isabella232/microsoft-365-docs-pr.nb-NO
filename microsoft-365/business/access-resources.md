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
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Lær hvordan du får tilgang til lokale ressurser, for eksempel linje med forretningsapper, delte filressurser og skrivere fra en Azure Active Directory-enhet som er koblet til Windows 10-enhet.
ms.openlocfilehash: 653b53d29e84bbdc91273cb78b9b8407c0f6a209
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593237"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Få tilgang til lokale ressurser fra en Azure AD-tilknyttet enhet i Microsoft 365 Business

Alle Windows 10-enheter som er Azure Active Directory-sammenføyd, har tilgang til alle skybaserte ressurser, for eksempel Office 365-appene, og kan beskyttes av Microsoft 365 Business. Du kan også gi tilgang til lokale ressurser, for eksempel bransjeapper (LOB), delte filressurser og skrivere. Hvis du vil gi tilgang, kan du bruke [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) til å synkronisere den lokale Active Directory med Azure Active Directory. 

Hvis du vil ha mer informasjon, kan du se [Innføring i enhetsbehandling i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
Trinnene summeres også i avsnittene nedenfor.

> [!IMPORTANT]
> Denne prosedyren gjelder bare for OAuth og NTLM. Kerberos støttes ikke.
 
## <a name="run-azure-ad-connect"></a>Kjør Azure AD Connect

Fullfør følgende trinn for å gjøre det mulig for organisasjonens Azure AD-tilknyttede enheter å få tilgang til lokale ressurser.
  
1. Hvis du vil synkronisere brukere, grupper og kontakter fra den lokale Active Directory til Azure Active Directory, kjører du veiviseren for katalogsynkronisering og Azure AD Connect som beskrevet i [Konfigurere katalogsynkronisering for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Når katalogsynkroniseringen er fullført, må du kontrollere at organisasjonens Windows 10-enheter er Koblet til Azure AD. Dette trinnet gjøres individuelt på hver Windows 10-enhet. Se [Konfigurere Windows-enheter for Brukere av Microsoft 365 Business](set-up-windows-devices.md) hvis du vil ha mer informasjon. 
    
3. Når Windows 10-enhetene er Koblet til Azure AD, må hver bruker starte enhetene sine på nytt og logge på med legitimasjonen for Microsoft 365 Business. Alle enheter har nå tilgang til lokale ressurser også.
    
Ingen flere trinn er nødvendig for å få tilgang til lokale ressurser for Azure AD-tilknyttede enheter. Denne funksjonaliteten er innebygd i Windows 10. 

Hvis du har planer om å logge inn på AADJ-enheten annet enn passordmetode Som PIN/Bio-metrisk via WHFB-pålogging av legitimasjon og deretter få tilgang til lokale ressurser (delinger, skrivere.. osv.), vennligst følghttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Hvis organisasjonen ikke er klar til å distribuere i Azure AD-sammenføyde enhetskonfigurasjonen som er beskrevet ovenfor, kan du vurdere å konfigurere [konfigurasjonen av Hybrid Azure AD Tilknyttet enhet](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Vurderinger når du blir med i Windows-enheter i Azure AD

Hvis Windows-enheten du azure-AD ble med i, tidligere var domene-sammenføyd eller i en arbeidsgruppe, bør du vurdere følgende begrensninger:
  
- Når en enhet Azure AD blir med, opprettes en ny bruker uten å referere til en eksisterende profil. Profiler må overføres manuelt. En brukerprofil inneholder informasjon som favoritter, lokale filer, nettleserinnstillinger og Innstillinger for Start-menyen. En best tilnærming er å finne et tredjepartsverktøy for å kartlegge eksisterende filer og innstillinger til den nye profilen.

- Hvis enheten bruker gruppepolicyobjekter (GPO), kan det hende at noen gruppepolicyobjekter ikke har en sammenlignbar [configuration serviceleverandør](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) i Intune. Kjør [MMAT-verktøyet](https://www.microsoft.com/download/details.aspx?id=45520) for å finne sammenlignbare CSPer for eksisterende gruppepolicyobjekter.

- Brukere kan ikke godkjenne programmer som er avhengige av Active Directory-godkjenning. Evaluer den eldre appen og vurder å oppdatere til en app som bruker moderne Auth, hvis mulig.

- Active Directory-skrivergjenkjenning fungerer ikke. Du kan angi direkte skriverbaner for alle brukere eller bruke [Hybrid Cloud Print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
