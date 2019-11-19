---
title: Komme i gang med Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Lær hvordan du konfigurerer Microsoft 365 Business.
ms.openlocfilehash: f269e970cc1ee5ba7455ea799b238db577116f09
ms.sourcegitcommit: 38934a2115d5cdeb44c7484d57be07686c6f7720
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704119"
---
# <a name="get-started-with-microsoft-365-business"></a>Komme i gang med Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>Hva er Microsoft 365 Business

Microsoft 365 Business er et omfattende sett med verktøy for forretningsproduktivitet og samarbeid, for eksempel Outlook, Word, Excel og andre Office-produkter, som alltid er oppdatert. Du kan beskytte arbeidsfilene dine på alle iOS-, Android-og Windows 10-enhetene dine med sikkerhet i foretaksklasse som er enkel å administrere.
  
Microsoft 365 Business er ment for opptil 300 lisenser. Hvis du trenger flere lisenser, kan du se [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) -dokumentasjonen for mer informasjon. 
  
## <a name="get-microsoft-365-business"></a>Skaff deg Microsoft 365 Business

- Hvis du har en partner, vil de få Microsoft 365 Business: [få microsoft 365 Business fra Microsoft Partner Center](get-microsoft-365-business.md).
    
- Hvis du ikke har en partner og ønsker å skaffe deg Microsoft 365 Business, kan du [kjøpe det her](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Konfigurere Microsoft 365 Business

 **Oversikt over Microsoft 365 Business Suite-oppsett**
  
Diagrammet nedenfor beskriver hvordan administratorer konfigurerer Microsoft 365 Business. Den beskriver også hvordan Windows PC-er klargjøres for Microsoft 365 Business. Du kan også legge til nye enheter i Microsoft 365 Business Administrasjonssenter med [Windows autopilot](add-autopilot-devices-and-profile.md). Du kan bruke AutoPilot til å konfigurere og forhånds konfigurere nye enheter, slik at de er klare for produktiv bruk så snart en bruker logger på med Microsoft 365 Business-legitimasjon.
  
![A diagram that shows the setup and management flow for admins, and also for a user](media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)
  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Konfigurer Microsoft 365 Business (admin)

Logg på [microsoft 365 Business Administrasjonssenter](https://portal.office.com/adminportal/home) med legitimasjonen for global administrator, og Fullfør fremgangsmåten nedenfor for å konfigurere Microsoft 365 Business. 
  
1. [Forutsetninger for å beskytte data på enheter med Microsoft 365 Business](pre-requisites-for-data-protection.md)
    
    Les forutsetningene først for å kontrollere at enhetene er klare for Microsoft 365 Business.
    
2. [Bruk installasjonsveiviseren til å konfigurere Microsoft 365 Business](set-up.md)
    
    Hvis du **flytter fra en lokal Active Directory til skyen for godt**, kan du gå til administrasjonssenteret for Microsoft 365 og bruke installasjonsveiviseren til å legge til brukerne manuelt, eller du kan gjøre en en gangs synkronisering med Azure ad-tilkobling. Dette kan gjøres på to måter: 
    
    - Hvis du også har en Exchange-2010, Exchange 2013 eller Exchange 2016-server, kan du [bruke minimal hybrid til raskt å overføre Exchange-postbokser til Office-365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). De minimale hybrid trinnene inkluderer en en gangs synkronisering av brukere til Azure AD, og e-postoverføring fra lokale til skyen. Etter at e-postoverføring er fullført, deaktiveres katalogsynkroniseringen automatisk når du bruker denne metoden.
    
    - Bruk veiviseren for katalogsynkronisering i Office 365 til å synkronisere brukerne til skyen. Følg trinnene i [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) for å fullføre denne prosessen. Når du har synkronisert brukerne til skyen, må du [slå av katalogsynkronisering for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Du må også gi hver bruker som ble lagt til på denne måten en lisens til Microsoft 365 Business. Du kan gjøre dette i [installasjonsveiviseren](set-up.md) , eller du kan [Tilordne lisenser til brukere i Office 365 for bedrifter](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: klargjør mobile enheter

Følg trinnene i [konfigurere mobile enheter for Microsoft 365 Business-brukere](set-up-mobile-devices.md) å installere Office-programmer på enheter, og sørg for at de er beskyttet av Microsoft 365 Business. 
  
### <a name="3-prepare-pcs"></a>3: klargjøre PCer

Administratorer kan forhånds velge innstillinger for nye Windows 10-PCer ved hjelp av [Windows autopilot](add-autopilot-devices-and-profile.md). Brukere kan konfigurere sine eksisterende eller nye Windows 10-enheter ved å følge fremgangsmåten i dette emnet: [konfigurere Windows-PCer for Microsoft 365 Business-brukere](set-up-windows-devices.md). For eksisterende enheter kan brukere **eventuelt** [flytte filer til OneDrive for Business](move-files-to-onedrive.md). De kan også bruke tredjepartsverktøy til å flytte filer som er knyttet til Windows-profilen, til OneDrive.
  
Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business for å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgang til lokale ressurser som krever lokal godkjenning. Følg trinnene i [aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business](manage-windows-devices.md) for å konfigurere dette. Denne metoden foretrekkes, og enheter i denne tilstanden kalles **hybrid Azure ad koblet enheter**. 
  
Hvis du beholder en lokal Active Directory som inneholder noen lokale ressurser (for eksempel delte filressurser og skrivere), kan du gi dine **Azure ad-tilknyttede enheter** tilgang til disse ressursene ved å følge fremgangsmåten her: [få tilgang til lokale ressurser fra en Azure ad-sammenkoblet enhet i Microsoft 365 Business](access-resources.md).
  
  
## <a name="contact-support"></a>Kontakt kundestøtte

 **Hvis du må ta kontakt med kundestøtte:**
  
- Kontakt partneren din.
    
- Som en Microsoft 365 Business-administrator har du tilgang til vårt kundestøtteteam: ** [Kontakt kundestøtte for bedriftsprodukter-admin hjelp](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="related-topics"></a>Beslektede emner
[Microsoft 365 Business-dokumentasjon og -ressurser](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Administrere Microsoft 365 Business](manage.md)[Overføre til Microsoft 365 Business](migrate-to-microsoft-365-business.md)
  

