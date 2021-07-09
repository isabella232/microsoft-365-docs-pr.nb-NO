---
title: Kom i gang med Microsoft 365 for bedrifter
f1.keywords:
- NOCSH
ms.author: efrene
author: efrene
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
description: Lær om Microsoft 365 for bedrifter, hvordan du konfigurerer det og hvordan du klargjør brukernes enheter og PC-er for å sikre at de er beskyttet av Microsoft 365 for bedrifter.
ms.openlocfilehash: 2ab0079da7a8f30d481cdb3d3dc6d165b4a19e99
ms.sourcegitcommit: 0d1b065c94125b495e9886200f7918de3bda40b3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/08/2021
ms.locfileid: "53339294"
---
# <a name="get-started-with-microsoft-365-for-business"></a>Kom i gang med Microsoft 365 for bedrifter

## <a name="what-is-microsoft-365-for-business"></a>Hva er Microsoft 365 for bedrifter

Microsoft 365 for bedrifter er et omfattende sett med verktøy for forretningsproduktivitet og samarbeid, for eksempel Outlook, Word, Excel og andre Office produkter, som alltid er oppdatert. Du kan beskytte arbeidsfilene dine på alle iOS-, Android- og Windows 10 enheter med sikkerhet i bedriftsklasse som er enkel å administrere.

## <a name="watch-what-is-microsoft-365-business-premium"></a>Se: Hva er Microsoft 365 Business Premium

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2mhaA] 
  
Microsoft 365 for bedrifter er ment for opptil 300 lisenser. Hvis du trenger flere lisenser, kan du se dokumentasjonen for [Microsoft 365 Enterprise](../enterprise/index.yml) for å få mer informasjon. 
  
## <a name="get-microsoft-365-for-business"></a>Få Microsoft 365 for bedrifter

- Hvis du har en partner, får de tilgang Microsoft 365 for bedrifter: Få Microsoft 365 [for bedrifter fra Microsoft Partnersenter.](get-microsoft-365-business.md)
    
