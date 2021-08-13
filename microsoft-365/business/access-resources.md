---
title: Få tilgang til lokale ressurser fra en Azure AD-sammenføyd enhet i Microsoft 365 Business
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
- AdminTemplateSet
search.appverid:
- BCS160
- MET150
ms.assetid: b0f4d010-9fd1-44d0-9d20-fabad2cdbab5
description: Lær hvordan du får tilgang til lokale ressurser, for eksempel bransjeapper, delte filressurser og skrivere fra en Azure Active Directory koblet til Windows 10 enhet.
ms.openlocfilehash: 49d7150adb8bcb0dd611e7dce10ee92d3de1755dbe8662e454c9afcca2055e69
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53809474"
---
# <a name="access-on-premises-resources-from-an-azure-ad-joined-device-in-microsoft-365-business-premium"></a>Få tilgang til lokale ressurser fra en Azure AD-sammenføyd enhet i Microsoft 365 Business Premium

Denne artikkelen gjelder for Microsoft 365 Business Premium.

Alle Windows 10 som er Azure Active Directory har tilgang til alle skybaserte ressurser, for eksempel Microsoft 365-appene, og kan beskyttes av Microsoft 365 Business Premium. Du kan også gi tilgang til lokale ressurser, for eksempel bransjeapper (LOB), delte filressurser og skrivere. Hvis du vil tillate tilgang, bruker [du Azure AD Koble til](/azure/active-directory/connect/active-directory-aadconnect) til å synkronisere den lokale Active Directory med Azure Active Directory.

Hvis du vil ha mer informasjon, kan du se Innføring i [enhetsbehandling i Azure Active Directory](/azure/active-directory/device-management-introduction).
Trinnene oppsummeres også i avsnittene nedenfor.

## <a name="run-azure-ad-connect"></a>Kjør Azure AD-Koble til

Fullfør følgende trinn for å aktivere organisasjonens Azure AD-sammenføyde enheter for å få tilgang til lokale ressurser.

1. Hvis du vil synkronisere brukere, grupper og kontakter fra lokale Active Directory til Azure Active Directory, kjører du veiviseren for katalogsynkronisering og Azure AD Koble til som beskrevet i Konfigurere katalogsynkronisering [for Office 365](../enterprise/set-up-directory-synchronization.md).

2. Når katalogsynkroniseringen er fullført, må du kontrollere at organisasjonens Windows 10 er Azure AD sammenføyd. Dette trinnet gjøres enkeltvis på hver Windows 10 enhet. Se [Konfigurere Windows for Microsoft 365 Business Premium for mer](set-up-windows-devices.md) informasjon.

3. Når enhetene Windows 10 Azure AD, må hver bruker starte enhetene på nytt og logge på med Microsoft 365 Business Premium legitimasjon. Alle enheter har nå også tilgang til lokale ressurser.

Ingen ekstra trinn er nødvendig for å få tilgang til lokale ressurser for Azure AD-sammenføyde enheter. Denne funksjonaliteten er innebygd i Windows 10.

Hvis du har planer om å logge på AADJ-enheten annet enn passordmetode, for eksempel PIN/Bio-metrisk via WHFB-pålogging og deretter få tilgang til lokale ressurser (aksjer, skrivere og så videre), følger du [denne artikkelen](/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

Hvis organisasjonen ikke er klar til å distribuere i konfigurasjonen av azure AD-sammenføyde enheter som er beskrevet ovenfor, bør du vurdere å konfigurere konfigurasjon av [hybrid Azure AD-sammenføyd enhet.](manage-windows-devices.md)

### <a name="considerations-when-you-join-windows-devices-to-azure-ad"></a>Hensyn når du blir med Windows til Azure AD

Hvis enheten Windows Azure-AD ble med i tidligere domene, ble med i eller i en arbeidsgruppe, bør du vurdere følgende begrensninger:

- Når en enhet Azure AD blir med, opprettes en ny bruker uten å referere til en eksisterende profil. Profiler må overføres manuelt. En brukerprofil inneholder informasjon som favoritter, lokale filer, nettleserinnstillinger og Start-meny innstillinger. Den beste fremgangsmåten er å finne et tredjepartsverktøy for å tilordne eksisterende filer og innstillinger til den nye profilen.

- Hvis enheten bruker gruppepolicyobjekter (GPO), kan det hende [](/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers) at enkelte gruppepolicyobjekter ikke har en sammenlignbar konfigurasjonstjenesteleverandør (CSP) i Intune. Kjør [MMAT-verktøyet for](https://www.microsoft.com/download/details.aspx?id=45520) å finne sammenlignbare CSP-er for eksisterende gruppepolicyobjekter.

- Brukere kan kanskje ikke godkjenne til programmer som er avhengige av Active Directory-godkjenning. Evaluer den eldre appen, og vurder om mulig å oppdatere til en app som bruker moderne Auth.

- Active Directory-skriveroppdagelse fungerer ikke. Du kan angi direkte skriverbaner for alle brukere eller bruke [Universal Print](/universal-print/).

### <a name="related-articles"></a>Relaterte artikler

[Forutsetninger for Azure AD-Koble til](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)
