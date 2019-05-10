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
ms.openlocfilehash: e635b828609fc47cd8b92bb179a25bcc43cb0a1a
ms.sourcegitcommit: db1dfb2df2c2f7beced3b57bc772d106c189e88a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/07/2019
ms.locfileid: "33660853"
---
# <a name="set-up-microsoft-365-business"></a>Konfigurere Microsoft 365 Business

Før du begynner, kan du se [Få Microsoft 365 Business](get-microsoft-365-business.md) for registrering detaljene.

Se en [kort video om hvordan du konfigurerer Microsoft 365 Business](https://support.office.com/article/38003e30-9d10-44cf-b596-f1b5f662bfa1) ved hjelp av Sett opp veiviseren, og når du ikke har en lokale Active Directory
  

## <a name="overview"></a>Oversikt

Det meste av den er satt opp trinnene kan gjøres i installasjonsveiviseren, men de andre alternativene er også oppført.

1. [Legg til domenet ditt](#add-your-domain-to-personalize-sign-in) (Hvis du kjøpte domenet ditt ved å [registrere deg](sign-up.md), dette trinnet er allerede har gjort.)
2. Legg til brukere. Du kan gjøre dette på en av tre måter:
    - I [installasjonsveiviseren](#add-users-in-the-wizard).
    - Bruk katalogsynkronisering for å [legge til brukere ved hjelp av Azure AD-tilkobling](#add-users-by-using-azure-ad-connect) Hvis du har en lokale Active directory.
    - Du kan også [legge til senere brukere](add-users-m365b.md) i administrasjonssenteret.
3. Definere retningslinjer for sikkerhet og konfigurere enheter. Du kan gjøre dette på en av tre måter:
    - I [installasjonsveiviseren](#set-up-policies-in-the-wizard).  
    - [Administrasjonssenteret](#modify-or-add-policies-in-the-admin-center).
    - [Intune administrasjonssenteret](https://docs.microsoft.com/intune/what-is-device-management).
4. Definer og administrer Windows 10 enheter.

    Når du slår sammen en enhet for WIndows 10 Azure AD, får alle policyene brukes på den.
    - Sette opp Windows 10 enheten konfigurasjoner i [installasjonsveiviseren](#set-up-policies-in-the-wizard).
    - Bli med i en [ny enhet for Windows 10](set-up-windows-devices.md#for-a-brand-new-or-newly-upgraded-windows-10-pro-device) Azure AD.
    - Koble en [eksisterende Windows-10-enhet](set-up-windows-devices.md#for-a-device-already-set-up-and-running-windows-10-pro) til Azure AD.
1. Installer Office 365 Business.
    - Du kan installere Office automatisk i Windows-enheter ved hjelp av [installasjonsveiviseren](#set-up-policies-in-the-wizard).
    - Automatisk [installerer Office](auto-install-or-uninstall-office.md) fra administrasjonssenteret.
    - La brukere [installere Office-programmer](https://docs.microsoft.com/office365/admin/setup/install-applications) for Windows og enheter.
     
1. Angi ekstra sikkerhet.
    - Veiviseren legger til policyer for å sikre dine enheter, men du kan også dra nytte av [ytterligere](#additional-security-settings) sikkerhetsfunksjoner til bidrar til å sikre dine data, kontoer og e-post. 

## <a name="add-your-domain-users-and-set-up-policies"></a>Legge til domenet, brukere og definere policyer

![Banner som peker til https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Når du kjøper Microsoft 365 Business, har du muligheten til å bruke et domene du eier, eller kjøpe en i løpet av [registreringen](sign-up.md).

- Hvis du har kjøpt et nytt domene når du registrerte deg, domenet er alle satt opp, og du kan flytte for å [legge til brukere og tilordne lisenser](#add-users-and-assign-licenses).

### <a name="add-your-domain-to-personalize-sign-in"></a>Legge til domenet for å tilpasse pålogging

1. Logg på [administrasjonssenteret for Microsoft 365](https://admin.microsoft.com) ved hjelp av global admin-rettigheter. 

2. Velg **Legg til et domene** for å starte veiviseren.

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
Hvis du har en lokal domenekontroller, og bruker Active Directory, kan du se [hvordan ddd brukere ved hjelp av Azure AD-tilkobling](#add-users-by-using-azure-ad-connect).

![Skjermbilde av siden Legg til nye brukere i veiviseren](media/addnewuserspage.png)

1. Hvis ditt Microsoft 365 Business-abonnement har eksisterende brukere (for eksempel hvis du brukte Azure AD Connect), får du muligheten til å tildele lisenser til dem nå. Gå videre og legg til lisenser for dem også.

3. Når du har lagt til brukerne, får du også muligheten til å dele legitimasjon med de nye brukerne du har lagt til. Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.

4. Hopp over overføring av e-postmeldinger, og velg **Neste** på **Overfør e-postmeldinger**-siden. 

    Hvis du flytter fra en annen leverandør av e-post og vil kopiere dataene senere, kan du [Overfør e-post og kontakter til Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).

#### <a name="add-users-by-using-azure-ad-connect"></a>Legge til brukere ved hjelp av Azure AD-tilkobling

 Hvis du har en lokal domenekontroller med Active Directory, synkroniserer du brukerne med Microsoft 365 Business ved hjelp av [Azure AD-tilkobling](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express). Fullfør dette før du starter veiviseren. Du kan laste den ned i administrasjonssenteret:

- Gå til **brukere** \> **aktive brukere**, velg ellipser øverst på siden, og velg deretter **katalogsynkronisering** for å laste ned Azure AD-tilkobling.

    ![Velg ellipser > Directory snchronization på aktive brukere-siden.](media/setupdirsync.png)

    > [!IMPORTANT]
    > Hvis du oppretter brukere på denne måten, vil du fortsatt har til å tilordne lisenser til dem i administrasjonssenteret.

##### <a name="continue-to-access-domain-joined-apps-and-devices"></a>Fortsette å få tilgang til domenetilknyttede programmer og enheter

Hvis du vil fortsette å få tilgang til domenetilknyttede programmer og enheter, kan du lese følgende artikler for to forskjellige måter for å aktivere som:
  
- [Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business](manage-windows-devices.md)
    - Dette er den anbefalte måten.

- [Access lokale ressurser fra en Azure AD-koblet enheten i Microsoft 365 Business](access-resources.md)

### <a name="connect-your-domain"></a>Koble til domenet ditt

> [!NOTE]
> Hvis du velger å bruke .onmicrosoft-domene, eller brukt Azure AD-tilkobling til å definere brukere, vil du ikke se dette trinnet.
  
Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.
  
1. Oppsettsveiviseren oppdager vanligvis registratoren og gir deg en kobling til trinnvise instruksjoner for hvordan du oppdaterer NS-postene på nettstedet til registratoren. Hvis ikke, [Endre nameservers for å konfigurere Office 365 med en hvilken som helst domeneregistrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2). 

    - Hvis du har eksisterende DNS-poster, for eksempel et eksisterende webområde, vil du håndtere dine egne DNS-poster for å kontrollere eksisterende tjenester forbli tilkoblet. Se [Grunnleggende om domenet](https://docs.microsoft.com/office365/admin/get-help-with-domains/dns-basics) for mer informasjon.

        ![Koble ditt domene-siden med jeg skal behandle mine egne DNS-poster.](media/connectyourdomainpage.png)

2. Følg trinnene i veiviseren, og e-post og andre tjenester vil bli satt opp for deg.

### <a name="set-up-security-policies-and-device-configurations"></a>Konfigurere sikkerhetspolicyer og enheten konfigurasjoner 

Disse policyene gjelder for hver bruker du gi en lisens til, eller til en gruppe brukere hvis du vil tilordne forskjellige policyer til et sett med brukere.

#### <a name="set-up-policies-in-the-wizard"></a>Definer policyer i veiviseren

Policyer som er definert i veiviseren brukes automatisk på en [sikkerhetsgruppe](https://docs.microsoft.com/office365/admin/create-groups/compare-groups#security-groups) kalt *Alle brukere*.

1. Du **beskytte filene arbeid på mobile enheter** alternativet er **Beskytt arbeidsfiler når enhetene mistes eller stjeles** valgt som standard. Du har et alternativ for å aktivere **styre hvordan brukere får tilgang til Office-filer på mobile enheter**, og dette anbefales.

    ![Skjermbilde av beskytte arbeidsfiler på mobile enheter-siden.](media/protectworkfilesondevices.png)

     - Hvis du utvider **Beskytt arbeidsfiler når enhetene mistes eller blir stjålet**, [standardverdier](protect-work-files-on-lost-or-stolen-device.md) , er forhåndsvalgt:

        ![Skjermbilde av standardverdier for å beskytte filer på tapt enheter.](media/protectworkfilesondevicesdefault.png)

    - Hvis du velger å **Behandle hvordan brukere får tilgang til Office-filer på mobile enheter** og utvide den, vises [standardverdiene](manage-user-access-on-mobile-devices.md) . Vi anbefaler at du godtar standardverdiene under konfigurasjonen for å opprette programpolicyer for Android, iOS og Windows 10 som gjelder for alle brukere. Du kan opprette flere policyer når konfigurasjonen er fullført.

        ![Skjermbilde av beskyttelsesinnstillingene for Office-filer på mobile.](media/useraccessonmobile.png)

2. Det siste trinnet på beskytte data og enheter, kan du definere policyer for å sikre Windows 10 enheter. Disse innstillingene brukes automatisk når en bruker Windows 10 kobler seg til organisasjonen. Du kan utvide **sikre Windows 10 enheter** for å vise og endre [standardverdiene](secure-windows-10-devices.md).
3. Du kan også velge å [automatisk installere Office](install-office-on-windows-10-during-setup.md) på Windows 10 enheter.

    ![Skjermbilde av satt Windows 10 konfigurasjonssiden for enheten.](media/setwin10config.png)

#### <a name="modify-or-add-policies-in-the-admin-center"></a>Endre eller legge til policyer i administrasjonssenteret

Se [Behandle Microsoft 365 Business](manage.md) for koblinger til emner om hvordan du kan vise og endre beskyttelse enheten og app-policyer, og hvordan du kan fjerne data fra, eller tilbakestille Brukerenheter.

## <a name="deploy-and-manage-windows-10"></a>Distribuere og administrere Windows 10
Se [konfigurere Windows-enheter for Microsoft 365 Business brukere](set-up-windows-devices.md) koble til Azure AD, enten under installasjonen for nye datamaskiner, eller ved å endre e-postadressen for eksisterende datamaskiner manuelt. 

### <a name="use-autopilot-to-set-up-new-devices"></a>Bruk Autopilot til å definere nye enheter

Du kan bruke [Windows Autopilot](add-autopilot-devices-and-profile.md) å automatisk forhåndskonfigurere **nye** Windows 10 enheter for en bruker, men det kan være enklere å få en [partner](https://www.microsoft.com/solution-providers/search) som kan gjøre dette for deg. Du kan også gå til [Microsoft Store](https://go.microsoft.com/fwlink/?linkid=874598) og be om en sky teknologi ekspert definere nye enheter du kjøpe for deg.

### <a name="access-on-premises-resources"></a>Få tilgang til lokale ressurser

Hvis organisasjonen bruker Windows Server Active Directory på lokaler, kan du definere Microsoft 365 Business til å beskytte Windows 10 enheter, samtidig som du har tilgang til lokale ressurser som krever lokal godkjenning. Følg trinnene i [aktivere domenetilknyttede Windows 10 enheter som skal administreres av Microsoft 365 Business](manage-windows-devices.md) å sette opp dette. Dette er den foretrukne metoden og enheter i denne tilstanden kalles Hybrid Azure AD koblet enheter.

Hvis firmaet har en lokal Active Directory, som inneholder noen lokale ressurser (for eksempel delte filer og skrivere), kan du gi din Azure AD-koblet enheter tilgang til disse ressursene ved å følge fremgangsmåten her: [Access lokale ressurser fra en Azure AD-koblet enheten i Microsoft 365 Business](access-resources.md).

## <a name="deploy-office-365-client-apps"></a>Distribuere Office 365-klientprogrammer

Hvis du velger å installere Office-programmer i automatisk under settet opp, installerer apps på Windows 10-enheter når brukerne har logget på Azure AD fra deres Windows-enheter med legitimasjonen arbeid.
Hvis du vil installere Office på mobile iOS eller Android enheter, kan du se [definere mobile enheter for forretningsbrukere som Microsoft 365](set-up-mobile-devices.md).

Du kan også installere Office individuelt. Se [installere Office på en PC eller Mac](https://support.office.com/article/4414eaaf-0478-48be-9c42-23adc471665) for å få instruksjoner.

## <a name="additional-security-settings"></a>Flere sikkerhetsinnstillinger

I tillegg til sikkerhet og overholdelse innstillingen i installasjonsveiviseren, kan du også angi følgende tilleggsinnstillinger:
  
- **Beskyttelse mot skadelig programvare for e-post**
- **Avanserte Threat Protection (ATP) trygt vedlegg**
- **ATP-klarerte koblinger**
- **PASSENDE anti-phishing**
- **Exchange Online Archiving**
- **Data tap forebygging (DLP)**
- **Azure informasjonsbeskyttelse** (Planlegge 1)
- **Intune portal tilgjengelighet**

Å komme i gang, kan du se [konfigurere avanserte sikkerhetspolicyer](set-up-advanced-security.md).

Se også [topp 10 måter å sikre bedriften din Microsoft-365](https://docs.microsoft.com/office365/admin/security-and-compliance/secure-your-business-data) for et veikart for gode fremgangsmåter for sikkerhet.