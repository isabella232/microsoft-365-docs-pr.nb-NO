---
title: Komme i gang med Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.date: 9/20/2018
ms.audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Lær å konfigurere Microsoft 365 Business.
ms.openlocfilehash: 80c6590a682af5fadeceac7a75e409adac897f6f
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32276735"
---
# <a name="get-started-with-microsoft-365-business"></a>Komme i gang med Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>Hva er Microsoft 365 Business

Microsoft 365 Business er et omfattende sett med forretningsproduktivitet- og samarbeidsverktøy, for eksempel Outlook, Word, Excel og andre Office-produkter som alltid er oppdatert. Du kan beskytte arbeidsfiler på alle iOS-, Android- og Windows 10-enheter med sikkerhet på foretaksnivå som er enkel å administrere.
  
Microsoft 365 Business er beregnet for opptil 300 lisenser. Hvis du trenger flere lisenser, kan du se dokumentasjonen for [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) for å få mer informasjon. 
  
## <a name="get-microsoft-365-business"></a>Skaff deg Microsoft 365 Business

- Hvis du har en partner, vil de få Microsoft 365 Business: [Skaff deg Microsoft 365 Business fra Microsoft Partnersenter](get-microsoft-365-business.md).
    
- Hvis du ikke har en partner og ønsker å skaffe deg Microsoft 365 Business, kan du [kjøpe det her](https://www.microsoft.com/en-us/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Konfigurere Microsoft 365 Business

 **Definere oversikt over Microsoft 365 Business Suite**
  
Følgende diagram beskriver hvordan administratorer Microsoft 365 Business. Den beskriver også hvordan Windows PC-er klargjøres for Microsoft 365 Business. Du kan også legge til nye enheter i administrasjonssenteret for Microsoft 365 Business med [Windows AutoPilot](add-autopilot-devices-and-profile.md). Du kan bruke AutoPilot til å opprette og forhåndskonfigurere nye enheter, slik at de er klare for produktiv bruk når en bruker logger på med Microsoft 365 Business-legitimasjonen sin.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: konfigurere Microsoft 365 Business (Admin)

Logg deg på [administrasjonssenteret for Microsoft 365 Business](https://portal.office.com/adminportal/home) med den globale administratorlegitimasjonen, og følg fremgangsmåten nedenfor for å konfigurere Microsoft 365 Business. 
  
1. [Forutsetninger for å beskytte data på enheter med Microsoft 365 Business](pre-requisites-for-data-protection.md)
    
    Les forhåndskravet først for å sikre at enhetene er klare for Microsoft 365 Business.
    
2. [Konfigurere Microsoft 365 Business ved hjelp av veiviseren for konfigurasjon](set-up.md)
    
    Hvis du er **permanent flytting fra en lokal Active Directory til skyen**, kan du enten legge brukerne manuelt i Microsoft 365 Business administrasjonssenteret ved hjelp av veiviseren for installasjon av, eller du kan gjøre en engangs synkronisering med Azure AD-tilkobling. Dette kan gjøres på to måter: 
    
  - Hvis du har også en Exchange 2010, Exchange 2013 eller 2016 for Exchange server, kan du [Bruke minimalt Hybrid til å raskt overføre Exchange-postbokser til Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). De minimale hybridtrinnene omfatter en engangs synkronisering av brukere til Azure AD samt e-postoverføring fra lokalt til skyen. Når e-postoverføringen er fullført, er katalogsynkronisering automatisk deaktivert når du bruker denne metoden.
    
  - Bruk veiviseren for katalogsynkronisering for Office 365 for å synkronisere brukerne til skyen. Følg trinnene i [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) for å fullføre denne prosessen. Når du synkroniserer brukerne til skyen, må du [Turn off directory synchronization for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Du må også gi hver bruker som ble lagt til på denne måten, en lisens til Microsoft 365 Business. Du kan gjøre dette i [installasjonsveiviseren](set-up.md), eller [tilordne lisenser til brukere i Office 365 for bedrifter](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: klargjøre mobile enheter

Følg trinnene i[konfigurere mobile enheter for forretningsbrukere som Microsoft 365](set-up-mobile-devices.md) å installere Office-programmer på enheter og gjør at de er beskyttet av Microsoft 365 Business. 
  
### <a name="3-prepare-pcs"></a>3: klargjøre PCer

Administratorer kan velge innstillinger for nye enheter Windows 10 datamaskiner før ved hjelp av [Windows AutoPilot](add-autopilot-devices-and-profile.md). Brukere kan definere sine eksisterende eller nye Windows 10 enheter ved å følge fremgangsmåten i dette emnet: [konfigurere Windows-PCer for bedrifter i Microsoft 365](set-up-windows-devices.md). For eksisterende enheter kan brukere også **eventuelt**[flytte filene til OneDrive for bedrifter](move-files-to-onedrive.md). De kan også bruke tredjeparts-verktøy til å flytte filer som er knyttet til Windows-profil til OneDrive.
  
Hvis organisasjonen bruker Windows Server Active Directory på lokaler, kan du definere Microsoft 365 Business til å beskytte Windows 10 enheter, samtidig som du har tilgang til lokale ressurser som krever lokal godkjenning. Følg trinnene i [aktivere domenetilknyttede Windows 10 enheter som skal administreres av Microsoft 365 Business](manage-windows-devices.md) å sette opp dette. Dette er den foretrukne metoden og enheter i denne tilstanden kalles **Hybrid Azure AD koblet enheter**. 
  
Hvis du beholder en lokal Active Directory, som inneholder noen lokale ressurser (for eksempel delte filer og skrivere), kan du gi din **Azure AD-koblet enheter** tilgang til disse ressursene ved å følge fremgangsmåten her: [Access lokale ressurser fra en Azure AD-koblet enheten i Microsoft 365 Business](access-resources.md).
  
Etter at du har satt opp Windows 10-PCer, kan du [installere Office automatisk](auto-install-or-uninstall-office.md) til enhetene. 
  
## <a name="contact-support"></a>Kontakt kundestøtte

 **Hvis du må ta kontakt med kundestøtte:**
  
- Kontakt partneren din.
    
- Du har tilgang til kundestøtteavdelingen, ** [Kontakt kundestøtte for produkter for bedrifter - Admin hjelp](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b) som en Microsoft 365 Business admin**
    

