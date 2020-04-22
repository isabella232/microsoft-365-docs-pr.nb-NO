---
title: Komme i gang med Microsoft 365 for bedrifter
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
description: Finn ut mer om Microsoft 365 for bedrifter, hvordan du konfigurerer det og hvordan du klargjør brukernes enheter og PCer for å sikre at de er beskyttet av Microsoft 365 for bedrifter.
ms.openlocfilehash: 17b142fb704d1b0be088a649490e751effb19517
ms.sourcegitcommit: 2614f8b81b332f8dab461f4f64f3adaa6703e0d6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/21/2020
ms.locfileid: "43633207"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Komme i gang med Microsoft 365 for bedrifter

## <a name="what-is-microsoft-365-for-business"></a>Hva er Microsoft 365 for bedrifter

Microsoft 365 for bedrifter er et omfattende sett med forretningsproduktivitets- og samarbeidsverktøy, for eksempel Outlook, Word, Excel og andre Office-produkter, som alltid er oppdaterte. Du kan beskytte arbeidsfilene dine på alle iOS-, Android- og Windows 10-enheter med sikkerhet i foretaksklasse som er enkel å administrere.

Se denne videoen for en rask oversikt over Microsoft 365 for bedrifter.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 for bedrifter er ment for opptil 300 lisenser. Hvis du trenger flere lisenser, kan du se Dokumentasjonen for [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) hvis du vil ha mer informasjon. 
  
## <a name="get-microsoft-365-for-business"></a>Skaff deg Microsoft 365 for bedrifter

- Hvis du har en partner, får de Microsoft 365 for bedrifter: [Få Microsoft 365 for bedrifter fra Microsoft Partner Center](get-microsoft-365-business.md).
    
