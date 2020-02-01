---
title: Klargjøre for distribusjon av Office-klienten med Microsoft 365 Business
f1.keywords:
- CSH
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
ms.openlocfilehash: fa5b2ce1852ebdb1e76c1fa844793fee56af3d68
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593623"
---
# <a name="prepare-for-office-client-deployment-by-microsoft-365-business"></a>Klargjøre for distribusjon av Office-klienten med Microsoft 365 Business

## <a name="prepare-to-automatically-install-office-apps-to-client-computers"></a>Klargjøre for å installere Office-programmer automatisk på klientmaskiner

Du kan bruke Microsoft 365 Business til å installere 32-biters Office-apper automatisk på Windows 10-datamaskiner og holde dem oppdatert med oppdateringer.
  
Automatisk installasjon fungerer best hvis sluttbrukerens datamaskin er på Windows 10 Business og:
  
- Ikke har eksisterende Office-skrivebordsapper (Word, Excel, PowerPoint, Outlook, OneNote, Publisher, Access og OneDrive).
    
    eller
    
- Har en eksisterende versjon av Klikk og bruk Office installert.
    
Hvis du vil finne ut om du har klikk og bruk-versjonen av Office, gå til **Fil** \> **Konto** i en hvilken som helst Office-app ( **Office Konto** i Outlook). Hvis du **ser Office-oppdateringer** som vist i figuren nedenfor, ble installasjonen utført ved hjelp av Klikk og bruk. 
  
![Screenshot of Office updates in Office app Account](media/e3439380-fa43-4ed6-ae5d-64851c297df5.png)
  
 **Hvem drar nytte av å ha denne funksjonen**
  
Sluttbruker med PC som:
  
- **Har** brukerlisens for Windows 10 Business, en aktiv Microsoft 365 Business-lisens, Windows 10 Creators Update og er knyttet til Azure Active Directory. 
    
- **Har ikke** 64-biters Office-apper (f.eks. Word, Excel, PowerPoint). Hvis 64-biters Office-apper er nødvendig, passer ikke denne funksjonen fordi det ikke finnes støtte for å utløse en 64-biters 2016 Klikk og bruk-versjon av Office fra administrasjonskonsollen for Microsoft 365 Business. 
    
- **Ikke har** noen frittstående apper for 2016 Windows Installer (MSI) (for eksempel Visio eller Project). Microsoft 365 Business oppgraderer Office til Klikk og kjør-versjonen av Office-2016, og som ikke fungerer med frittstående Office 2016 MSI-apper. 
    
Tabellen nedenfor viser hvilken handling sluttbrukerne/administratorene må utføre, avhengig av starttilstanden, for å ha en vellykket 32-biters Klikk og bruk-versjon av Office-distribusjon fra administrasjonskonsollen for Microsoft 365 Business.
  
|**Status for Office-installasjon før start**|**Handling som skal utføres før Microsoft 365 Business-Office-installasjon**|**Sluttstatus**|
|:-----|:-----|:-----|
|Ingen Office suite installert  <br/> |Ingen  <br/> |Office 2016 32-biters er installert ved hjelp av Klikk og bruk  <br/> |
|Eksisterende 32-biters Klikk og bruk-versjon av Office (2016 eller tidligere), og ingen frittstående apper  <br/> |Ingen  <br/> |Oppgradert til den nyeste 32-biters Klikk og bruk-versjonen av Office 2016, etter behov **\*** <br/> |
|Eksisterende Klikk og bruk 32-biters versjon av Office og Klikk og bruk 32-biters eller 64-biters frittstående Office-apper (for eksempel Visio, Project)  <br/> |Ingen  <br/> |Frittstående apper påvirkes ikke. Programserien er oppgradert til 32-biters Klikk og bruk-versjon av Office 2016  <br/> |
|Eksisterende 32-biters Klikk og bruk-versjon av Office og eventuelle 32- eller 64-biters (unntatt 2016) MSI frittstående Office-apper  <br/> |Ingen  <br/> |Frittstående apper påvirkes ikke. Programserien er oppgradert til 32-biters Klikk og bruk-versjon av Office 2016  <br/> ||||
|En hvilken som helst eksisterende 64-biters Klikk og bruk-versjon av Office  <br/> |Avinstaller 64-biters Office-apper, hvis det er ok å erstatte dem med 32-biters Office-apper  <br/> |Hvis Office 64-biters apper blir fjernet, installeres 32-biters Klikk og bruk-versjonen av Office 2016  <br/> |
|En eksisterende MSI-installasjon av Office 2016 med eller uten frittstående apper  <br/> |Avinstallere MSI Office 2016.  <br/> |32-biters versjon av Klikk og bruk av Office 2016 er installert. Ingen endring i frittstående apper  <br/> |
|Eksisterende MSI-installasjon av Office 2013 (eller tidligere) og/eller frittstående Office-apper  <br/> |Ingen  <br/> |32-biters Klikk og bruk-versjonen av Office 2016 med den eksisterende MSI Office-installasjonen (og frittstående apper) finnes side ved side  <br/> |
||||
   
 **(\*) Obs:** Oppgrader ikke til 32-biters Klikk og bruk-versjonen av Office 2016 på grunn av en kjent feil. En løsning pågår. 
  