---
title: Overføre fra Microsoft 365 Business til Microsoft 365 E3
f1.keywords:
- NOCSH
ms.author: josephd
author: JoeDavies-MSFT
manager: laurawi
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Finn ut hvordan du flytter bedriften fra Microsoft 365 Business Premium til Microsoft 365 E3.
ms.openlocfilehash: 6a795d96ccae7e054e7e52d4fd60a4e73b3c71dd
ms.sourcegitcommit: 2d59b24b877487f3b84aefdc7b1e200a21009999
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/27/2020
ms.locfileid: "45081869"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Overføre fra Microsoft 365 Business Premium til Microsoft 365 E3

Microsoft 365 Business Premium har alt du trenger for småbedrifter, og kombinerer de best i klassen skybaserte produktivitetsapper med enkel enhetsadministrasjon og sikkerhet som gjør det mulig for de ansatte å gjøre sitt beste arbeid. I noen tilfeller må du imidlertid overføre Microsoft 365 Business Premium-abonnementet til Microsoft 365 E3. 

For eksempel har bedriften din vokst og trenger mer enn 300 lisenser (gratulerer, forresten).

Eller bedriften trenger bedriftsfunksjoner, for eksempel Microsoft 365 Apps for enterprise, Windows 10 Enterprise E3 eller Enterprise Client Access Licenses (CALer).

Oppgradering er enkelt: Du kan starte oppgraderingen [fra administrasjonssenteret](../commerce/subscriptions/upgrade-to-different-plan.md). Alle dataene og konfigurasjonen i det gjeldende abonnementet opprettholdes. Det er ingenting du kan gjøre for å forberede deg på migreringen og ingenting å gjøre etterpå, bortsett fra å dra nytte av de nye funksjonene.

>[!Note]
>Du kan også bruke et Microsoft 365 Business Premium-abonnement for opptil 300 seter og få et Microsoft 365 E3-abonnement for mer enn 300 seter. Office 365 ATP er imidlertid ikke inkludert i Microsoft 365 E3. For fortsatt trusselbeskyttelse bør du legge til flere Office 365 ATP-lisenser slik at alle brukerne i omfanget av Office 365 ATP-politiet er lisensiert.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Forskjeller mellom Microsoft 365 Business Premium og Microsoft 365 Enterprise

Denne tabellen viser forskjellene mellom Microsoft 365 Business Premium og Microsoft 365 E3.

| Funksjon    | Støtte i Microsoft 365 Business Premium    | Støtte i Microsoft 365 E3 | 
|:-------|:-----|:-----|
| **Lokalt**        | | | 
| Windows 10    | Windows 10-bedrift  |     Windows 10 Enterprise E3| 
| Office-apper*    | [Microsoft 365-apper for bedrifter](#office-365-business)    | Microsoft 365-apper for bedrifter | 
| **Skyproduktivitetsapper**        | | | 
| Exchange Online og Outlook    | 50 GB lagringsgrense per postboks og ubegrenset Exchange Online-arkivering    | 100 GB lagringsgrense per postboks og ubegrenset Exchange Online-arkivering | 
| Lag    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
| OneDrive for Business    | 1 TB lagringsgrense per bruker    | Ubegrenset | 
| Yammer, SharePoint Online, Planlegger, Strøm    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
| Kundeansvarlig for Outlook, MileIQ    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Beskyttelse mot trusler**        | | | 
| Angrepsoverflatereduksjonsfunksjoner    | [Se denne listen](#threat-protection) | Bedriftsadministrasjon av maskinvarebasert isolasjon for Microsoft Edge | 
| Office 365 Avansert trusselbeskyttelse (ATP)-plan 1 | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | Ikke inkludert, men kan legges til på | 
| **Identitetsadministrasjon**        | | | 
| Selvbetjent tilbakestilling av passord for hybride Azure Active Directory-kontoer (Azure AD), Azure multifaktorautentisering (MFA), Betinget tilgang, passordskriving for lokale identiteter|     ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
| Oppdagelse av skyapper, Azure AD Connect-tilstand    |     | ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
| Azure AD Office 365-apper enkel pålogging (SSO): 10 apper per bruker (Galleri SaaS-apper som Salesforce)* | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
| Azure AD Premium 1 SSO: ingen grense (lokale apper via Azure AD Application Proxy og ikke-galleriapper som bruker selvbetjente appintegreringsmaler)    |     | ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
| **Administrasjon av enheter og apper**        | | | 
| Microsoft Intune, Windows Autopilot|     ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
|Tilgang til virtuelt skrivebord (VDA)    |  |     ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
|Windows virtuelt skrivebord (WVD)    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png) |     ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
|Aktivering av delt datamaskin (SCA)    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png) |     ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
| Optimaliseringspakke for Microsoft-skrivebordet    | |     ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
| **Beskyttelse av informasjon**        | | | 
| Forebygging av tap av data for Office 365, Azure Information Protection Plan 1    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
| Vindusinformasjonsbeskyttelse for endepunkt DLP    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
| **Klienttilgangslisens (CAL-rettigheter)**    | | |     
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)| |         ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
| **Samsvar**        | | | 
| Ubegrenset e-postarkivering    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
| Samsvarsvurdering/samsvarsbehandling    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
| Ediscovery    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
| På stedet hold og rettssaker hold    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
| Oppbevaringskoder for meldingsarkiver (MRM) og oppbevaringspolicyer    | ![Følger med Microsoft 365 Business Premium](../media/check-mark.png)    | ![Følger med Microsoft 365 E3](../media/check-mark.png) | 
||||

