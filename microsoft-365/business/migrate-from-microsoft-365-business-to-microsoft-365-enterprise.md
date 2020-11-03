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
description: Lær hvordan du flytter virksomheten fra Microsoft 365 Business Premium til Microsoft 365 E3.
ms.openlocfilehash: 874da0d35759c8af4c3ee2ca4a1bdfa90a91627c
ms.sourcegitcommit: 815229e39a0f905d9f06717f00dc82e2a028fa7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/03/2020
ms.locfileid: "48842204"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Overføre fra Microsoft 365 Business Premium til Microsoft 365 E3

Microsoft 365 Business Premium har alt du trenger for din lille bedrift, og kombinerer de beste Sky BAS ert produktivitets appene med enkel enhets behandling og sikkerhet som gjør at de ansatte kan gjøre sitt beste arbeid. I noen tilfeller må du imidlertid kanskje overføre Microsoft 365 Business Premium-abonnementet til Microsoft 365 E3. 

Virksomheten din har for eksempel vokst og trenger mer enn 300 lisenser (Gratulerer, av veien).

Virksomheten din trenger enterprise-funksjoner, for eksempel Microsoft 365-apper for Enterprise, Windows 10 Enterprise E3 eller Enterprise Client Access licenses (CALs).

Det er enkelt å oppgradere: du kan starte oppgraderingen [fra administrasjons senteret](../commerce/subscriptions/upgrade-to-different-plan.md). Alle data og konfigurasjon i det gjeldende abonnementet beholdes. Det er ingenting for deg å gjøre deg klar for overføring og ingenting å gjøre etterpå, bortsett fra å dra nytte av de nye funksjonene.

>[!Note]
>Du kan også bruke et Microsoft 365 Business Premium-abonnement på opptil 300 plasser og få et Microsoft 365 E3-abonnement for mer enn 300 seter. Microsoft Defender for Office 365 er imidlertid ikke inkludert i Microsoft 365 E3. For videre trussel beskyttelse bør du legge til flere Defender for Office 365-lisenser slik at alle brukerne i omfanget av dine Defender for Office-365-policyer er lisensiert.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Forskjeller mellom Microsoft 365 Business Premium og Microsoft 365 Enterprise

Denne tabellen viser forskjellene mellom Microsoft 365 Business Premium og Microsoft 365 E3.

| Funksjon    | Støtte i Microsoft 365 Business Premium    | Støtte i Microsoft 365 E3 | 
|:-------|:-----|:-----|
| **Lokalt**        | | | 
| Windows 10    | Windows 10 Business  |     Enterprise E3 for Windows 10| 
| Office-apper *    | [Microsoft 365-apper for bedrifter](#office-365-business)    | Microsoft 365-apper for enterprise | 
| **Produktivitets programmer for skyen**        | | | 
| Exchange Online og Outlook    | lagrings grensen på 50 GB per post boks og ubegrenset Exchange Online-arkivering    | lagrings grensen på 100 GB per post boks og ubegrenset Exchange Online-arkivering | 
| Team    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| OneDrive for Business    | 1 TB lagrings grense per bruker    | Uendelige | 
| Yammer, SharePoint Online, Planner, dataflyt    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Outlook Customer Manager, MileIQ    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Trussel beskyttelse**        | | | 
| Funksjoner for reduksjon av angreps overflate    | [Se denne listen](#threat-protection) | Bedrifts styring av maskin vare BAS ert isolasjon for Microsoft Edge | 
| Defender for Office 365 plan 1 | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | Ikke inkludert, men kan legges til på | 
| **Identitets behandling**        | | | 
| Selv betjent tilbakestilling av passord for hybride Azure Active Directory-kontoer (Azure AD), Azure multi-Factor Authentication (MFA), betinget tilgang, passord bakgrunn for lokale identiteter|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Sky BAS ert app-oppdagelse, Azure AD Connect-tilstand    |     | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Azure AD Office 365-apper enkelt Sign-On (SSO): 10 apper per bruker (Galleri SaaS apper som Salesforce) * | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Azure AD Premium 1 SSO: ingen grense (lokale apper gjennom Azure AD Application proxy og ikke-Galleri programmer ved hjelp av Self-Service app Integration-maler)    |     | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| **Enhets-og app-behandling**        | | | 
| Microsoft Intune, Windows autopilot|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
|Tilgang til virtuelt skrive bord (VDA)    |  |     ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
|Windows virtuelt skrive bord (WVD)    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png) |     ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
|Aktivering av delt data maskin (SCA)    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png) |     ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Microsoft Desktop optimize-pakke    | |     ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| **Informasjons beskyttelse**        | | | 
| Office 365 datatap, Azure Information Protection Plan 1    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Beskyttelse av vindus informasjon for Endpoint DLP    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| **Klient adgangs lisens (CAL-rettigheter)**    | | |     
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)| |         ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| **Skrift**        | | | 
| Ubegrenset e-postarkivering    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Samsvars ansvarlig    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| eDiscovery    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Lokal sperring og søksmål-sperring    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Koder for post behandling for meldinger (MRM) og oppbevarings policyer    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
||||

