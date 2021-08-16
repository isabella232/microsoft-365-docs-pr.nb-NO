---
title: Konfigurere Microsoft 365 Business Premium
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
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
ms.openlocfilehash: 8158e911a8520c07cf5f85fea8b64d65820d603d7f9f49938849ff2df6fc45ed
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53882013"
---
# <a name="set-up-microsoft-365-business-premium-in-the-setup-wizard"></a>Konfigurere Microsoft 365 Business Premium i konfigurasjonsveiviseren

## <a name="watch-overview-of-microsoft-365-setup"></a>Se: Oversikt over Microsoft 365 oppsett

Se denne videoen for en oversikt over Microsoft 365 Business Premium oppsett.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4jZwg] 

## <a name="add-your-domain-users-and-set-up-policies"></a>Legge til domenet, brukerne og konfigurere policyer

Når du kjøper Microsoft 365 Business Premium, har du muligheten til å bruke et domene du eier, eller kjøpe et under [registreringen.](sign-up.md)

- Hvis du kjøpte et nytt domene da du registrerte deg, er domenet konfigurert, og du kan flytte til Legg til brukere [og tilordne lisenser](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Legge til domenet for å tilpasse påloggingen

1. Logg på [Administrasjonssenter for Microsoft 365](https://admin.microsoft.com) ved hjelp av den globale administratorlegitimasjonen. 

2. Velg **Gå til konfigurasjon for** å starte veiviseren.

    ![Velg Gå til konfigurasjon.](../media/gotosetupinadmincenter.png)

3. På siden **Installer Office apper** kan du eventuelt installere appene på din egen datamaskin.
    
4. Skriv inn **domenenavnet** du vil bruke (for eksempel contoso.com) i trinnet Legg til domene.

    > [!IMPORTANT]
    > Hvis du kjøpte et domene under registreringen, vil du ikke se Legge **til et domenetrinn** her. Gå til [Legg til brukere i](#add-users-and-assign-licenses) stedet.

    ![Skjermbilde av siden Tilpass påloggingen.](../media/adddomain.png)

    
4. Følg trinnene i veiviseren for å opprette DNS-poster hos en [DNS-vertsleverandør for](/office365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider) Microsoft 365 som bekrefter at du eier domenet. Hvis du kjenner domeneverten, kan du se også [Legge til et domene i Microsoft 365](/microsoft-365/admin/setup/add-domain).

    Hvis vertsleverandøren din er GoDaddy [](/office365/admin/get-help-with-domains/domain-connect)eller en annen vert aktivert med domenetilkryssing, er prosessen enkel, og du blir automatisk bedt om å logge på og la Microsoft godkjenne på dine vegne.

    ![Velg Godkjenn på Siden Bekreft tilgang for GoDaddy.](../media/godaddyauth.png)

### <a name="add-users-and-assign-licenses"></a>Legge til brukere og tilordne lisenser

Du kan legge til brukere i veiviseren, men du kan også [legge til brukere senere](../admin/add-users/add-users.md) i administrasjonssenteret. Hvis du har en lokal domenekontroller, kan du i tillegg legge til brukere med [Azure AD Koble til.](/azure/active-directory/hybrid/how-to-connect-install-express)

#### <a name="add-users-in-the-wizard"></a>Legge til brukere i veiviseren

Alle brukere du legger til i veiviseren, får automatisk tilordnet en Microsoft 365 Business Premium lisens.

![Skjermbilde av siden Legg til nye brukere i veiviseren](../media/addnewuserspage.png)

1. Hvis abonnementet Microsoft 365 Business Premium eksisterende brukere (for eksempel hvis du brukte Azure AD Koble til), får du et alternativ for å tilordne lisenser til dem nå. Gå videre og legg til lisenser for dem også.

2. Når du har lagt til brukerne, får du også et alternativ for å dele legitimasjon med de nye brukerne du har lagt til. Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.

### <a name="connect-your-domain"></a>Koble til domenet ditt

> [!NOTE]
> Hvis du valgte å bruke .onmicrosoft-domenet eller brukte Azure AD Koble til å konfigurere brukere, vil du ikke se dette trinnet.
  
Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.
  
1. Oppsettsveiviseren oppdager vanligvis registratoren og gir deg en kobling til trinnvise instruksjoner for hvordan du oppdaterer NS-postene på nettstedet til registratoren. Hvis den ikke gjør det, [endrer du navneservere for å Microsoft 365 med en hvilken som helst domeneregistrator.](../admin/get-help-with-domains/change-nameservers-at-any-domain-registrar.md) 

    - Hvis du har eksisterende DNS-poster, for eksempel et eksisterende nettsted, men DNS-verten er aktivert for [domene-tilkobling,](/office365/admin/get-help-with-domains/domain-connect)velger du Legg til **poster for meg**. Godta alle **standardene** på siden Velg **nettbaserte** tjenester, og velg **Neste**, og velg Godkjenn på dns-vertens side.
    - Hvis du har eksisterende DNS-poster med andre DNS-verter (ikke aktivert for domenekoblet), bør du administrere dine egne DNS-poster for å sikre at de eksisterende tjenestene forblir tilkoblet. Se [grunnleggende om domener](/office365/admin/get-help-with-domains/dns-basics) hvis du vil ha mer informasjon.

        ![Aktiver poster-siden.](../media/activaterecords.png)

2. Følg trinnene i veiviseren, og e-post og andre tjenester vil bli konfigurert for deg.

### <a name="protect-your-organization"></a>Beskytt organisasjonen 

Policyene du konfigurerer i veiviseren, brukes automatisk på en [sikkerhetsgruppe](/office365/admin/create-groups/compare-groups#security-groups) kalt *Alle brukere*. Du kan også opprette flere grupper som du kan tilordne policyer til i administrasjonssenteret.

1. På Øk beskyttelse mot avanserte **cybertrusler** anbefales det at du godtar standardinnstillingene for å la Office 365 [Advance Threat Protection](../security/office-365-security/defender-for-office-365.md) skanne filer og koblinger i Office apper.

    ![Skjermbilde av Siden Øk beskyttelse.](../media/increasetreatprotection.png)


2. På siden Forhindre **lekkasjer** av sensitive data godtar du standardinnstillingene for å aktivere Office 365 Data loss Prevention (DLP) for å spore sensitive data i Office-apper og hindre utilsiktet deling av disse utenfor organisasjonen.

3. På siden **Beskytt data i Office for** mobil lar du administrasjon av mobilapper være på, utvider innstillingene og ser gjennom dem, og velger deretter Opprett policy for administrasjon av **mobilapper**.

    ![Skjermbilde av Beskytt data i Office for mobilsiden.](../media/protectdatainmobile.png)


## <a name="secure-windows-10-pcs"></a>Sikre Windows 10 PC-er

Velg Oppsett til  venstre, og **velg** deretter Sikre datamaskinene Windows 10 dine under Pålogging **og sikkerhet**. Velg **Vis for** å komme i gang. Se [sikre datamaskinene Windows 10 for](secure-win-10-pcs.md) fullstendige instruksjoner.

## <a name="deploy-office-365-client-apps"></a>Distribuere Office 365 klientapper

Hvis du velger å installere Office-apper automatisk under installasjonen, installeres appene på Windows 10-enhetene når brukerne har logget på Azure AD fra Windows-enhetene sine ved hjelp av jobblegitimasjonen.

Hvis du vil Office på mobile iOS- eller [Android-enheter,](set-up-mobile-devices.md)kan du se Konfigurere mobile enheter for Microsoft 365 Business Premium brukere .

Du kan også installere Office enkeltvis. Se [Installere Office på en PC eller Mac](https://support.microsoft.com/office/4414eaaf-0478-48be-9c42-23adc4716658) for instruksjoner.

## <a name="related-content"></a>Beslektet innhold

[Microsoft 365 opplæringsvideoer for bedrifter](../business-video/index.yml) (koblingsside)
