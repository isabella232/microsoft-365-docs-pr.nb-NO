---
title: Konfigurere Microsoft 365 Business
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
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Finn ut hvordan du konfigurerer Microsoft 365 Business.
ms.openlocfilehash: c370a5b3fd735e704eea56ac1079bb2e5dad4c4b
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594273"
---
# <a name="set-up-microsoft-365-business-in-the-setup-wizard"></a>Konfigurere Microsoft 365 Business i installasjonsveiviseren

Se denne videoen for en oversikt over installasjonsprogrammet for Microsoft 365 Business.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE1FYSM] 

Hvis du synes at denne videoen er nyttig, kan du se den [fullstendige opplæringsserien for små bedrifter og de som er nybegynnere i Microsoft 365](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).

## <a name="add-your-domain-users-and-set-up-policies"></a>Legg til domenet, brukerne og konfigurer policyer

[![Etikett for å gi deg beskjed om at administrasjonssenteret endres. Du finner mer informasjon på aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Når du kjøper Microsoft 365 Business, har du muligheten til å bruke et domene du eier, eller kjøpe et under [registreringen](sign-up.md).

- Hvis du kjøpte et nytt domene da du registrerte deg, er domenet konfigurert, og du kan flytte til [Legg til brukere og tilordne lisenser](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Legg til domenet for å tilpasse påloggingen

1. Logg på [administrasjonssenteret for Microsoft 365](https://admin.microsoft.com) ved hjelp av den globale administratorlegitimasjonen. 

2. Velg **Gå til oppsett** for å starte veiviseren.

    ![Velg Gå til oppsett.](media/gotosetupinadmincenter.png)

3. På siden **Installer Office-apper** kan du eventuelt installere appene på din egen datamaskin.
    
4. Skriv **inn** domenenavnet du vil bruke (for eksempel contoso.com) i trinnet Legg til domene ( contoso.com).

    > [!IMPORTANT]
    > Hvis du kjøpte et domene under registreringen, ser du ikke **Legg til et domenetrinn** her. Gå til Legg til [brukere](#add-users-and-assign-licenses) i stedet.

    ![Skjermbilde av siden Tilpass pålogging.](media/adddomain.png)

    
4. Følg trinnene i veiviseren for å [opprette DNS-poster hos en DNS-vertsleverandør for Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) som bekrefter at du eier domenet. Hvis du kjenner domeneverten, kan du se også [de vertsspesifikke instruksjonene](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions).

    Hvis vertsleverandøren din er GoDaddy eller en annen vert som er aktivert med [domenetilkobling](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect), er prosessen enkel, og du blir automatisk bedt om å logge på og la Microsoft godkjenne på dine vegne.

    ![Velg Godkjenn på Siden Bekreft tilgang for GoDaddy.](media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Legge til brukere og tilordne lisenser

Du kan legge til brukere i veiviseren, men du kan også [legge til brukere senere](add-users-m365b.md) i administrasjonssenteret. Hvis du har en lokal domenekontroller, kan du også legge til brukere med [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

#### <a name="add-users-in-the-wizard"></a>Legge til brukere i veiviseren

Alle brukere du legger til i veiviseren, får automatisk tildelt en Microsoft 365 Business-lisens.

![Skjermbilde av siden Legg til nye brukere i veiviseren](media/addnewuserspage.png)

1. Hvis Microsoft 365 Business-abonnementet ditt har eksisterende brukere (for eksempel hvis du brukte Azure AD Connect), får du et alternativ for å tilordne lisenser til dem nå. Gå videre og legg til lisenser for dem også.

2. Når du har lagt til brukerne, får du også et alternativ for å dele legitimasjon med de nye brukerne du har lagt til. Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.

### <a name="connect-your-domain"></a>Koble til domenet ditt

> [!NOTE]
> Hvis du velger å bruke .onmicrosoft-domenet eller brukte Azure AD Connect til å konfigurere brukere, vil du ikke se dette trinnet.
  
Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.
  
1. Oppsettsveiviseren oppdager vanligvis registratoren og gir deg en kobling til trinnvise instruksjoner for hvordan du oppdaterer NS-postene på nettstedet til registratoren. Hvis den ikke gjør det, [endrer du navneservere for å konfigurere Office 365 med en domeneregistrator](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Hvis du har eksisterende DNS-poster, for eksempel et eksisterende webområde, men DNS-verten er aktivert for [domenetilkobling,](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)velger du **Legg til poster for meg**. Godta alle standardene på siden **Velg nettjenester,** og velg **Neste**, og velg **Autoriser** på DNS-vertens side.
    - Hvis du har eksisterende DNS-poster med andre DNS-verter (ikke aktivert for domenetilkobling), bør du administrere dine egne DNS-poster for å sikre at de eksisterende tjenestene forblir tilkoblet. Se [grunnleggende om domenet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) hvis du vil ha mer informasjon.

        ![Aktiver postsiden.](media/activaterecords.png)

2. Følg trinnene i veiviseren og e-post og andre tjenester vil bli satt opp for deg.

### <a name="protect-your-organization"></a>Beskytt organisasjonen 

Policyene du definerer i veiviseren, brukes automatisk på en [sikkerhetsgruppe](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) kalt *Alle brukere*. Du kan også opprette flere grupper for å tilordne policyer til i administrasjonssenteret.

1. På **Øke beskyttelsen mot avanserte cybertrusler**anbefales det at du godtar standardinnstillingene for å la [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) skanne filer og koblinger i Office-apper.

    ![Skjermbilde av øke beskyttelse-siden.](media/increasetreatprotection.png)


2. Godta standardinnstillingene for å aktivere Office 365 Data Loss Prevention (DLP) på siden **Forhindre lekkasjer av sensitive data** for å spore sensitive data i Office-apper og forhindre utilsiktet deling av disse utenfor organisasjonen.

3. På **siden Beskytt data i Office for mobil** lar du administrasjon av mobilapper være på, utvide innstillingene og se gjennom dem, og deretter velger du Opprett policy for administrasjon av **mobilapper**.

    ![Skjermbilde av Beskytt data i Office for mobilside.](media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Sikre Windows 10-PCer

Velg **Oppsett** på venstre navigasjonsenhet, og velg deretter Sikre **Windows 10-datamaskiner**under **Sing-in og sikkerhet**. Velg **Vis** for å komme i gang. Se [sikre Windows 10-datamaskinene](secure-win-10-pcs.md) for fullstendige instruksjoner.

## <a name="deploy-office-365-client-apps"></a>Distribuere Office 365-klientapper

Hvis du velger å installere Office-apper automatisk under installasjonen, installeres appene på Windows 10-enhetene når brukerne har logget på Azure AD fra Windows-enhetene sine ved hjelp av arbeidslegitimasjonen.

Hvis du vil installere Office på mobile iOS- eller Android-enheter, kan du se [Konfigurere mobile enheter for Brukere av Microsoft 365 Business](set-up-mobile-devices.md).

Du kan også installere Office individuelt. Se [installere Office på en PC eller Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc4716658) for instruksjoner.

## <a name="see-also"></a>Se også

[Opplæringsvideoer for Microsoft 365-bedrifter](https://support.office.com/article/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
