---
title: Komme i gang med Microsoft 365 Business
f1.keywords:
- NOCSH
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
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Finn ut mer om Microsoft 365 Business, hvordan du konfigurerer det og hvordan du klargjør brukernes enheter og PCer for å sikre at de er beskyttet av Microsoft 365 Business.
ms.openlocfilehash: 220fb747e2bc501f3f6d46d967b30d2e5fd79a4a
ms.sourcegitcommit: 217de0fc54cbeaea32d253f175eaf338cd85f5af
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/07/2020
ms.locfileid: "42561444"
---
# <a name="get-started-with-microsoft-365-business"></a>Komme i gang med Microsoft 365 Business

## <a name="what-is-microsoft-365-business"></a>Hva er Microsoft 365 Business

Microsoft 365 Business er et omfattende sett med forretningsproduktivitets- og samarbeidsverktøy, for eksempel Outlook, Word, Excel og andre Office-produkter, som alltid er oppdaterte. Du kan beskytte arbeidsfilene dine på alle iOS-, Android- og Windows 10-enheter med sikkerhet i foretaksklasse som er enkel å administrere.

Se denne videoen for en rask oversikt over Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 Business er ment for opptil 300 lisenser. Hvis du trenger flere lisenser, kan du se Dokumentasjonen for [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) hvis du vil ha mer informasjon. 
  
## <a name="get-microsoft-365-business"></a>Skaff deg Microsoft 365 Business

- Hvis du har en partner, får de Microsoft 365 Business: [Få Microsoft 365 Business fra Microsoft Partner Center](get-microsoft-365-business.md).
    
- Hvis du ikke har en partner og ønsker å skaffe deg Microsoft 365 Business, kan du [kjøpe det her](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-business"></a>Konfigurere Microsoft 365 Business

 **Oversikt over Microsoft 365 Business Suite-oppsett**
  
Diagrammet nedenfor beskriver hvordan administratorer konfigurerer Microsoft 365 Business. Den beskriver også hvordan Windows PC-er klargjøres for Microsoft 365 Business. Du kan også legge til nye enheter i administrasjonssenteret for Microsoft 365 Business med [Windows AutoPilot](add-autopilot-devices-and-profile.md). Du kan bruke AutoPilot til å konfigurere og forhåndskonfigurere nye enheter slik at de er klare for produktiv bruk så snart en bruker logger på med legitimasjonen for Microsoft 365 Business.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Se denne videoen for å få en oversikt over installasjonsprogrammet for Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Hvis du synes at denne videoen er nyttig, kan du se den [fullstendige opplæringsserien for små bedrifter og de som er nybegynnere i Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-business-admin"></a>1: Konfigurere Microsoft 365 Business (Admin)

Logg på administrasjonssenteret for [Microsoft 365 Business](https://portal.office.com/adminportal/home) med den globale administratorlegitimasjonen, og fullfør følgende fremgangsmåte for å konfigurere Microsoft 365 Business. 
  
1. [Forutsetninger for å beskytte data på enheter med Microsoft 365 Business](pre-requisites-for-data-protection.md)
    
    Les forutsetningene først for å forsikre deg om at enhetene er klare for Microsoft 365 Business.
    
2. [Bruke installasjonsveiviseren til å konfigurere Microsoft 365 Business](set-up.md)
    
    Hvis du **flytter permanent fra en lokal Active Directory til skyen**, kan du gå til administrasjonssenteret for Microsoft 365 Business og bruke installasjonsveiviseren til å legge til brukerne manuelt, eller du kan gjøre en engangssynkronisering med Azure AD Connect. Dette kan gjøres på to måter: 
    
    - Hvis du også har en Exchange 2010-, Exchange-2013- eller Exchange-2016-server, kan du [bruke Minimal Hybrid til raskt å overføre Exchange-postbokser til Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). De minimale hybridtrinnene inkluderer en engangssynkronisering av brukere til Azure AD, og e-postoverføring fra lokale til skyen. Når e-postoverføringen er fullført, deaktiveres katalogsynkroniseringen automatisk når du bruker denne metoden.
    
    - Bruk veiviseren for katalogsynkronisering av Office 365 til å synkronisere brukerne til skyen. Følg trinnene i [Set up directory synchronization for Office 365](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) for å fullføre denne prosessen. Når du synkroniserer brukerne til skyen, må du [deaktivere katalogsynkronisering for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Du må også gi hver bruker som ble lagt til på denne måten en lisens til Microsoft 365 Business. Du kan gjøre dette i [installasjonsveiviseren,](set-up.md) eller du kan [tilordne lisenser til brukere i Office 365 for bedrifter](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: Klargjøre mobile enheter

Følg trinnene i [Konfigurere mobile enheter for Microsoft 365 Business-brukere](set-up-mobile-devices.md) til å installere Office-apper på enheter og kontrollere at de er beskyttet av Microsoft 365 Business. 
  
### <a name="3-prepare-pcs"></a>3: Klargjøre PCer

Administratorer kan forhåndsvelge innstillinger for nye Windows 10-PCer ved hjelp av [Windows AutoPilot](add-autopilot-devices-and-profile.md). Brukere kan konfigurere eksisterende eller nye Windows 10-enheter ved å følge fremgangsmåten i dette emnet: [Konfigurere Windows-PCer for Microsoft 365 Business-brukere](set-up-windows-devices.md). For eksisterende enheter kan brukere **eventuelt** [flytte filer til OneDrive for Business](move-files-to-onedrive.md). De kan også bruke tredjepartsverktøy til å flytte filer som er knyttet til Windows-profil, til OneDrive.
  
Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 Business til å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgang til lokale ressurser som krever lokal godkjenning. Følg trinnene i [Aktiver domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business](manage-windows-devices.md) for å konfigurere dette. Denne metoden foretrekkes, og enheter i denne tilstanden kalles **Hybrid Azure AD-tilknyttede enheter**. 
  
Hvis du beholder en lokal Active Directory som inneholder noen lokale ressurser (for eksempel delte filressurser og skrivere), kan du gi **Azure AD-tilknyttede enheter** tilgang til disse ressursene ved å følge fremgangsmåten her: [Få tilgang til lokale ressurser fra en Azure AD-tilknyttet enhet i Microsoft 365 Business](access-resources.md).
  
  
## <a name="contact-support"></a>Kontakt kundestøtte

 **Hvis du må ta kontakt med kundestøtte:**
  
- Kontakt partneren din.
    
- Som administrator for Microsoft 365 Business har du tilgang til kundestøtteteamet vårt: ** [Kontakt kundestøtte for forretningsprodukter - Hjelp for administratorer](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="see-also"></a>Se også

[Microsoft 365 Business-dokumentasjon og -ressurser](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Administrere Microsoft 365 Business](manage.md)[Overføre til Microsoft 365 Business](migrate-to-microsoft-365-business.md)

[Opplæringsvideoer for Microsoft 365-bedrifter](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