\* Brukere som har fått tilordnet tilgang til SaaS-apper, kan få SSO-tilgang til opptil 10 apper. Administratorer kan konfigurere SSO og endre bruker tilgang til forskjellige SaaS-apper, men SSO-tilgang er bare tillatt for 10 apper per bruker om gangen. Alle Office 365-apper telles som én app.

## <a name="migration"></a>Medlemsserver

Hvis du vil overføre, arbeider du med partneren din for å flytte Microsoft 365 Business Premium-abonnementet og lisenser til et egnet Microsoft 365 E3-abonnement med lisensene.

Avsnittene nedenfor beskriver hvilke endringer du må gjøre, og hva du kan gjøre etter overføringen.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Konfigurasjon og data for Microsoft 365-abonnement

Du trenger ikke å gjøre endringer i gjeldende abonnement eller data før du overfører, som omfatter følgende:

- Abonnements konfigurasjon, for eksempel DNS-domenenavn.
- Bruker-og gruppe kontoer og godkjennings innstillinger, for eksempel godkjenning for flere faktorer eller policyer for betinget tilgang.
- Produktivitets tjeneste konfigurasjoner og tilhørende data, for eksempel team, Exchange Online-postbokser, SharePoint Online-nettsteder, OneDrive for Business-mapper og OneNote-notatblokker.

Brukerne kan nå nyte ubegrenset lagrings plass i Exchange Online-post boksene og OneDrive for Business-mappene.

Du kan begynne å bruke program søk i skyen, Azure AD Connect-tilstand og SSO for mer enn 10 apper.

>[!Note]
>Brukere som er overført til Microsoft 365 E3, kan ikke lenger bruke Outlook Customer Manager og MileIQ.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Trussel beskyttelse

Windows 10 Business inneholder disse beskyttelsene:

- Integritets håndhevelse av oppstart prosessen for operativ systemet
- Integritets håndhevelse av sensitive operativ komponenter
- Avansert sikkerhets problem og reduksjon av null dager
- Rykte-basert nettverks beskyttelse for Microsoft Edge, Internet Explorer og Chrome
- Verts BAS ert brann mur
- Reduksjon av løse penge virus
- Maskin vare BAS ert isolasjon for Microsoft Edge
- Program kontroll som leveres av intelligent Security Graph
- Enhets kontroll (USB)
- Nettverks beskyttelse for nett BAS ert trusler
- Regler for å hindre verts angrep

Windows 10 Enterprise E3 inkluderer også organisasjons styring av maskin vare BAS ert isolasjon for Microsoft Edge.

>[!Note]
>Brukere som er overført til Microsoft 365 E3, krever at hver Microsoft Defender for Office 365-lisens for videre beskyttelse mot trussel. Pass på at du kjøper flere Defender for Office 365-lisenser slik at alle brukerne i omfanget av dine Defender for Office-365 er lisensiert. 
>

### <a name="device-management-with-intune"></a>Enhets behandling med Intune

Du trenger ikke å gjøre endringer i den gjeldende Intune-konfigurasjonen før overføring, som inkluderer registrerte enheter og enhets-og App-innstillinger.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium inkluderer Windows 10 Business, som du kan installere med Windows autopilot. Når du overfører til Microsoft 365-E3, omfatter hver bruker lisens Windows 10 Enterprise E3, som du også kan installere med Windows autopilot.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365-apper for bedrifter

Microsoft 365-appene for Business-klienten som er installert på enhetene dine, begynner automatisk å bruke funksjonene i Microsoft 365-apper for Enterprise. Etter overføring kan du nå bruke:

 - Volum aktivering via gruppe policy
 - App-telemetri
 - Oppdatere kontroller
 - Regne ark sammenligning og forespørsel
 - Forretnings intelligens

