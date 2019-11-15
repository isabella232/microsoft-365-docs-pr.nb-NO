---
title: Klargjøre for distribusjon av Office-klienten med Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
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
search.appverid:
- BCS160
- MET150
ms.assetid: ed34fff3-2881-4ed4-9906-1ba6bb8dd804
description: Finn ut hvordan du installerer de 32-biters Office-appene på Windows 10-datamaskiner automatisk og holder dem oppdatert.
ms.openlocfilehash: 09857ddeb28e953da07979045a65f6b91925aeaf
ms.sourcegitcommit: 2c2248b03f7753d64490f2f7e56ec644a235b65a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/15/2019
ms.locfileid: "38640773"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Klargjøre for distribusjon av Office-klienten med Microsoft 365 Business

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Klargjøre for å installere Office-programmer automatisk på klientmaskiner

Du kan bruke Microsoft 365 Business til automatisk å installere 32-biters Office-programmer på Windows 10-datamaskiner og holde dem oppdatert med oppdateringer.
  
Automatisk installasjon fungerer best hvis sluttbrukerens datamaskin er på Windows 10 Business og:
  
- Ikke har eksisterende Office-skrivebordsapper (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access og OneDrive).
    
    eller
    
- Har en eksisterende versjon av Klikk og bruk Office installert.
    
Hvis du vil finne ut om du har klikk og bruk-versjonen av Office, gå til **Fil** \> **Konto** i en hvilken som helst Office-app ( **Office Konto** i Outlook). Hvis du ser **Office-oppdateringer** som vist i illustrasjonen nedenfor, ble installasjonen utført ved hjelp av klikk og bruk. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Hvem drar nytte av denne funksjonen**
  
Sluttbruker med PC som:
  
- **Har** brukerlisens for Windows 10 Business, en aktiv Microsoft 365 Business-lisens, Windows 10 Creators Update og er knyttet til Azure Active Directory. 
    
- **Har ikke** 64-biters Office-programmer (eksempel: Word, Excel, PowerPoint). Hvis 64-biters Office-programmer er påkrevd, er ikke denne funksjonen en god passform, fordi det ikke er støtte for å utløse en 64-biters 2016 Klikk og bruk-versjon av Office fra Microsoft 365 Business admin Console. 
    
- **Ikke har** noen frittstående apper for 2016 Windows Installer (MSI) (for eksempel Visio eller Project). Microsoft 365 Business oppgraderinger Office til Klikk og bruk-versjonen av Office 2016, og som ikke fungerer med Office 2016 MSI frittstående programmer. 
    
Tabellen nedenfor viser hvilken handling sluttbrukere/administratorer må ta, avhengig av deres starttilstand, for å ha en vellykket 32-biters Klikk og bruk-versjon av Office-distribusjon fra Microsoft 365 Business admin Console.
  
|**Status for Office-installasjon før start**|**Handling som skal utføres før Microsoft 365 Business-Office-installasjon**|**Sluttstatus**|
|:-----|:-----|:-----|
|Ingen Office suite installert  <br/> |Ingen  <br/> |Office 2016 32-biters er installert ved hjelp av klikk og bruk  <br/> |
|Eksisterende 32-biters Klikk og bruk-versjon av Office (2016 eller tidligere), og ingen frittstående apper  <br/> |Ingen  <br/> |Oppgradert til den nyeste 32-biters Klikk og bruk-versjonen av Office 2016, etter behov **\*** <br/> |
|Eksisterende Klikk og bruk-32-biters versjon av Office og klikk og bruk 32-biters eller 64-biters frittstående Office-programmer (for eksempel Visio, Project)  <br/> |Ingen  <br/> |Frittstående apper berøres ikke. Programserien er oppgradert til 32-biters Klikk og bruk-versjon av Office 2016  <br/> |
|Eksisterende 32-biters Klikk og bruk-versjon av Office og eventuelle 32- eller 64-biters (unntatt 2016) MSI frittstående Office-apper  <br/> |Ingen  <br/> |Frittstående apper berøres ikke. Programserien er oppgradert til 32-biters Klikk og bruk-versjon av Office 2016  <br/> ||||
|En hvilken som helst eksisterende 64-biters Klikk og bruk-versjon av Office  <br/> |Avinstallere 64-biters Office-programmer, hvis det er OK å erstatte dem med 32-biters Office-programmer  <br/> |Hvis Office 64-biters apper blir fjernet, installeres 32-biters Klikk og bruk-versjonen av Office 2016  <br/> |
|En eksisterende MSI-installasjon av Office 2016 med eller uten frittstående apper  <br/> |Avinstallere MSI Office 2016.  <br/> |32-biters versjon av Klikk og bruk av Office 2016 er installert. Ingen endring i frittstående apper  <br/> |
|Eksisterende MSI-installasjon av Office 2013 (eller tidligere) og/eller frittstående Office-apper  <br/> |Ingen  <br/> |32-biters Klikk og bruk-versjonen av Office 2016 med den eksisterende MSI Office-installasjonen (og frittstående apper) finnes side ved side  <br/> |
||||
   
 **(\*) Obs:** Oppgrader ikke til 32-biters Klikk og bruk-versjonen av Office 2016 på grunn av en kjent feil. En hurtigreparasjon pågår. 
  