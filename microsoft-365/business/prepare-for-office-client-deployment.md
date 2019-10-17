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
description: Lær hvordan du installerer 32-biters Office-apper automatisk på Windows 10-datamaskiner og holder dem oppdatert.
ms.openlocfilehash: 5b28c1e62d813c52b41ce8e7619c865cdf7690e2
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575822"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Klargjøre for distribusjon av Office-klienten med Microsoft 365 Business

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Klargjøre for å installere Office-programmer automatisk på klientmaskiner

Du kan bruke Microsoft 365 Business for automatisk å installere 32-biters Office-appene på datamaskiner med Windows 10 og for å holde dem automatisk oppdatert med oppdateringer.
  
Dette fungerer best hvis sluttbrukerens datamaskin bruker Windows 10 Business og:
  
- Ikke har eksisterende Office-skrivebordsapper (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access og OneDrive).
    
    eller
    
- Har en eksisterende versjon av Klikk og bruk Office installert.
    
Hvis du vil finne ut om du har klikk og bruk-versjonen av Office, gå til **Fil** \> **Konto** i en hvilken som helst Office-app ( **Office Konto** i Outlook). Hvis du ser Office-oppdateringer som vist i figuren nedenfor, ble installasjonen utført ved hjelp av Klikk og bruk. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Hvem vil dra nytte av denne funksjonen**
  
Sluttbruker med PC som:
  
- **Har** brukerlisens for Windows 10 Business, en aktiv Microsoft 365 Business-lisens, Windows 10 Creators Update og er knyttet til Azure Active Directory. 
    
- **Ikke har** 64-biters Office-apper (for eksempel: Word, Excel og PowerPoint). Hvis 64-biters Office-apper er påkrevd, er denne funksjonen ikke å anbefale fordi det ikke er noen støtte for å utløse en 64-biters 2016 Klikk og bruk-versjon av Office fra Microsoft 365 Business-administrasjonskonsollen. 
    
- **Ikke har** noen frittstående apper for 2016 Windows Installer (MSI) (for eksempel Visio eller Project). Microsoft 365 Business oppgraderer Office til Klikk og bruk-versjonen av Office 2016, og det fungerer ikke med frittstående apper for Office 2016 MSI. 
    
I tabellen nedenfor finner du detaljert informasjon om hvilken handling sluttbrukere/administratorer må utføre, avhengig av startstatus, for å få en vellykket 32-biters Klikk og bruk-versjon av Office-distribusjon fra Microsoft 365 Business-administrasjonskonsollen.
  
|**Status for Office-installasjon før start**|**Handling som skal utføres før Microsoft 365 Business-Office-installasjon**|**Sluttstatus**|
|:-----|:-----|:-----|
|Ingen Office suite installert  <br/> |Ingen  <br/> |Office 2016 32-biters er installert ved hjelp av Klikk og bruk  <br/> |
|Eksisterende 32-biters Klikk og bruk-versjon av Office (2016 eller tidligere), og ingen frittstående apper  <br/> |Ingen  <br/> |Oppgradert til den nyeste 32-biters Klikk og bruk-versjonen av Office 2016, etter behov **\*** <br/> |
|Eksisterende 32-biters Klikk og bruk-versjon av Office samt 32 - eller 64-biters frittstående Office-apper (for eksempel Visio og Project)  <br/> |Ingen  <br/> |Frittstående apper berøres ikke. Programserien er oppgradert til 32-biters Klikk og bruk-versjon av Office 2016  <br/> |
|Eksisterende 32-biters Klikk og bruk-versjon av Office og eventuelle 32- eller 64-biters (unntatt 2016) MSI frittstående Office-apper  <br/> |Ingen  <br/> |Frittstående apper berøres ikke. Programserien er oppgradert til 32-biters Klikk og bruk-versjon av Office 2016  <br/> ||||
|En hvilken som helst eksisterende 64-biters Klikk og bruk-versjon av Office  <br/> |Avinstaller 64-biters Office-apper hvis det er greit å erstatte dem med 32-biters Office-apper  <br/> |Hvis Office 64-biters apper blir fjernet, installeres 32-biters Klikk og bruk-versjonen av Office 2016  <br/> |
|En eksisterende MSI-installasjon av Office 2016 med eller uten frittstående apper  <br/> |Avinstallere MSI Office 2016.  <br/> |32-biters versjon av Klikk og bruk av Office 2016 er installert. Ingen endring i frittstående apper  <br/> |
|Eksisterende MSI-installasjon av Office 2013 (eller tidligere) og/eller frittstående Office-apper  <br/> |Ingen  <br/> |32-biters Klikk og bruk-versjonen av Office 2016 med den eksisterende MSI Office-installasjonen (og frittstående apper) finnes side ved side  <br/> |
||||
   
 **(\*) Obs:** Oppgrader ikke til 32-biters Klikk og bruk-versjonen av Office 2016 på grunn av en kjent feil. Rettelse pågår. 
  


