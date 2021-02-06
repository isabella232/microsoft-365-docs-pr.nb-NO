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
ms.openlocfilehash: 019a422bb879389f42a32cf30f9a8094f776078a
ms.sourcegitcommit: eac5d9f759f290d3c51cafaf335a1a1c43ded927
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/06/2021
ms.locfileid: "50126205"
---
# <a name="migrate-from-microsoft-365-business-premium-to-microsoft-365-e3"></a>Overføre fra Microsoft 365 Business Premium til Microsoft 365 E3

Microsoft 365 Business Premium har alt du trenger for småbedriften din, og kombinerer skybaserte produktivitetsapper i klassen med enkel enhetsbehandling og sikkerhet som gjør det mulig for ansatte å gjøre sitt beste arbeid. I noen tilfeller må du kanskje overføre Microsoft 365 Business Premium-abonnementet til Microsoft 365 E3. 

Bedriften din har for eksempel vokser og trenger mer enn 300 lisenser (gratulerer forresten).

Eller bedriften din trenger bedriftsfunksjoner, for eksempel Microsoft 365 Apps for Enterprise, Windows 10 Enterprise E3 eller Tilgangslisenser for Enterprise-klienter.

Oppgradering er enkelt: Du kan starte oppgraderingen [fra administrasjonssenteret.](../commerce/subscriptions/upgrade-to-different-plan.md) Alle dataene og konfigurasjonen i det gjeldende abonnementet opprettholdes. Det er ingenting du trenger å gjøre for å klargjøre for overføringen, og ingenting skal gjøre etterpå, bortsett fra å dra nytte av de nye funksjonene.

>[!Note]
>Du kan også bruke et Microsoft 365 Business Premium-abonnement for opptil 300 seter og få et Microsoft 365 E3-abonnement for mer enn 300 seter. Microsoft Defender for Office 365 er imidlertid ikke inkludert i Microsoft 365 E3. For fortsatt trusselbeskyttelse bør du legge til flere Defender for Office 365-lisenser, slik at alle brukerne i omfanget av Defender for Office 365-politiene er lisensiert.
>

## <a name="differences-between-microsoft-365-business-premium-and-microsoft-365-enterprise"></a>Forskjeller mellom Microsoft 365 Business Premium og Microsoft 365 Enterprise

Denne tabellen viser forskjellene mellom Microsoft 365 Business Premium og Microsoft 365 E3.

| Funksjon    | Støtte i Microsoft 365 Business Premium    | Støtte i Microsoft 365 E3 | 
|:-------|:-----|:-----|
| **Lokalt**        | | | 
| Windows 10    | Windows 10 Business  |     Windows 10 Enterprise E3| 
| Office-apper*    | [Microsoft 365 Apps for business](#office-365-business)    | Microsoft 365 Apps for enterprise | 
| **Skyproduktivitetsapper**        | | | 
| Exchange Online og Outlook    | 50 GB lagringsgrense per postboks og ubegrenset Exchange Online-arkivering    | Lagringsgrense på 100 GB per postboks og ubegrenset Exchange Online-arkivering | 
| Team    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| OneDrive for Business    | 1 TB lagringsgrense per bruker    | Ubegrenset | 
| Yammer, SharePoint Online, Planner, Stream    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| MileIQ    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | | 
| **Threat Protection**        | | | 
| Funksjoner for reduksjon av angrepsoverflater    | [Se denne listen](#threat-protection) | Administrasjon av maskinvarebasert isolering for Microsoft Edge | 
| Defender for Office 365 Plan 1 | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | Ikke inkludert, men kan legges til i | 
| **Identitetsbehandling**        | | | 
| Selvbetjent tilbakestilling av passord for hybrid Azure Active Directory-kontoer (Azure AD), Azure AD-godkjenning med flere faktorer (MFA), betinget tilgang, tilbakeskriving av passord for lokale identiteter|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Oppdagelse av skyapper, Azure AD Connect-tilstand    |     | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Azure AD Office 365-apper for enkel Sign-On (SSO): 10 apper per bruker (Galleri SaaS-apper som Salesforce)* | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Azure AD Premium 1 SSO: ingen grense (lokale apper via Azure AD-programproxy og apper uten galleri ved hjelp Self-Service appintegreringsmaler)    |     | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| **Enhets- og appbehandling**        | | | 
| Microsoft Intune, Windows Autopilot|     ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
|Tilgang til virtuelt skrivebord (VDA)    |  |     ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
|Windows Virtuelt skrivebord (WVD)    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png) |     ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
|Aktivering av delt datamaskin (SCA)    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png) |     ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Optimaliseringspakke for Microsoft Desktop    | |     ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| **Informasjonsbeskyttelse**        | | | 
| Office 365 Data Loss Prevention, Azure Information Protection Plan 1    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Windows Information Protection for endepunkt-DLP    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| **Lisens for klienttilgang (CAL-rettigheter)**    | | |     
| Enterprise CAL Suite (Exchange, SharePoint, Skype, Windows, Microsoft Endpoint Configuration Manager, Windows Rights Management)| |         ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| **Samsvar**        | | | 
| Ubegrenset e-postarkivering    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Samsvarsbehandling    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| eDiscovery    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| In-place hold and litigation hold    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
| Oppbevaringskoder og oppbevaringspolicyer for meldingsposterbehandling (MRM)    | ![Inkludert i Microsoft 365 Business Premium](../media/check-mark.png)    | ![Inkludert i Microsoft 365 E3](../media/check-mark.png) | 
||||