- Hvis du ikke har en partner og ønsker å få Microsoft 365 for bedrifter, kan du [kjøpe den her](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-for-business"></a>Konfigurere Microsoft 365 for bedrifter

 **Oversikt over Microsoft 365 for business Suite som er konfigurert**
  
Diagrammet nedenfor beskriver hvordan administratorer konfigurerer Microsoft 365 for bedrifter. Den beskriver også trinnene for å klargjøre Windows-PCer for Microsoft 365 for bedrifter. Du kan også legge til nye enheter i administrasjonssenteret for Microsoft 365 med [Windows AutoPilot](add-autopilot-devices-and-profile.md). Du kan bruke AutoPilot til å konfigurere og forhåndskonfigurere nye enheter slik at de er klare for produktiv bruk så snart en bruker logger på med microsoft 365 for forretningslegitimasjon.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Se denne videoen for å få en oversikt over installasjonsprogrammet for Microsoft 365 for bedrifter.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Hvis du synes at denne videoen er nyttig, kan du se den [fullstendige opplæringsserien for små bedrifter og de som er nybegynnere i Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: Konfigurere Microsoft 365 for bedrifter (Admin)

Logg på [administrasjonssenteret for Microsoft 365](https://portal.office.com/adminportal/home) med den globale administratorlegitimasjonen, og fullfør følgende fremgangsmåte for å konfigurere Microsoft 365 for bedrifter. 
  
1. [Forutsetninger for å beskytte data på enheter med Microsoft 365 for bedrifter](pre-requisites-for-data-protection.md)
    
    Les forutsetningene først for å forsikre deg om at enhetene er klare for Microsoft 365 for bedrifter.
    
2. [Bruke installasjonsveiviseren til å konfigurere Microsoft 365 for bedrifter](set-up.md)
    
    Hvis du **flytter permanent fra en lokal Active Directory til skyen**, kan du gå til administrasjonssenteret for Microsoft 365 og bruke installasjonsveiviseren til å legge til brukerne manuelt, eller du kan gjøre en engangssynkronisering med Azure AD Connect. Dette kan gjøres på to måter: 
    
    - Hvis du også har en Exchange 2010-, Exchange-2013- eller Exchange-2016-server, kan du [bruke Minimal Hybrid til raskt å overføre Exchange-postbokser til Office 365](https://support.office.com/article/fdecceed-0702-4af3-85be-f2a0013937ef). De minimale hybridtrinnene inkluderer en engangssynkronisering av brukere til Azure AD, og e-postoverføring fra lokale til skyen. Når e-postoverføringen er fullført, deaktiveres katalogsynkroniseringen automatisk når du bruker denne metoden.
    
    - Bruk veiviseren for katalogsynkronisering til å synkronisere brukerne til skyen. Følg trinnene i [Konfigurere katalogsynkronisering for Microsoft 365 for](https://support.office.com/article/1b3b5318-6977-42ed-b5c7-96fa74b08846) å fullføre denne prosessen. Når du synkroniserer brukerne til skyen, må du [deaktivere katalogsynkronisering for Office 365](https://support.office.com/article/ee5f861e-bd48-4267-83d1-a4ead4b4a00d).
    
    Du må også gi hver bruker som ble lagt til på denne måten en lisens til Microsoft 365 for bedrifter. Du kan gjøre dette i [installasjonsveiviseren,](set-up.md) eller du kan [tilordne lisenser til brukere i Microsoft 365 for bedrifter](https://support.office.com/article/997596B5-4173-4627-B915-36ABAC6786DC).
    
### <a name="2-prepare-mobile-devices"></a>2: Klargjøre mobile enheter

Følg trinnene i [Konfigurere mobile enheter for Microsoft 365 for bedrifter](set-up-mobile-devices.md) til å installere Office-apper på enheter og sørge for at de er beskyttet av Microsoft 365 for bedrifter. 
  
### <a name="3-prepare-pcs"></a>3: Klargjøre PCer

Administratorer kan forhåndsvelge innstillinger for nye Windows 10-PCer ved hjelp av [Windows AutoPilot](add-autopilot-devices-and-profile.md). Brukere kan konfigurere eksisterende eller nye Windows 10-enheter ved å følge fremgangsmåten i dette emnet: [Konfigurere Windows-PCer for Microsoft 365 for forretningsbrukere](set-up-windows-devices.md). For eksisterende enheter kan brukere **eventuelt** [flytte filer til OneDrive for Business](move-files-to-onedrive.md). De kan også bruke tredjepartsverktøy til å flytte filer som er knyttet til Windows-profil, til OneDrive.
  
Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 for bedrifter til å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgang til lokale ressurser som krever lokal godkjenning. Følg trinnene i [Aktiver domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 for bedrifter for](manage-windows-devices.md) å konfigurere dette. Denne metoden foretrekkes, og enheter i denne tilstanden kalles **Hybrid Azure AD-tilknyttede enheter**. 
  
Hvis du beholder en lokal Active Directory som inneholder noen lokale ressurser (for eksempel delte filressurser og skrivere), kan du gi **Azure AD-tilknyttede enheter** tilgang til disse ressursene ved å følge fremgangsmåten her: [Få tilgang til lokale ressurser fra en Azure AD-tilknyttet enhet i Microsoft 365 for bedrifter](access-resources.md).
  
  
## <a name="contact-support"></a>Kontakt kundestøtte

 **Hvis du må ta kontakt med kundestøtte:**
  
- Kontakt partneren din.
    
- Som Microsoft 365 for business admin har du tilgang til kundestøtteteamet vårt: ** [Kontakt kundestøtte for forretningsprodukter - Admin Hjelp](https://support.office.com/article/32a17ca7-6fa0-4870-8a8d-e25ba4ccfd4b)**
    
## <a name="see-also"></a>Se også

[Microsoft 365 for forretningsdokumentasjon og ressurser](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Administrere Microsoft 365 for bedrifter](manage.md)[migrere til Microsoft 365 for bedrifter](migrate-to-microsoft-365-business.md)

[Microsoft 365 for business opplæring videoer](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
