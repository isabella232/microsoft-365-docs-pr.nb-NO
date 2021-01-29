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
description: Oppdag konfigurasjonstrinnene for Microsoft 365 Business Premium, inkludert å legge til et domene og brukere, konfigurere sikkerhetspolicyer og mer.
ms.openlocfilehash: e7ebe179c67077dc71ae4873b0711d0e810c701a
ms.sourcegitcommit: 1b30ac6e05906c8a014b1fed33fc71e1821f6ad2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2021
ms.locfileid: "50044734"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Konfigurere Microsoft 365 Business Premium i konfigurasjonsveiviseren

Se denne videoen for å få en oversikt over konfigurasjon av Microsoft 365 Business Premium.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a>Legge til domenet ditt, brukere og konfigurere policyer

Når du kjøper Microsoft 365 Business Premium, kan du bruke et domene du eier, eller kjøpe et under [registreringen.](sign-up.md)

- Hvis du kjøpte et nytt domene da du registrerte deg, er domenet konfigurert, og du kan flytte til Legg til brukere og [tilordne lisenser.](#add-users-and-assign-licenses)

### <a name="add-your-domain-to-personalize-sign-in"></a>Legge til domenet for å tilpasse pålogging

1. Logg på [administrasjonssenteret for Microsoft 365](https://admin.microsoft.com) ved hjelp av legitimasjonen for global administrator. 

2. Velg **Gå til konfigurasjon for** å starte veiviseren.

    ![Velg Gå til konfigurasjon.](../media/gotosetupinadmincenter.png)

3. På siden **Installer Office-apper** kan du også installere appene på din egen datamaskin.
    
4. I **trinnet Legg til** domene skriver du inn domenenavnet du vil bruke (for contoso.com).

    > [!IMPORTANT]
    > Hvis du kjøpte et domene under registreringen, ser du ikke Legg til **et domene-trinn** her. Gå til [Legg til brukere i](#add-users-and-assign-licenses) stedet.

    ![Skjermbilde av siden Tilpass påloggingen.](../media/adddomain.png)

    
4. Følg fremgangsmåten i veiviseren for å [opprette DNS-poster hos en DNS-vert for Microsoft 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) som bekrefter at du eier domenet. Hvis du kjenner domeneverten, kan du også se [vertens spesifikke instruksjoner.](https://docs.microsoft.com/office365/admin/get-help-with-domains/set-up-your-domain-host-specific-instructions)

    Hvis vertsleverandøren er GoDaddy eller [](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)en annen vert som er aktivert med domenekryssing, er prosessen enkel, og du blir automatisk bedt om å logge på og la Microsoft godkjenne på dine vegne.

    ![Velg Godkjenn på GoDaddys bekreft tilgang-side.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Legge til brukere og tilordne lisenser

Du kan legge til brukere i veiviseren, men du kan også [legge til brukere senere](add-users-m365b.md) i administrasjonssenteret. Hvis du har en lokal domenekontroller, kan du i tillegg legge til brukere [med Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

#### <a name="add-users-in-the-wizard"></a>Legge til brukere i veiviseren

Alle brukere du legger til i veiviseren, tilordnes automatisk en Lisens for Microsoft 365 Business Premium.

![Skjermbilde av siden Legg til nye brukere i veiviseren](../media/addnewuserspage.png)

1. Hvis Microsoft 365 Business Premium-abonnementet har eksisterende brukere (for eksempel hvis du brukte Azure AD Connect), får du et alternativ for å tilordne lisenser til dem nå. Gå videre og legg til lisenser for dem også.

2. Når du har lagt til brukerne, får du også et alternativ for å dele legitimasjon med de nye brukerne du har lagt til. Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.

### <a name="connect-your-domain"></a>Koble til domenet ditt

> [!NOTE]
> Hvis du valgte å bruke .onmicrosoft-domenet, eller brukte Azure AD Connect til å konfigurere brukere, vil du ikke se dette trinnet.
  
Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.
  
1. Oppsettsveiviseren oppdager vanligvis registratoren og gir deg en kobling til trinnvise instruksjoner for hvordan du oppdaterer NS-postene på nettstedet til registratoren. Hvis den ikke gjør det, [endrer du navneservere for å konfigurere Microsoft 365 med en hvilken som helst domeneregistrator.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar) 

    - Hvis du har eksisterende DNS-poster, for eksempel et eksisterende nettsted, men DNS-verten er aktivert for [domene](https://docs.microsoft.com/office365/admin/get-help-with-domains/domain-connect)connect, velger du Legg **til poster for meg.** Godta alle **standardinnstillingene på** siden Velg nettjenester, og velg  **Neste,** og velg Autoriser på siden til DNS-verten.
    - Hvis du har eksisterende DNS-poster med andre DNS-verter (ikke aktivert for domenekoblet), må du administrere dine egne DNS-poster for å sikre at de eksisterende tjenestene forblir tilkoblet. Se [grunnleggende funksjoner](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for domenet hvis du vil ha mer informasjon.

        ![Siden Aktiver poster.](../media/activaterecords.png)

2. Følg trinnene i veiviseren, og e-post og andre tjenester vil bli konfigurert for deg.

### <a name="protect-your-organization"></a>Beskytte organisasjonen 

Policyene du konfigurerte i veiviseren, brukes automatisk på en [sikkerhetsgruppe](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) kalt *Alle brukere.* Du kan også opprette flere grupper for å tilordne policyer til i administrasjonssenteret.

1. På Øk beskyttelse fra avanserte **datatrusler** anbefales det at du godtar standardverdiene for å la [Office 365 Advance Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp) skanne filer og koblinger i Office-apper.

    ![Skjermbilde av Øk beskyttelse-siden.](../media/increasetreatprotection.png)


2. Godta standardinnstillingen for å slå på Office 365 Data Loss Prevention (DLP) for å spore sensitive data i Office-apper og forhindre utilsiktet deling av disse utenfor organisasjonen, på siden Forhindre lekkasje av sensitive **data.**

3. La administrasjon av mobilapper være på, utvid innstillingene og se gjennom dem, og velg deretter Opprett policy for administrasjon av **mobilapper** på siden Beskytt data i **Office for** mobil.

    ![Skjermbilde av siden Beskytt data i Office for mobil.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Sikre PC-er med Windows 10

Velg Konfigurer til  venstre, og velg deretter Sikre **Windows 10-datamaskinene** under Pålogging og sikkerhet.  Velg **Vis for** å komme i gang. Se [sikre Windows 10-datamaskiner](secure-win-10-pcs.md) for fullstendige instruksjoner.

## <a name="deploy-office-365-client-apps"></a>Distribuere Office 365-klientapper

Hvis du velger å installere Office-apper automatisk under installasjonen, installeres appene på Windows 10-enhetene når brukerne har logget på Azure AD fra Windows-enhetene sine ved hjelp av jobblegitimasjonen.

Hvis du vil installere Office på mobile iOS- eller Android-enheter, kan du se Konfigurere mobile enheter for Brukere av [Microsoft 365 Business Premium.](set-up-mobile-devices.md)

Du kan også installere Office enkeltvis. Se [installere Office på en PC eller Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instruksjoner.

## <a name="see-also"></a>Se også

[Opplæringsvideoer for Microsoft 365 for bedrifter](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