\* Brukere som har fått tilgang til SaaS-apper, kan få SSO-tilgang til opptil 10 apper. Administratorer kan konfigurere enkel pålogging og endre brukertilgang til forskjellige SaaS-apper, men SSO-tilgang er bare tillatt for 10 apper per bruker om gangen. Alle Office 365-apper telles som én enkelt app.

## <a name="migration"></a>Overføring

Hvis du vil overføre, samarbeider du med partneren for å flytte Abonnementet og lisensene for Microsoft 365 Business Premium til et passende Abonnement på Microsoft 365 E3 med lisensene.

Avsnittene nedenfor beskriver hvilke endringer du må gjøre, hvis det er noen, og hva du kan gjøre etter overføringen.

### <a name="microsoft-365-subscription-configuration-and-data"></a>Konfigurasjon og data for Microsoft 365-abonnement

Du trenger ikke å gjøre endringer i det gjeldende abonnementet eller dataene før du overfører, noe som omfatter:

- Abonnementskonfigurasjon, for eksempel DNS-domenenavn.
- Bruker- og gruppekontoer og godkjenningsinnstillinger, for eksempel godkjenning med flere faktorer eller policyer for betinget tilgang.
- Produktivitetstjenestekonfigurasjoner og deres data, for eksempel Teams, Exchange Online-postbokser, SharePoint Online-nettsteder, OneDrive for Business-mapper og OneNote-notatblokker.

Brukerne kan nå få ubegrenset lagringsplass i Exchange Online-postbokser og OneDrive for Business-mapper.

Du kan begynne å bruke Cloud App Discovery, Azure AD Connect Health og SSO for mer enn 10 apper.

>[!Note]
>Brukere som er overført til Microsoft 365 E3, kan ikke lenger bruke MileIQ.
>

<a name="threat-protection"></a>
### <a name="threat-protection"></a>Trusselbeskyttelse

Windows 10 Business omfatter disse beskyttelsene:

- Integritetshåndhevelse av oppstartsprosessen for operativsystemet
- Integritetshåndhevelse av sensitive operativkomponenter
- Advanced vulnerability and zero-day exploit mitigations
- Omdømmebasert nettverksbeskyttelse for Microsoft Edge, Internet Explorer og Chrome
- Vertsbasert brannmur
- Tiltak for løsepengevirus
- Maskinvarebasert isolering for Microsoft Edge
- Programkontroll levert av intelligent sikkerhetsgraf
- Enhetskontroll (USB)
- Nettverksbeskyttelse for nettbaserte trusler
- Regler for hindring av inntrenging

Windows 10 Enterprise E3 omfatter også administrasjon av maskinvarebasert isolering for Microsoft Edge.

>[!Note]
>Brukere som er overført til Microsoft 365 E3, krever hver av dem en Microsoft Defender for Office 365-lisens for fortsatt trusselbeskyttelse. Pass på å kjøpe flere Defender for Office 365-lisenser slik at alle brukere i omfanget av defenderen for Office 365-politi er lisensiert. 
>

### <a name="device-management-with-intune"></a>Enhetsbehandling med Intune

Du trenger ikke å gjøre endringer i den gjeldende Intune-konfigurasjonen før du overfører, som omfatter registrerte enheter og innstillinger for enhet og app.

### <a name="windows-10"></a>Windows 10

Microsoft 365 Business Premium inkluderer Windows 10 Business, som du kan installere med Windows AutoPilot. Når du overfører til Microsoft 365 E3, inkluderer hver brukerlisens Windows 10 Enterprise E3, som du også kan installere med Windows Autopilot.

<a name="office-365-business"></a>
###  <a name="microsoft-365-apps-for-business"></a>Microsoft 365 Apps for business

Microsoft 365 Apps for Business-klienten som er installert på enhetene dine, begynner automatisk å bruke funksjonene i Microsoft 365 Apps for Enterprise. Etter overføringen kan du nå bruke:

 - Støtte for gruppepolicy
 - Regnearksammenligning og spørring
 - Forretningsintelligens

