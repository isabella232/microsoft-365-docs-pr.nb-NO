---
title: Klargjøre distribusjon av Office-klient av Microsoft 365 for bedrifter
f1.keywords:
- CSH
ms.author: efrene
author: efrene
manager: scotv
ms.date: 10/31/2017
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: M365-subscription-management
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Lær hvordan du installerer 32-biters Office-apper automatisk på Windows 10-datamaskiner og holder dem oppdatert.
ms.openlocfilehash: 868d06fadfef0f55b41131b7fdfbb368b9128405
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/02/2021
ms.locfileid: "51580058"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-for-business"></a>Klargjøre distribusjon av Office-klient av Microsoft 365 for bedrifter

Denne artikkelen gjelder for Microsoft 365 Business Premium.

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Klargjøre for å installere Office-programmer automatisk på klientmaskiner

Du kan bruke Microsoft 365 Business Premium til å installere 32-biters Office-appene automatisk på Windows 10-datamaskiner og holde dem oppdatert med oppdateringer.
  
Automatisk installasjon fungerer best hvis sluttbrukerens datamaskin er på Windows 10 Business og:
  
- Ikke har eksisterende Office-skrivebordsapper (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access og OneDrive).
    
    eller
    
- Har en eksisterende versjon av Klikk og bruk Office installert.
    
Hvis du vil finne ut om du har klikk og bruk-versjonen av Office, gå til **Fil** \> **Konto** i en hvilken som helst Office-app ( **Office Konto** i Outlook). Hvis du ser **Office-oppdateringer** som vist i figuren nedenfor, ble installasjonen utført ved hjelp av Klikk og bruk. 
  
![Screenshot of Office updates in Office app Account](../media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Hvem drar nytte av å ha denne funksjonen**
  
Sluttbruker med PC som:
  
- **Har**  en Brukerlisens for Windows 10 Business, en aktiv lisens for Microsoft 365 for bedrifter, Windows 10 Creators Update og er med i Azure Active Directory. 
    
- **Har ikke** 64-biters Office-apper (for eksempel Word, Excel, PowerPoint). Hvis det kreves 64-biters Office-apper, passer ikke denne funksjonen, fordi det ikke er støtte for å utløse en 64-biters 2016 Klikk og bruk-versjon av Office fra administrasjonskonsollen for Microsoft 365 for bedrifter. 
    
- **Ikke har** noen frittstående apper for 2016 Windows Installer (MSI) (for eksempel Visio eller Project). Microsoft 365 for bedrifter oppgraderer Office til Klikk og bruk-versjonen av Office 2016, og det fungerer ikke med frittstående Office 2016 MSI-apper. 
    
Tabellen nedenfor viser hvilken handling sluttbrukerne/administratorene må gjøre, avhengig av startstatusen, for å få en vellykket 32-biters Klikk og bruk-versjon av Office-distribusjon fra administrasjonskonsollen for Microsoft 365 for bedrifter.
  
|**Status for Office-installasjon før start**|**Handling som må iverksettes før Office-installasjonen av Microsoft 365 for bedrifter**|**Sluttstatus**|
|:-----|:-----|:-----|
|Ingen Office suite installert  <br/> |Ingen  <br/> |32-biters Office 2016 installeres ved hjelp av Klikk og bruk  <br/> |
|Eksisterende 32-biters Klikk og bruk-versjon av Office (2016 eller tidligere), og ingen frittstående apper  <br/> |Ingen  <br/> |Oppgradert til den nyeste 32-biters Klikk og bruk-versjonen av Office 2016, etter behov **\*** <br/> |
|Eksisterende Klikk og bruk 32-biters versjon av Office og Klikk og bruk 32-biters eller 64-biters frittstående Office-apper (for eksempel Visio, Project)  <br/> |Ingen  <br/> |Frittstående apper påvirkes ikke. Programserien er oppgradert til 32-biters Klikk og bruk-versjon av Office 2016  <br/> |
|Eksisterende 32-biters Klikk og bruk-versjon av Office og eventuelle 32- eller 64-biters (unntatt 2016) MSI frittstående Office-apper  <br/> |Ingen  <br/> |Frittstående apper påvirkes ikke. Programserien er oppgradert til 32-biters Klikk og bruk-versjon av Office 2016  <br/> ||||
|En hvilken som helst eksisterende 64-biters Klikk og bruk-versjon av Office  <br/> |Avinstaller 64-biters Office-apper hvis det er GREIT å erstatte dem med 32-biters Office-apper  <br/> |Hvis Office 64-biters apper blir fjernet, installeres 32-biters Klikk og bruk-versjonen av Office 2016  <br/> |
|En eksisterende MSI-installasjon av Office 2016 med eller uten frittstående apper  <br/> |Avinstallere MSI Office 2016.  <br/> |32-biters versjon av Klikk og bruk av Office 2016 er installert. Ingen endring i frittstående apper  <br/> |
|Eksisterende MSI-installasjon av Office 2013 (eller tidligere) og/eller frittstående Office-apper  <br/> |Ingen  <br/> |32-biters Klikk og bruk-versjonen av Office 2016 med den eksisterende MSI Office-installasjonen (og frittstående apper) finnes side ved side  <br/> |
||||
   
 **(\*) Obs:** Oppgrader ikke til 32-biters Klikk og bruk-versjonen av Office 2016 på grunn av en kjent feil. En løsning pågår. 
  
