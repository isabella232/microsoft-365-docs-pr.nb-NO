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
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 496e690b-b75d-4ff5-bf34-cc32905d0364
description: Finn ut mer om Microsoft 365 for bedrifter, hvordan du konfigurerer det, og hvordan du klargjør brukernes enheter og PC-er for å sikre at de er beskyttet av Microsoft 365 for Business.
ms.openlocfilehash: ec50036f589cfd8497b0e7e9af6519b30d25dcd3
ms.sourcegitcommit: 555d756c69ac9031d1fb928f2e1f9750beede066
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/29/2020
ms.locfileid: "47306493"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Komme i gang med Microsoft 365 for bedrifter

## <a name="what-is-microsoft-365-for-business"></a>Hva er Microsoft 365 for bedrifter

Microsoft 365 for Business er et omfattende sett med bedrifts produktivitets-og samarbeids verktøy, for eksempel Outlook, Word, Excel og andre Office-produkter, som alltid er oppdatert. Du kan beskytte arbeids filene dine på alle iOS-, Android-og Windows 10-enhetene dine med bedrifts grad sikkerhet som er enkel å administrere.

Se denne videoen for å få en rask oversikt over Microsoft 365 for bedrifter.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 for bedrifter er ment for opptil 300 lisenser. Hvis du trenger flere lisenser, kan du se dokumentasjonen for [Microsoft 365 Enterprise](https://go.microsoft.com/fwlink/p/?linkid=860986) for å få mer informasjon. 
  
## <a name="get-microsoft-365-for-business"></a>Få Microsoft 365 for bedrifter

- Hvis du har en partner, vil de få Microsoft 365 for bedrifter: [Skaff deg microsoft 365 for bedrifter fra Microsoft partner senter](get-microsoft-365-business.md).
    
- Hvis du ikke har en partner og ønsker å få tak i Microsoft 365 for bedrifter, kan du [kjøpe den her](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-for-business"></a>Konfigurere Microsoft 365 for bedrifter

 **Oversikt over Microsoft 365 for Business Suite konfigurert**
  
Diagrammet nedenfor beskriver hvordan administratorer konfigurerer Microsoft 365 for bedrifter. Den beskriver også Fremgangs måten for å klargjøre Windows-PC-er for Microsoft 365 for bedrifter. Du kan også legge til nye enheter i administrasjons senteret for Microsoft 365 med [Windows autopilot](add-autopilot-devices-and-profile.md). Du kan bruke automatisk pilot til å konfigurere og forhånds konfigurere nye enheter, slik at de er klare til å bruke så snart en bruker logger seg på med Microsoft-365 for bedrifters legitimasjon.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

Se denne videoen for å få en oversikt over Microsoft 365 for Business-oppsett.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Hvis du synes at denne videoen er nyttig, kan du se den [fullstendige opplæringsserien for små bedrifter og de som er nybegynnere i Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: konfigurere Microsoft 365 for bedrifter (administrator)

Logg deg på [administrasjons senteret for Microsoft 365](https://portal.office.com/adminportal/home) med den globale administrator legitimasjonen, og følg Fremgangs måten nedenfor for å konfigurere Microsoft 365 for Business. 
  
1. [Forutsetninger for å beskytte data på enheter med Microsoft 365 for bedrifter](pre-requisites-for-data-protection.md)
    
    Les forutsetningene først for å sikre at enhetene dine er klare for Microsoft 365 for bedrifter.
    
2. [Bruke konfigurasjons vei viseren til å konfigurere Microsoft 365 for bedrifter](set-up.md)
    
    Hvis du **flytter permanent fra en lokal Active Directory til skyen**, kan du gå til administrasjons senteret for Microsoft 365 og bruke konfigurasjons vei viseren til å legge til brukerne manuelt, eller du kan utføre en en gangs synkronisering med Azure ad Connect. Dette kan gjøres på to måter: 
    
    - Hvis du også har en Exchange 2010-, Exchange-2013-eller Exchange 2016-server, kan du [bruke minimal hybrid til raskt å overføre Exchange-postbokser til Microsoft 365](https://docs.microsoft.com/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate). Minimums trinnene for hybrid omfatter en en gangs synkronisering av brukere til Azure AD, og e-postoverføring fra lokal til skyen. Når e-postoverføringen er fullført, deaktiveres katalog synkroniseringen automatisk når du bruker denne metoden.
    
    - Bruk vei viseren for katalog synkronisering til å synkronisere brukere til skyen. Følg Fremgangs måten i [konfigurere katalog synkronisering for Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/set-up-directory-synchronization) for å fullføre denne prosessen. Når du har synkronisert brukerne til skyen, må du deaktivere [katalog synkronisering for Microsoft 365](https://docs.microsoft.com/microsoft-365/enterprise/turn-off-directory-synchronization).
    
    Du må også gi hver bruker som er lagt til på denne måten, en lisens til Microsoft 365 for bedrifter. Du kan gjøre dette i [installasjons vei viseren](set-up.md) , eller du kan [Tilordne lisenser til brukere](../admin/manage/assign-licenses-to-users.md).
    
### <a name="2-prepare-mobile-devices"></a>2: klargjøre mobile enheter

Følg Fremgangs måten i [konfigurere mobile enheter for Microsoft 365 for Business-brukere](set-up-mobile-devices.md) for å installere Office-apper på enheter og sikre at de er beskyttet av Microsoft 365 for Business. 
  
### <a name="3-prepare-pcs"></a>3: klargjøre PC-er

Administratorer kan forhåndsvelge innstillinger for nye Windows 10-PCer ved hjelp av [Windows autopilot](add-autopilot-devices-and-profile.md). Brukere kan konfigurere sine eksisterende eller nye Windows 10-enheter ved å følge Fremgangs måten i dette emnet: [konfigurere Windows-PC-er for Microsoft 365 for bedrifter-brukere](set-up-windows-devices.md). For eksisterende enheter kan brukere **eventuelt** [flytte filer til OneDrive for Business](move-files-to-onedrive.md). De kan også bruke tredje parts verktøy til å flytte filer som er knyttet til Windows-profilen, til OneDrive.
  
Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 for bedrifter til å beskytte Windows 10-enhetene, samtidig som du fortsatt har tilgang til lokale ressurser som krever lokal godkjenning. Følg trinnene i [Aktiver domene tilknyttede Windows 10-enheter for å administreres av Microsoft 365 for Business](manage-windows-devices.md) for å konfigurere dette. Denne metoden er foretrukket, og enheter i denne tilstanden kalles **hybrid Azure ad-tilknyttede enheter**. 
  
Hvis du beholder en lokal Active Directory som inneholder enkelte lokale ressurser (for eksempel delte fil ressurser og skrivere), kan du gi **Azure ad-tilknyttede enheter** tilgang til disse ressursene ved å følge Fremgangs måten nedenfor: [få tilgang til lokale ressurser fra en Azure ad-tilkoblet enhet i Microsoft 365 for Business](access-resources.md).
  
  
## <a name="contact-support"></a>Kontakt kundestøtte

 **Hvis du må ta kontakt med kundestøtte:**
  
- Kontakt partneren din.
    
- Som en Microsoft 365 for Business-administrator har du tilgang til kunde støtte teamet vårt: ** [kontakt kunde støtte for bedrifts produkter – Hjelp for administratorer](https://docs.microsoft.com/microsoft-365/admin/contact-support-for-business-products)**
    
## <a name="see-also"></a>Se også

[Dokumentasjon og ressurser for Microsoft 365 for Business](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Administrere microsoft 365 for bedrifter](manage.md)[overføre til Microsoft 365 for Business](migrate-to-microsoft-365-business.md)

[Opplærings videoer for Microsoft 365 for bedrifter](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816) 