\*Brukere som har fått tilgang til SaaS-apper, kan få SSO-tilgang til opptil 10 apper. Administratorer kan konfigurere SSO og endre brukertilgang til forskjellige SaaS-apper, men SSO-tilgang er bare tillatt for 10 apper per bruker om gangen. Alle Office 365-apper regnes som én enkelt app.

## <a name="migration"></a>Migrasjon

Hvis du vil overføre, kan du samarbeide med partneren din om å flytte Microsoft 365 Business Premium-abonnementet og lisensene til et passende Microsoft 365 E3-abonnement med lisensene.

Avsnittene nedenfor beskriver hvilke endringer du må gjøre, om noen, og hva du kan gjøre etter overføringen.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Konfigurasjon og data for Microsoft 365-abonnement

Du trenger ikke å gjøre endringer i gjeldende abonnement eller data før du overfører, som inkluderer:

- Abonnementskonfigurasjon, for eksempel DNS-domenenavn.
- Bruker- og gruppekontoer og godkjenningsinnstillinger, for eksempel godkjenning med flere faktorer eller policyer for betinget tilgang.
- Produktivitetstjenestekonfigurasjoner og deres data, for eksempel Teams, Exchange Online-postbokser, SharePoint Online-områder, OneDrive for Business-mapper og OneNote-notatblokker.

Brukerne kan nå nyte ubegrenset lagringsplass i Exchange Online-postbokser og OneDrive for Business-mapper.

Du kan begynne å bruke Cloud App Discovery, Azure AD Connect Health og SSO for mer enn 10 apper.

>[!Note]
>Brukere som er overført til Microsoft 365 E3, kan ikke lenger bruke Outlook Customer Manager og MileIQ.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Beskyttelse mot trusler

Windows 10 Business inneholder disse beskyttelsene:

- Integritet håndhevelse av operativsystemet oppstartsprosessen
- Integritetshåndhevelse av sensitive driftskomponenter
- Avansert sårbarhet og nulldagsutnyttelsesreduksjoner
- Omdømmebasert nettverksbeskyttelse for Microsoft Edge, Internet Explorer og Chrome
- Vertsbasert brannmur
- Ransomware begrensninger
- Maskinvarebasert isolasjon for Microsoft Edge
- Programkontroll drevet av Intelligent Security Graph
- Enhetskontroll (USB)
- Nettverksbeskyttelse for nettbaserte trusler
- Regler for forebygging av verter

Windows 10 Enterprise E3 inkluderer også bedriftsadministrasjon av maskinvarebasert isolasjon for Microsoft Edge.

>[!Note]
>Brukere som er overført til Microsoft 365 E3, krever alle en Office 365 ATP-lisens for fortsatt trusselbeskyttelse. Pass på at du kjøper flere Office 365 ATP-lisenser slik at alle brukerne i omfanget av Office 365 ATP-politiet er lisensiert. 
>

### <a name="device-management-with-intune"></a>Enhetsbehandling med Intune

Du trenger ikke å gjøre endringer i den gjeldende Intune-konfigurasjonen før du overfører, som inkluderer registrerte enheter og enhets- og appinnstillinger.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium inkluderer Windows 10 Business, som du kan installere med Windows AutoPilot. Når du overfører til Microsoft 365 E3, inkluderer hver brukerlisens Windows 10 Enterprise E3, som du også kan installere med Windows Autopilot.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365-apper for bedrifter

Microsoft 365 Apps for business-klienten som er installert på enhetene dine, begynner automatisk å bruke funksjonene i Microsoft 365 Apps for enterprise. Etter overføringen kan du nå bruke:

 - Volumaktivering via gruppepolicy
 - App telemetri
 - Oppdatere kontroller
 - Sammenligning og forespørsel om regneark
 - Forretningsintelligens

