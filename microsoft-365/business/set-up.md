---
title: Konfigurere Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
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
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Lær hvordan du konfigurerer Microsoft 365 Business.
ms.openlocfilehash: cd59570cbcb9b027780e160117b44be88770d6b9
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575552"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Konfigurere Microsoft 365 Business i installasjonsveiviseren

## <a name="add-your-domain-users-and-set-up-policies"></a>Legg til domene, brukere og Konfigurer policyer

[![Label å fortelle deg at Administrasjonssenteret er i endring, og du kan finne mer informasjon på aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Når du kjøper Microsoft 365 Business, har du muligheten til å bruke et domene du eier, eller kjøpe et under [registreringen](sign-up.md).

- Hvis du kjøpte et nytt domene da du registrerte deg, er domenet ditt konfigurert, og du kan gå videre til å [legge til brukere og tilordne lisenser](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Legge til domenet for å tilpasse påloggingen

1. Logg på [administrasjonssenteret for Microsoft 365](https://admin.microsoft.com) ved hjelp av legitimasjonen for global administrator. 

2. Velg **Legg til et domene** eller **Legg til brukere** for å starte veiviseren.
    > [!IMPORTANT]
    > Hvis du har kjøpt et domene under registreringen, vil du ikke se **Legg til et domene** trinn her. Gå til [Legg til brukere](#add-users-and-assign-licenses) i stedet.

    ![Velg gå til oppsett.](media/gotosetupinadmincenter.png)
    
3. I veiviseren skriver du inn domenenavnet du vil bruke (som contoso.com).


    ![Skjermbilde av Tilpass påloggingssiden.](media/personalizesignin.png)

    
4. Følg trinnene i veiviseren for å [opprette DNS-poster i en hvilken som helst DNS-webvert for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) som bekrefter at du eier domenet. Hvis du kjenner domeneverten, kan du også se de [spesifikke instruksjonene for verten](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Hvis vertsleverandøren er GoDaddy, eller en annen vert som er aktivert med [domene tilkobling](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), er prosessen enkel, og du blir automatisk bedt om å logge på og la Microsoft godkjenne på dine vegne:

    ![På GoDaddy Bekreft tilgang-siden velger du Godkjenn.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Legge til brukere og tilordne lisenser

Du kan legge til brukere i veiviseren, men du kan også [legge til brukere senere](add-users-m365b.md) i administrasjonssenteret. I tillegg, hvis du har en lokal domenekontroller, kan du legge til brukere med [Azure ad-tilkobling](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Legg til brukere i veiviseren

Alle brukere du legger til i veiviseren, får automatisk tilordnet en Microsoft 365 business-lisens.

![Skjermbilde av siden Legg til nye brukere i veiviseren](media/addnewuserspage.png)

1. Hvis Microsoft 365 Business-abonnementet har eksisterende brukere (for eksempel hvis du brukte Azure AD-tilkobling), får du muligheten til å tilordne lisenser til dem nå. Gå videre og legg til lisenser for dem også.

2. Når du har lagt til brukerne, vil du også få mulighet til å dele legitimasjonen med de nye brukerne du la til. Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.

3. På Opprett team for organisasjonen kan du velge å legge til team og legge til brukere i dem. Du kan også gjøre dette senere. Hvis du vil ha mer informasjon, kan du se [opprette et team på hele firmaet](https://support.office.com/article/037bb27a-bcc9-48fe-8d72-44d9482420a3).

4. Hopp over overføring av e-postmeldinger, og velg **Neste** på **Overfør e-postmeldinger**-siden. 

    Hvis du flytter fra en annen e-postleverandøren og vil kopiere dataene senere, kan du [overføre e-post og kontakter til Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).


### <a name="connect-your-domain"></a>Koble til domenet ditt

> [!NOTE]
> Hvis du velger å bruke. onmicrosoft-domenet, eller brukte Azure AD Connect til å konfigurere brukere, vil du ikke se dette trinnet.
  
Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.
  
1. Oppsettsveiviseren oppdager vanligvis registratoren og gir deg en kobling til trinnvise instruksjoner for hvordan du oppdaterer NS-postene på nettstedet til registratoren. Hvis den ikke gjør det, [endrer du navneservere for å konfigurere Office 365 med en hvilken som helst domeneregistratoren](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Hvis du har eksisterende DNS-poster, for eksempel et eksisterende webområde, men DNS-verten er aktivert for [domene tilkobling](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), velger **du Legg til oppføringer for meg**. Godta alle standardene på siden **Velg dine elektroniske tjenester** , velg **neste**, og velg **Godkjenn** på DNS-vertens side.
    - Hvis du har eksisterende DNS-poster med andre DNS-verter (ikke aktivert for domene tilkobling), vil du administrere dine egne DNS-poster for å sikre at de eksisterende tjenestene forblir tilkoblet. Se [grunnleggende om domenet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for mer info.

        ![Koble domenet siden med jeg skal administrere mine egne DNS-poster.](media/connectyourdomainpage.png)

2. Følg trinnene i veiviseren, og e-post og andre tjenester vil bli satt opp for deg.

### <a name="protect-data-and-devices"></a>Beskytt data og enheter 

Policyene du definerer i veiviseren, brukes automatisk på en [sikkerhetsgruppe](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) som kalles *alle brukere*. Du kan også opprette flere grupper for å tilordne policyer til i administrasjonssenteret.

1. På **Beskytt arbeidet filer på mobile enheter** alternativet **Beskytt arbeidsfiler når enheter er tapt eller stjålet** er valgt som standard. Du har muligheten til å aktivere **administrere hvordan brukere får tilgang til Office-filer på mobile enheter**, og dette anbefales.

    ![Skjermene av beskytte arbeide fil-størrelse opp på transportabel anordninger side.](media/protectworkfilesondevices.png)

     - Utfolde **beskytte arbeide fil-størrelse når anordninger er bortkommet eller stjålet** å utfoldelse [uteblivelsen verdier](protect-work-files-on-lost-or-stolen-device.md):

        ![Skjermbilde av standardverdier for beskyttelse av filer på tapte enheter.](media/protectworkfilesondevicesdefault.png)

    - Velg **Administrer hvordan brukere får tilgang til Office-filer på mobile enheter** , og Utvid dem for å vise [standardverdiene](manage-user-access-on-mobile-devices.md). Vi anbefaler at du godtar standardverdiene under installasjonen for å opprette programpolicyer for Android, iOS og Windows 10 som gjelder for alle brukere. Du kan opprette flere policyer når konfigurasjonen er fullført.

        ![Skjermbilde av beskyttelsesinnstillinger for Office-filer på mobilenheter.](media/useraccessonmobile.png)

2. Det siste trinnet på beskyttelse av data og enheter gjør det mulig å konfigurere policyer for å sikre Windows 10-enheter. Disse innstillingene brukes automatisk når en brukers Windows 10 kobler til organisasjonen. Du kan utvide **sikre Windows 10-enheter** for å se og endre [standardverdiene](secure-windows-10-devices.md).
3. Du kan også velge å [installere Office](install-office-on-windows-10-during-setup.md) på Windows 10-enheter automatisk.

    ![Skjermbilde av angi konfigurasjonssiden for Windows 10-enheten.](media/setwin10config.png)


## <a name="deploy-office-365-client-apps"></a>Distribuere klientprogrammer for Office 365

Hvis du velger å installere Office-apper automatisk i løpet av oppsettet, installeres appene på Windows 10-enhetene når brukerne har logget på Azure AD fra Windows-enhetene sine med arbeids legitimasjonen sin.
Hvis du vil installere Office på mobile iOS-eller Android-enheter, kan du se [konfigurere mobile enheter for Microsoft 365 Business-brukere](set-up-mobile-devices.md).

Du kan også installere Office individuelt. Se [installere Office på en PC eller Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instruksjoner.
