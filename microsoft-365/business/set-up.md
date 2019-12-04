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
- TRN_SMB
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Lær hvordan du konfigurerer Microsoft 365 Business.
ms.openlocfilehash: 0001c2b9962f6cce0be1f77cbf427c68f9ee3249
ms.sourcegitcommit: c5ca71d6feb0f033b50ccd4de816fd59b0925007
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2019
ms.locfileid: "39831307"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Konfigurere Microsoft 365 Business i installasjonsveiviseren

Se denne videoen for en oversikt over Microsoft 365 Business-oppsett.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Hvis du fant denne videoen nyttig, sjekk ut [komplett trening serien for små bedrifter og de som er nye til Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

## <a name="add-your-domain-users-and-set-up-policies"></a>Legg til domene, brukere og Konfigurer policyer

[![Etikett for å gi deg beskjed om at administrasjonssenteret endres. Du finner mer informasjon på aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Når du kjøper Microsoft 365 Business, har du muligheten til å bruke et domene du eier, eller kjøpe et under [registreringen](sign-up.md).

- Hvis du kjøpte et nytt domene da du registrerte deg, er domenet ditt konfigurert, og du kan gå videre til å [legge til brukere og tilordne lisenser](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Legge til domenet for å tilpasse påloggingen

1. Logg på [administrasjonssenteret for Microsoft 365](https://admin.microsoft.com) ved hjelp av legitimasjonen for global administrator. 

2. Velg **gå til oppsett** for å starte veiviseren.

    ![Velg gå til oppsett.](media/gotosetupinadmincenter.png)

3. På siden **Installer Office-apper** kan du velge om du vil installere appene på din egen datamaskin.
    
4. I **Legg til domene** -trinnet angir du domenenavnet du vil bruke (for eksempel contoso.com).

    > [!IMPORTANT]
    > Hvis du har kjøpt et domene under registreringen, vil du ikke se **Legg til et domene** trinn her. Gå til [Legg til brukere](#add-users-and-assign-licenses) i stedet.

    ![Skjermbilde av Tilpass påloggingssiden.](media/adddomain.png)

    
4. Følg trinnene i veiviseren for å [opprette DNS-poster i en hvilken som helst DNS-webvert for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) som bekrefter at du eier domenet. Hvis du kjenner domeneverten, kan du også se de [spesifikke instruksjonene for verten](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Hvis vertsleverandøren er GoDaddy eller en annen vert som er aktivert med [domene tilkobling](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), er prosessen enkel, og du blir automatisk bedt om å logge på og la Microsoft godkjenne på dine vegne.

    ![På GoDaddy Bekreft tilgang-siden velger du Godkjenn.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Legge til brukere og tilordne lisenser

Du kan legge til brukere i veiviseren, men du kan også [legge til brukere senere](add-users-m365b.md) i administrasjonssenteret. I tillegg, hvis du har en lokal domenekontroller, kan du legge til brukere med [Azure ad-tilkobling](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Legg til brukere i veiviseren

Alle brukere du legger til i veiviseren, får automatisk tilordnet en Microsoft 365 business-lisens.

![Skjermbilde av siden Legg til nye brukere i veiviseren](media/addnewuserspage.png)

1. Hvis Microsoft 365 Business-abonnementet har eksisterende brukere (for eksempel hvis du brukte Azure AD-tilkobling), får du muligheten til å tilordne lisenser til dem nå. Gå videre og legg til lisenser for dem også.

2. Når du har lagt til brukerne, får du også mulighet til å dele legitimasjon med de nye brukerne du har lagt til. Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.

### <a name="connect-your-domain"></a>Koble til domenet ditt

> [!NOTE]
> Hvis du velger å bruke. onmicrosoft-domenet, eller brukte Azure AD Connect til å konfigurere brukere, vil du ikke se dette trinnet.
  
Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.
  
1. Oppsettsveiviseren oppdager vanligvis registratoren og gir deg en kobling til trinnvise instruksjoner for hvordan du oppdaterer NS-postene på nettstedet til registratoren. Hvis den ikke gjør det, [endrer du navneservere for å konfigurere Office 365 med en hvilken som helst domeneregistratoren](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Hvis du har eksisterende DNS-poster, for eksempel et eksisterende webområde, men DNS-verten er aktivert for [domene tilkobling](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), velger **du Legg til oppføringer for meg**. Godta alle standardene på siden **Velg dine elektroniske tjenester** , velg **neste**, og velg **Godkjenn** på DNS-vertens side.
    - Hvis du har eksisterende DNS-poster med andre DNS-verter (ikke aktivert for domene tilkobling), bør du administrere dine egne DNS-poster for å sikre at de eksisterende tjenestene forblir tilkoblet. Se [grunnleggende om domenet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for mer info.

        ![Siden for å aktivere poster.](media/activaterecords.png)

2. Følg trinnene i veiviseren, og e-post og andre tjenester vil bli satt opp for deg.

### <a name="protect-your-organization"></a>Beskytt organisasjonen din 

Policyene du definerer i veiviseren, brukes automatisk på en [sikkerhetsgruppe](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) som kalles *alle brukere*. Du kan også opprette flere grupper for å tilordne policyer til i administrasjonssenteret.

1. På **økningen beskyttelse mot avanserte Cyber trusler**, anbefales det at du godtar standardinnstillingene for å la [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) skanne filer og koblinger i Office-programmer.

    ![Skjermene av forhøye sikringen side.](media/increasetreatprotection.png)


2. På **hindre lekkasjer av sensitive data** siden, godta standardinnstillingene for å slå på Office 365 data tap PREVENTION (DLP) til å spore sensitive data i Office-programmer og hindre utilsiktet deling av disse utenfor organisasjonen.

3. På siden **Beskytt data i Office for mobil** lar du administrasjon av Mobilapper være aktivert, utvider innstillingene og går gjennom dem, og deretter velger du **Opprett administrasjonspolicy for Mobilapper**.

    ![Skjermene av beskytte data inne kontor for Transportabel side.](media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Sikre Windows 10-PCer

Velg **Oppsett** i venstre navigasjonssystem, og velg deretter **sikre Windows 10-maskinene dine**under **Sing-in og sikkerhet**. Velg **Vis** for å komme i gang. Se [sikre Windows 10-datamaskiner](secure-win-10-pcs.md) for fullstendige instruksjoner.

## <a name="deploy-office-365-client-apps"></a>Distribuere klientprogrammer for Office 365

Hvis du velger å installere Office-programmer automatisk under installasjonen, vil appene installeres på Windows 10-enhetene når brukerne har logget på Azure AD fra Windows-enhetene sine, ved hjelp av arbeids legitimasjonen deres.

Hvis du vil installere Office på mobile iOS-eller Android-enheter, kan du se [konfigurere mobile enheter for Microsoft 365 Business-brukere](set-up-mobile-devices.md).

Du kan også installere Office individuelt. Se [installere Office på en PC eller Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instruksjoner.

## <a name="see-also"></a>See al1so

[Microsoft 365 Business opplæring videoer](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
