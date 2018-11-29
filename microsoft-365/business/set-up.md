---
title: Konfigurere Microsoft 365 Business ved hjelp av veiviseren for konfigurasjon
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
ms.collection: Adm_O365
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 6e7a2dfd-8ec4-4eb7-8390-3ee103e5fece
description: Lær hvordan du konfigurerer Microsoft 365 Business ved å fylle ut fire trinn.
ms.openlocfilehash: f57239b884bd2e186c0bc01973130a10fa4cfe84
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/28/2018
ms.locfileid: "26982196"
---
# <a name="set-up-microsoft-365-business-by-using-the-setup-wizard"></a>Konfigurere Microsoft 365 Business ved hjelp av veiviseren for konfigurasjon

Fullfør trinn 1-4 nedenfor.
  
### <a name="set-up-microsoft-365-business"></a>Konfigurere Microsoft 365 Business

Se en video om hvordan du konfigurerer Microsoft 365 Business når du ikke har en lokale Active Directory:
  
> [!VIDEO https://www.microsoft.com/videoplayer/embed/0705c337-f3e8-4d28-bb6c-530cd28e99f2?autoplay=false]
  
Fremgangsmåten for oppsett inneholder informasjon for oppsett som inkluderer lokale Active Directory. Hvis du vil fortsette å få tilgang til domenetilknyttede enheter, Les følgende artikler for to forskjellige måter for å aktivere som, og Fullfør trinnene før du kjører veiviseren for installasjon:
  
- [Aktivere domenetilknyttede Windows 10-enheter som skal administreres av Microsoft 365 Business](manage-windows-devices.md)
    
    – Dette er den anbefalte måten.
    
- [Access lokale ressurser fra en Azure AD-koblet enheten i Microsoft 365 Business](access-resources.md)
    
### <a name="step-1-personalize-sign-in"></a>Trinn 1: Tilpasse pålogging

1. Logg på [Microsoft 365 Business](https://portal.microsoft.com) ved hjelp av legitimasjonen for global administrator. Velg **Administrasjon**-flisen for å gå til administrasjonssenteret. 
    
2. Velg **Start konfigurasjon** (det kan hende du ser **Fortsett konfigurasjon** i stedet, avhengig av status) i administrasjonssenteret for å starte veiviseren. 
    
3. Skriv inn domenenavnet du vil bruke (for eksempel contoso.com).
    
    Gå videre og Skriv inn domenet ditt selv om du har bekreftet det ved hjelp av Azure AD-tilkobling, for eksempel. De følgende to trinnene gjelder ikke for deg hvis du brukte Azure AD-tilkobling for å bekrefte domenet.
    
4. Følg trinnene i veiviseren til å [opprette DNS-poster på alle DNS-vertsleverandøren for Office 365](https://support.office.com/article/7b7b075d-79f9-4e37-8a9e-fb60c1d95166) , som bekrefter at du eier domenet. 
    
    Du kan vise et eksempel video av [Video: installasjonsprogrammet for Office 365 i administrasjonssenteret nye](https://support.office.com/article/a8c2002a-34bc-4ab3-93d8-9b5156c48bf8). Vær oppmerksom på at denne videoen ikke inneholder data protection trinnene i Microsoft 365 Business.
    
    ![Screenshot of the Business Cloud Suite setup wizard.](media/3c4fd40c-2de1-4a87-8ee0-78d3928c7bb7.png)
  
### <a name="step-2-add-users-and-assign-licenses"></a>Trinn 2: Legge til brukere og tilordne lisenser

1. Du kan legge til brukere her, eller du kan [legge til brukere senere](add-users-m365b.md) i administrasjonssenteret. 
    
    Alle brukerne du legger til, får automatisk tildelt en Microsoft 365 Business-lisens.
    
2. Hvis ditt Microsoft 365 Business-abonnement har eksisterende brukere (for eksempel hvis du brukte Azure AD Connect), får du muligheten til å tildele lisenser til dem nå. Gå videre og legg til lisenser for dem også.
    
3. Du får også en mulighet til å dele legitimasjon med de nye brukerne du har lagt til. Du kan velge å skrive dem ut, sende dem via e-post eller laste dem ned.
    
4. Hopp over overføring av e-postmeldinger, og velg **Neste** på **Overfør e-postmeldinger**-siden. 
    
    Hvis du flytter fra en annen leverandør av e-post og vil kopiere dataene senere, kan du [Overfør e-post og kontakter til Office 365](https://support.office.com/article/a3e3bddb-582e-4133-8670-e61b9f58627e).
    
    ![Screenshot of two new users added in the setup wizard](media/8f729967-5c65-4ceb-b737-18119db40564.png)
  
### <a name="step-3-connect-your-domain"></a>Trinn 3: Koble til domenet

> [!NOTE]
> Hvis du velger å bruke .onmicrosoft-domene, eller brukt Azure AD-tilkobling, vil du ikke se dette trinnet. 
  
Hvis du vil konfigurere tjenester, må du oppdatere noen poster på DNS-verten eller domeneregistratoren.
  
1. Installasjonsveiviseren vanligvis oppdager registraren og gir deg en kobling til trinnvise instruksjoner for å oppdatere NS-postene på webområdet registrar. Hvis ikke, [Endre nameservers for å konfigurere Office 365 med en hvilken som helst domeneregistrar](https://support.office.com/article/a8b487a9-2a45-4581-9dc4-5d28a47010a2).
    
2. E-post og andre tjenester vil bli opprettet for deg
    
### <a name="step-4-manage-devices-and-work-files"></a>Trinn 4: Håndtere enheter og arbeide filer

1. Siden Angi **styre hvordan brukere får tilgang til Office-filer på mobile enheter** innstillinger og **Beskytt arbeidsfiler når enhetene mistes eller blir stjålet** **på**, på **Beskytt arbeidsfiler på mobile enheter** . Du kan også få tilgang til hver underordnet innstilling ved å klikke pilene ved siden av hver innstilling.
  
  Alle de lisensierte brukere arbeidsfiler blir nå beskyttet på iOS og Android enheter, så snart de [installerer Office-programmer](set-up-mobile-devices.md) (og godkjenne legitimasjonen Microsoft 365 Business). 
  
  ![Screenshot of protect work files on your mobile devices page](media/3139a9aa-6228-4e74-8166-c6a886d7319f.PNG)
  
2. På siden **Angi Windows-10 enhetskonfigurasjon** sette innstillingen for **Sikker Windows 10 enheter** **på**.
  
   Du kan også få tilgang til hver underordnet innstilling ved å klikke vinkeltegnet ved siden av den.
  
3. Sett innstillingen for å **Installere Office på Windows 10 enheter** til **Ja** hvis alle brukerne har 10 for Windows-datamaskiner, og ingen eksisterende Office installeres, eller klikk for å kjøre Office-installasjoner. Hvis dette ikke er tilfelle, setter du dette alternativet til **Nei**. Du kan [automatisk installere Office](auto-install-or-uninstall-office.md) senere fra administrasjonssenteret når du har klargjort på brukernes datamaskiner. For instruksjoner, kan du se [forberede installasjon av Office-klienten](prepare-for-office-client-deployment.md).
  
    Den lisensierte brukere arbeidsfiler på Windows 10 enheter blir vist så snart de [bli med sine Windows 10-enhet](set-up-windows-devices.md) til et Microsoft 365 Business Azure AD-domene eller [installere Windows 10 på en ny datamaskin](https://support.office.com/article/c654bd23-d256-4ac7-8fba-0c993bf5a771.aspx) mens du samtidig å bli med i Microsoft-365 Business Azure AD-domene. 
  
4. Klikk **Neste** , og du er ferdig med installasjonen. 
  
    La oss tilbakemelding på dette trinnet for å hjelpe oss å forbedre opplevelsen.
  
    ![Screenshot of Prepare Windows 10 devices page](media/bff701c1-48a3-44f4-aa95-9d959d57c85b.PNG)
  
## <a name="additional-security-settings"></a>Flere sikkerhetsinnstillinger

I tillegg til sikkerhet og overholdelse innstillingen i installasjonsveiviseren, kan du også angi følgende tilleggsinnstillinger:
  
- Angi beskyttelse mot usikre vedlegg. **Avansert Threat Protection** (ATP) identifiserer skadelig innhold og blokkerer leveringen av usikre vedlegg, bidrar til å beskytte deg mot phishing-forsøk og ransomware infeksjoner. Hvis du vil aktivere beskyttelse for vedlegg, kan du se [definere policyer for Office 365 ATP trygt vedlegg](https://support.office.com/article/078eb946-819a-4e13-8673-fe0c0ad3a775#setpolicy).
    
- Beskytte miljøet når brukere klikker skadelig koblinger. ATP undersøker koblinger i e-post når en bruker klikker dem.. Hvis en kobling er usikre, er brukeren varsles om ikke å gå til webområdet eller informert om at webområdet er blokkert. Dette bidrar til å beskytte deg mot phishing-forsøk. [Definer policyer for Office 365 ATP-klarerte koblinger](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#reveddefaultscc) eller [definere policyer for Office 365 ATP-klarerte koblinger](https://support.office.com/article/bdd5372d-775e-4442-9c1b-609627b94b5d#addemailpolscc).
    
- Du kan beholde alle postboks-innhold, inkludert Slettede elementer ved å plassere hele postboksen for en bruker i **rettstvist holder**. For instruksjoner, se 
- [Definer tilbakeholdelse av e-post med Exchange Online-arkivering](security-features.md#set-up-email-retention-with-exchange-online-archiving).
    
- Definer tilpassede **policyer for dokumentoppbevaring**, for eksempel å bevare i en bestemt tidsperiode eller slette innholdet permanent på slutten av Oppbevaringstiden. Du kan aktivere egendefinerte oppbevaringspolicyer i verdipapirer og overholdelse center, går du til **styring av Data** \> **oppbevaring**, og følg deretter instruksjonene i veiviseren. Hvis du vil ha mer informasjon, se [Oversikt over policyer for dokumentoppbevaring](https://support.office.com/article/5e377752-700d-4870-9b6d-12bfc12d2423).
    
## <a name="next-steps"></a>Neste trinn

For brukere som har sine lisenser, er neste trinn å konfigurere enheter.<br/> Se [konfigurere Windows-enheter for forretningsbrukere som Microsoft 365](set-up-windows-devices.md) og [definere mobile enheter for forretningsbrukere som Microsoft 365](set-up-mobile-devices.md). <br/>Se [Behandle Microsoft 365 Business](manage.md) for koblinger til emner om hvordan du angir beskyttelse enheten og app-policyer, og hvordan du kan fjerne data fra Brukerenheter. 
  


