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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Finn ut hvordan du får tilgang til lokale ressurser, for eksempel bransjeprogrammer, delte filer og skrivere fra en Azure Active Directory som er koblet til Windows 10-enheten.
ms.openlocfilehash: 89ac38f3da9cbdd3ff1a5eb33dc129d2e83521c7
ms.sourcegitcommit: 8c244b38c43dd00c4ef0102f8bed02ab36639a6b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/10/2019
ms.locfileid: "39967167"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business"></a>Få tilgang til lokale ressurser fra en Azure AD-sammenkoblet enhet i Microsoft 365 Business

Alle Windows 10-enheter som Azure Active Directory ble med i, har tilgang til alle skybaserte ressurser, for eksempel Office 365-appene dine, og kan beskyttes av Microsoft 365 Business. Du kan også gi tilgang til lokale ressurser som bransjeprogrammer (LOB), fildelinger og skrivere. Hvis du vil tillate tilgang, bruker du [Azure ad-tilkobling](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect) til å synkronisere den lokale Active Directory med Azure Active Directory. 

Hvis du vil vite mer, kan du se [innføring i Enhetsbehandling i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/device-management-introduction).
Trinnene oppsummeres også i avsnittene nedenfor.

> [!IMPORTANT]
> Denne fremgangsmåten gjelder bare for OAuth og NTLM. Kerberos støttes ikke.
 
## <a name="run-azure-ad-connect"></a>Kjør Azure AD-tilkobling

Fullfør fremgangsmåten nedenfor for å aktivere organisasjonens Azure AD ble enheter for å få tilgang til lokale ressurser.
  
1. Hvis du vil synkronisere brukere, grupper og kontakter fra lokal Active Directory til Azure Active Directory, kjører du veiviseren for katalogsynkronisering og koble til Azure AD som beskrevet i [Konfigurere katalogsynkronisering for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846).
    
2. Når katalogsynkroniseringen er fullført, må du kontrollere at organisasjonens Windows 10-enheter er Azure AD-tilknyttet. Dette trinnet gjøres individuelt på hver Windows 10-enhet. Se [konfigurere Windows-enheter for Microsoft 365 Business-brukere](set-up-windows-devices.md) for mer informasjon. 
    
3. Når Windows 10-enhetene er Azure AD-tilknyttet, må hver bruker starte enhetene sine på nytt og logge på med Microsoft 365-legitimasjonen for bedriften. Alle enheter har nå også tilgang til lokale ressurser.
    
Ingen flere trinn er nødvendig for å få tilgang til lokale ressurser for Azure AD koblet enheter. Denne funksjonaliteten er innebygd i Windows 10. 

Hvis du har planer å logikk å det AADJ apparat annet enn passord metoden like knappenål/bio-metrisk via WHFB legitimasjonen logikk og så adgang opp på-premiss ressursene (aksjer, Printer.. osv.), må du følgehttps://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base
  
Hvis organisasjonen ikke er klar til å distribuere i Azure AD sammenkoblet enhetskonfigurasjonen som er beskrevet ovenfor, kan du vurdere å konfigurere [hybrid Azure ad sammenkoblet enhetskonfigurasjon](manage-windows-devices.md).
  
### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Betraktninger når du blir med Windows-enheter til Azure AD

Hvis Windows-enheten du Azure-AD ble med i, tidligere var tilknyttet et domene eller i en arbeidsgruppe, bør du vurdere følgende begrensninger:
  
- Når en enhet Azure AD blir med, oppretter den en ny bruker uten å referere til en eksisterende profil. Profiler må migreres manuelt. En brukerprofil inneholder informasjon som favoritter, lokale filer, nettleserinnstillinger og innstillinger for Start-menyen. En beste fremgangsmåte er å finne et tredjepartsverktøy for å tilordne eksisterende filer og innstillinger til den nye profilen.

- Hvis enheten brukergruppe policy objekter (GPO), kan noen GPOer ikke ha en sammenlignbar [Konfigurasjonstjeneste leverandør](https://docs.microsoft.com/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) (CSP) i Intune. Kjør [MMAT-verktøyet](https://www.microsoft.com/download/details.aspx?id=45520) for å finne sammenlignbare CSPer for eksisterende gruppepolicyobjekter.

- Brukere vil ikke kunne godkjenne programmer som er avhengige av Active Directory-godkjenning. Evaluer arven app og vurdere å oppdatere til en app som bruker moderne Auth, hvis mulig.

- Discovery for Active Directory-skriveren fungerer ikke. Du kan angi direkte skriver baner for alle brukere eller bruke [hybrid Cloud print](https://docs.microsoft.com/windows-server/administration/hybrid-cloud-print/hybrid-cloud-print-deploy).
