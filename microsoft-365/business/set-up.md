---
title: Konfigurere Microsoft 365 Business Premium
f1.keywords:
- NOCSH
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Oppdag konfigurasjons trinnene for Microsoft 365 Business Premium, inkludert å legge til et domene og brukere, konfigurere sikkerhets policyer og mer.
ms.openlocfilehash: cc20637d7a78bd34ecb61a4ed46eb06d564d63df
ms.sourcegitcommit: 25afc0c34edc7f8a5eb389d8c701175256c58ec8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/01/2020
ms.locfileid: "47324500"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Konfigurere Microsoft 365 Business Premium i installasjons vei viseren

Se denne videoen for å få en oversikt over Microsoft 365 Business Premium-oppsett.<br><br>

## <a name="add-your-domain-users-and-set-up-policies"></a>Legge til domenet, brukere og konfigurere policyer

Når du kjøper Microsoft 365 Business Premium, kan du velge å bruke et domene som du eier, eller kjøpe et under [registreringen](sign-up.md).

- Hvis du har kjøpt et nytt domene da du registrerte deg, er domenet ditt alt konfigurert, og du kan flytte for å [legge til brukere og tilordne lisenser](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Legg til domenet ditt for å tilpasse påloggings

1. Logg deg på [administrasjons senteret for Microsoft 365](https://admin.microsoft.com) ved hjelp av den globale administrator legitimasjonen. 

2. Velg **gå til konfigurasjon** for å starte vei viseren.

    ![Velg gå til konfigurasjon.](../media/gotosetupinadmincenter.png)

3. På siden **Installer Office-apper** kan du også installere appene på din egen data maskin.
    
4. I **Legg til domene** -trinnet skriver du inn domene navnet du vil bruke (for eksempel contoso.com).

    > [!IMPORTANT]
    > Hvis du kjøpte et domene under registreringen, vil du ikke se **Legg til et domene** trinn her. Gå til [Legg til brukere](#add-users-and-assign-licenses) i stedet.

    ![Skjerm bilde av Tilpass påloggings siden.](../media/adddomain.png)

    
4. Følg trinnene i vei viseren for å [opprette DNS-poster hos en DNS-vert-leverandør for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) som bekrefter at du eier domenet. Hvis du vet verten for domenet, kan du se også de [spesifikke instruksjonene](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Hvis verts leverandøren din er GoDaddy eller en annen vert aktivert med [Domain Connect](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), blir prosessen enkelt og du blir bedt om å logge på og la Microsoft godkjenne på dine vegne.

    ![Velg Autoriser på GoDaddy Confirm Access Page.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Legge til brukere og tilordne lisenser

Du kan legge til brukere i vei viseren, men du kan også [legge til brukere senere](add-users-m365b.md) i administrasjons senteret. Hvis du har en lokal domene kontroller, kan du også legge til brukere med [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Legge til brukere i vei viseren

Alle brukere du legger til i vei viseren, får automatisk tildelt en lisens for Microsoft 365 Business Premium.

![Skjerm bilde av siden Legg til nye brukere i vei viseren](../media/addnewuserspage.png)

1. Hvis Microsoft 365 Business Premium-abonnementet har eksisterende brukere (for eksempel hvis du brukte Azure AD Connect), får du et alternativ for å tilordne lisenser til dem nå. Gå videre og legg til lisenser for dem også.

2. Når du har lagt til brukerne, får du også et alternativ for å dele legitimasjon med de nye brukerne du har lagt til. Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.

### <a name="connect-your-domain"></a>Koble til domenet ditt

> [!NOTE]
> Hvis du velger å bruke. onmicrosoft-domenet, eller du brukte Azure AD Connect til å konfigurere brukere, vil du ikke se dette trinnet.
  
Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.
  
1. Oppsettsveiviseren oppdager vanligvis registratoren og gir deg en kobling til trinnvise instruksjoner for hvordan du oppdaterer NS-postene på nettstedet til registratoren. Hvis den ikke gjør det, [endrer du navneservere for å konfigurere Microsoft 365 med alle domene registre ring](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar). 

    - Hvis du har eksisterende DNS-poster, for eksempel et eksisterende Web område, men DNS-verten er aktivert for [domene tilkobling](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), velger du **Legg til poster for meg**. Godta alle standarder på siden **Velg nettbaserte tjenester** , og velg deretter på **neste**, og velg deretter **Godkjenn** på DNS-vertens side.
    - Hvis du har eksisterende DNS-poster med andre DNS-verter (ikke aktivert for Domain Connect), bør du administrere dine egne DNS-poster for å sikre at de eksisterende tjenestene forblir tilkoblet. Se [grunnleggende om domener](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for mer informasjon.

        ![Siden Aktiver poster.](../media/activaterecords.png)

2. Følg trinnene i vei viseren, og du kan konfigurere e-post og andre tjenester for deg.

### <a name="protect-your-organization"></a>Beskytt organisasjonen 

Policyene du konfigurerer i vei viseren, brukes automatisk på en [sikkerhets gruppe](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) kalt *alle brukere*. Du kan også opprette flere grupper for å tilordne policyer til i administrasjons senteret.

1. Hvis du vil **øke beskyttelsen mot avanserte kyberterrorisme-trusler**, anbefales det at du godtar standard innstillingene for å la [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) skanne filer og koblinger i Office-apper.

    ![Skjerm bilde av siden for å øke beskyttelse.](../media/increasetreatprotection.png)


2. På siden **hindre lekkasjer av sensitive data** , godtar du standardene for å aktivere Office 365 datatap (DLP) for å spore sensitive data i Office-apper og hindre skader deling av disse utenfor organisasjonen.

3. På siden **Beskytt data på Office for mobil** kan du forlate administrasjon av mobilapp på, utvide innstillingene og se gjennom dem og deretter velge **Opprett policy for administrasjon av Mobilapper**.

    ![Skjerm bilde av Beskytt data på Office for mobil-siden.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Sikre Windows 10-PC-er

Velg **konfigurasjon** i det venstre navigasjons feltet, og velg deretter **sikre Windows 10-datamaskiner**under **pålogging og sikkerhet**. Velg **visning** for å komme i gang. Se [sikre Windows 10-datamaskiner](secure-win-10-pcs.md) for fullstendige instruksjoner.

## <a name="deploy-office-365-client-apps"></a>Distribuere Office 365-klient programmer

Hvis du velger å installere Office-apper automatisk under installasjonen, blir appene installert på Windows 10-enhetene når brukerne har logget seg på Azure AD fra Windows-enhetene sine, ved hjelp av arbeids legitimasjonen deres.

Hvis du vil installere Office på mobile iOS-eller Android-enheter, kan du se [konfigurere mobile enheter for Microsoft 365 Business Premium-brukere](set-up-mobile-devices.md).

Du kan også installere Office individuelt. Se [installere Office på en PC eller Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for å få instruksjoner.

## <a name="see-also"></a>Se også

[Opplærings videoer for Microsoft 365 for bedrifter](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