- Hvis du ikke har en partner og ønsker å få tilgang Microsoft 365 for bedrifter, kan du [kjøpe den her](https://www.microsoft.com/microsoft-365/business).
    
## <a name="set-up-microsoft-365-for-business"></a>Konfigurere Microsoft 365 for bedrifter

 **Oversikt over Microsoft 365 for business Suite-oppsett**
  
Diagrammet nedenfor beskriver hvordan administratorer konfigurerer Microsoft 365 for bedrifter. Den beskriver også trinnene for å klargjøre Windows PC-er for Microsoft 365 for bedrifter. Du kan også legge til nye enheter i Administrasjonssenter for Microsoft 365 med [Windows AutoPilot](add-autopilot-devices-and-profile.md). Du kan bruke AutoPilot til å konfigurere og forhåndskonfigurere nye enheter slik at de er klare til produktiv bruk så snart en bruker logger på med Microsoft 365 for bedriftslegitimasjon.
  
![A diagram that shows the setup and management flow for admins, and also for a user](../media/249f81fc-7e79-44c7-8425-3a0b7b651c3b.png)

## <a name="watch-set-up-microsoft-365-business"></a>Se: Konfigurere Microsoft 365 Business

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Hvis du synes at denne videoen er nyttig, kan du se den [fullstendige opplæringsserien for små bedrifter og de som er nybegynnere i Microsoft 365](../business-video/index.yml).

  
### <a name="1-set-up-microsoft-365-for-business-admin"></a>1: Konfigurere Microsoft 365 for bedrifter (administrator)

Logg på [Administrasjonssenter for Microsoft 365](https://admin.microsoft.com/adminportal/home) med den globale administratorlegitimasjonen, og fullfør følgende trinn for å konfigurere Microsoft 365 for bedrifter. 
  
1. [Forutsetninger for å beskytte data på enheter med Microsoft 365 for bedrifter](pre-requisites-for-data-protection.md)
    
    Les forutsetningene først for å sikre at enhetene er klare for Microsoft 365 for bedrifter.
    
2. [Bruk konfigurasjonsveiviseren til å konfigurere Microsoft 365 for bedrifter](set-up.md)
    
    Hvis du flytter permanent fra en lokal **Active Directory** til skyen , kan du gå til Administrasjonssenter for Microsoft 365 og bruke konfigurasjonsveiviseren til å legge til brukerne manuelt, eller du kan gjøre en engangssynkronisering med Azure AD Koble til. Dette kan gjøres på to måter: 
    
    - Hvis du også har en server for Exchange 2010, Exchange 2013 eller Exchange 2016, kan du bruke minimal hybrid til raskt å overføre Exchange-postbokser [til Microsoft 365](/Exchange/mailbox-migration/use-minimal-hybrid-to-quickly-migrate). De minimale hybridtrinnene omfatter en engangssynkronisering av brukere til Azure AD og e-postoverføring fra lokal til skyen. Når e-postoverføringen er fullført, deaktiveres katalogsynkroniseringen automatisk når du bruker denne metoden.
    
    - Bruk veiviseren for katalogsynkronisering til å synkronisere brukerne til skyen. Følg fremgangsmåten i [Konfigurere katalogsynkronisering for Microsoft 365](../enterprise/set-up-directory-synchronization.md) å fullføre denne prosessen. Når du har synkronisert brukerne til skyen, må du deaktivere [katalogsynkronisering for](../enterprise/turn-off-directory-synchronization.md)Microsoft 365 .
    
    Du må også gi hver bruker som ble lagt til på denne måten, en lisens Microsoft 365 for bedrifter. Du kan gjøre dette i [konfigurasjonsveiviseren,](set-up.md) eller du kan [tilordne lisenser til brukere](../admin/manage/assign-licenses-to-users.md).
    
### <a name="2-prepare-mobile-devices"></a>2: Klargjøre mobile enheter

Følg fremgangsmåten i Konfigurere mobile enheter [for Microsoft 365 for](set-up-mobile-devices.md) bedriftsbrukere til å installere Office-apper på enheter og sørge for at de er beskyttet av Microsoft 365 for bedrifter. 
  
### <a name="3-prepare-pcs"></a>3: Klargjøre PC-er

Administratorer kan forhånds velge innstillinger for nye Windows 10 PC-er ved hjelp av Windows [AutoPilot](add-autopilot-devices-and-profile.md). Brukere kan konfigurere eksisterende eller nye Windows 10-enheter ved å følge fremgangsmåten i dette emnet: Konfigurere Windows PC-er for Microsoft 365 [for bedriftsbrukere](set-up-windows-devices.md). For eksisterende enheter kan brukere **eventuelt** [flytte filer til OneDrive for Business](move-files-to-onedrive.md). De kan også bruke tredjepartsverktøy til å flytte filer som er Windows til OneDrive.
  
Hvis organisasjonen bruker Windows Server Active Directory lokalt, kan du konfigurere Microsoft 365 for bedrifter til å beskytte Windows 10-enhetene dine, samtidig som du beholder tilgang til lokale ressurser som krever lokal godkjenning. Følg fremgangsmåten i [Aktivere domenekretserte](manage-windows-devices.md) Windows 10 enheter som skal administreres av Microsoft 365 for bedrifter for å konfigurere dette. Denne metoden foretrekkes, og enheter i denne tilstanden kalles **Hybrid Azure AD-sammenføyde enheter.** 
  
Hvis du beholder en lokal Active Directory som inneholder noen lokale ressurser (for eksempel delte filressurser og skrivere), kan du gi **azure AD-sammenføyde** enheter tilgang til disse ressursene ved å følge fremgangsmåten her: Få tilgang til lokale ressurser fra en Azure AD-sammenføyd enhet i [Microsoft 365 for bedrifter](access-resources.md).
  
  
## <a name="contact-support"></a>Kontakt kundestøtte

 **Hvis du må ta kontakt med kundestøtte:**
  
- Kontakt partneren din.
    
- Som Microsoft 365 for bedriftsadministrator har du tilgang til kundestøtteteamet vårt: Kontakt kundestøtte **[for bedriftsprodukter – hjelp for administratorer](../business-video/get-help-support.md)**
    
## <a name="related-content"></a>Beslektet innhold

[Microsoft 365 for forretningsdokumentasjon og -ressurser](./index.yml) (koblingsside)\
[Administrere Microsoft 365 for bedrifter](manage.md) (artikkel)\
[Overføre til Microsoft 365 for bedrifter](migrate-to-microsoft-365-business.md) (artikkel)\
[Microsoft 365 opplæringsvideoer for bedrifter](../business-video/index.yml) (koblingsside)