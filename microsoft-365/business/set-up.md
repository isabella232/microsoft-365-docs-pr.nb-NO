---
title: Konfigurere Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
f1_keywords:
- O365E_M365SetupBanner
- BCS365_M365SetupBanner
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Lær hvordan du konfigurerer Microsoft 365 Business.
ms.openlocfilehash: f3a9ad62f5ec8779296e800b9ecc8d6181d7aff7
ms.sourcegitcommit: f420a5cdedf3ec2babc6d8ad7e7c79da0b08e115
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/13/2019
ms.locfileid: "33966982"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Definere Microsoft 365 Business i installasjonsveiviseren for

## <a name="add-your-domain-users-and-set-up-policies"></a>Legge til domenet, brukere, og konfigurere policyer

![Banner som peker til https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Når du kjøper Microsoft 365 Business, har du muligheten til å bruke et domene du eier, eller kjøpe en i løpet av [registreringen](sign-up.md).

- Hvis du har kjøpt et nytt domene når du registrerte deg, domenet er alle satt opp, og du kan flytte for å [legge til brukere og tilordne lisenser](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Legge til domenet for å tilpasse pålogging

1. Logg på [administrasjonssenteret for Microsoft 365](https://admin.microsoft.com) ved hjelp av global admin-rettigheter. 

2. Velg **Legg til et domene** eller **legge til brukere** for å starte veiviseren.
    > [!IMPORTANT]
    > Hvis du har kjøpt et domene under registreringen, vil du ikke se **legge til et domene** trinn her. Gå til [Legg til brukere](#add-users-and-assign-licenses) i stedet.

    ![Velg Legg til et domene.](media/addadomainadmincenter.png)
    
3. I veiviseren angir du navnet på domenet du vil bruke (for eksempel contoso.com).


    ![Skjermbilde av Tilpass på siden.](media/personalizesignin.png)

    
4. Følg trinnene i veiviseren til å [opprette DNS-poster på alle DNS-vertsleverandøren for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) , som bekrefter at du eier domenet. Hvis du kjenner ditt domene host, se også [vert for spesifikke instruksjoner](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Hvis din vertsleverandøren er GoDaddy, prosessen er enkelt, og du blir automatisk bedt om å logge på og la Microsoft godkjenne på dine vegne:

    ![Velg Godkjenn på GoDaddy bekrefte tilgang-siden.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Legge til brukere og tilordne lisenser

Du kan legge til brukere i veiviseren, men du kan også [legge til senere brukere](add-users-m365b.md) i administrasjonssenteret. Hvis du har en lokal domenekontroller, kan du i tillegg legge til brukere med [Azure AD-tilkobling](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Legge til brukere i veiviseren

Eventuelle brukere du legger til i veiviseren Hent automatisk tilordnet en lisens for Microsoft 365 Business.

![Skjermbilde av siden Legg til nye brukere i veiviseren](media/addnewuserspage.png)

1. Hvis abonnementet på Microsoft 365 Business har eksisterende brukere (for eksempel, hvis du brukte Azure AD-tilkobling), får du et alternativ for å tilordne lisenser til dem nå. Gå videre og legg til lisenser for dem også.

3. Når du har lagt til brukerne, får du også muligheten til å dele legitimasjon med de nye brukerne du har lagt til. Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.

4. Hopp over overføring av e-postmeldinger, og velg **Neste** på **Overfør e-postmeldinger**-siden. 

    Hvis du flytter fra en annen leverandør av e-post og vil kopiere dataene senere, kan du [Overfør e-post og kontakter til Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).


### <a name="connect-your-domain"></a>Koble til domenet ditt

> [!NOTE]
> Hvis du velger å bruke .onmicrosoft-domene, eller brukt Azure AD-tilkobling til å definere brukere, vil du ikke se dette trinnet.
  
Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.
  
1. Oppsettsveiviseren oppdager vanligvis registratoren og gir deg en kobling til trinnvise instruksjoner for hvordan du oppdaterer NS-postene på nettstedet til registratoren. Hvis ikke, [Endre nameservers for å konfigurere Office 365 med en hvilken som helst domeneregistrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Hvis du har eksisterende DNS-poster, for eksempel et eksisterende webområde, vil du håndtere dine egne DNS-poster for å kontrollere eksisterende tjenester forbli tilkoblet. Se [Grunnleggende om domenet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for mer informasjon.

        ![Koble ditt domene-siden med jeg skal behandle mine egne DNS-poster.](media/connectyourdomainpage.png)

2. Følg trinnene i veiviseren, og e-post og andre tjenester vil bli satt opp for deg.

### <a name="set-up-security-policies-and-device-configurations"></a>Konfigurere sikkerhetspolicyer og enheten konfigurasjoner 

Policyer som er definert i veiviseren brukes automatisk på en [sikkerhetsgruppe](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) kalt *Alle brukere*. Du kan også opprette flere grupper du tilordner policyer til i administrasjonssenteret.

1. Du **beskytte filene arbeid på mobile enheter** alternativet er **Beskytt arbeidsfiler når enhetene mistes eller stjeles** valgt som standard. Du har et alternativ for å aktivere **styre hvordan brukere får tilgang til Office-filer på mobile enheter**, og dette anbefales.

    ![Skjermbilde av beskytte arbeidsfiler på mobile enheter-siden.](media/protectworkfilesondevices.png)

     - Utvid **Beskytt arbeidsfiler når enhetene mistes eller blir stjålet** for å vise [standardverdier](protect-work-files-on-lost-or-stolen-device.md):

        ![Skjermbilde av standardverdier for å beskytte filer på tapt enheter.](media/protectworkfilesondevicesdefault.png)

    - Velg **Behandle hvordan brukere får tilgang til Office-filer på mobile enheter** , og utvid den for å vise [standardverdier](manage-user-access-on-mobile-devices.md). Vi anbefaler at du godta standardverdiene under opprette programpolicyer for Android, iOS og 10 for Windows-installasjonen som gjelder for alle brukere. Du kan opprette flere policyer når konfigurasjonen er fullført.

        ![Skjermbilde av beskyttelsesinnstillingene for Office-filer på mobile.](media/useraccessonmobile.png)

2. Det siste trinnet på beskytte data og enheter, kan du definere policyer for å sikre Windows 10 enheter. Disse innstillingene brukes automatisk når en bruker Windows 10 kobler seg til organisasjonen. Du kan utvide **sikre Windows 10 enheter** for å vise og endre [standardverdiene](secure-windows-10-devices.md).
3. Du kan også velge å [automatisk installere Office](install-office-on-windows-10-during-setup.md) på Windows 10 enheter.

    ![Skjermbilde av satt Windows 10 konfigurasjonssiden for enheten.](media/setwin10config.png)



## <a name="deploy-office-365-client-apps"></a>Distribuere Office 365-klientprogrammer

Hvis du velger å installere Office-programmer i automatisk under settet opp, installerer apps på Windows 10-enheter når brukerne har logget på Azure AD fra deres Windows-enheter med legitimasjonen arbeid.
Hvis du vil installere Office på mobile iOS eller Android enheter, kan du se [definere mobile enheter for forretningsbrukere som Microsoft 365](set-up-mobile-devices.md).

Du kan også installere Office individuelt. Se [installere Office på en PC eller Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for å få instruksjoner.
