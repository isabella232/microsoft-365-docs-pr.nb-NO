---
title: Overføre et Microsoft 365 Business CSP-abonnement 
description: Finn ut hvordan du kan overføre et Microsoft 365 Business CSP-abonnement fra forhåndsvisning til GA. 
author: jasongroce
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Business, Microsoft 365, SMB, overgang CSP abonnement
ms.date: 11/01/2017
ms.openlocfilehash: b907c3a3bccc4179369890b7769dcb14ba2acbb7
ms.sourcegitcommit: 2c2248b03f7753d64490f2f7e56ec644a235b65a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/15/2019
ms.locfileid: "38311098"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Overføre et Microsoft 365 Business CSP-abonnement

Hvis du har et abonnement på Microsoft 365 Business Preview CSP, følger du denne veiledningen for å finne ut hvordan du kan overføre det eksisterende Forhåndsvisnings abonnementet til Microsoft 365 Business GA (generell tilgjengelighet).

**Slik overfører du et forhåndsvisningsabonnement til GA**

1. Logg på <a href="https://partnercenter.microsoft.com" target="_blank">partner senter</a>.
2. Velg **kunder**fra instrumentbordet, og Finn og velg firmanavnet.

    Abonnementene for selskapet vil bli oppført.

    ![Kundens abonnementer i partner senteret](images/pc_customer_subscriptions_1.png)
    
3. Velg **Legg til abonnement**på firmaets **abonnementer** -side.
4. Velg **Small Business** på siden **nytt abonnement** , og velg deretter **Microsoft 365 Business** fra listen.
5. Legg til antall lisenser, og velg deretter **Neste: gå gjennom** for å se gjennom abonnementet, og velg deretter **Send**.

    ![Se gjennom det nye abonnementet på Microsoft 365 Business](images/pc_customer_reviewnewsubscription.png)

    **Lisensbasert abonnement** vil vise **Microsoft 365 Business Preview** og **Microsoft 365 Business**. Du suspenderer Forhåndsvisnings abonnementet neste gang.

6. Velg **Microsoft 365 Business Preview**.
7. Velg **suspendert** på siden **Microsoft 365 Business Preview** for å utsette Forhåndsvisnings abonnementet.

    ![Suspendere Microsoft 365 Business Preview-abonnementet](images/pc_customer_m365bpreview_suspend.png)

8. Velg **Send** for å bekrefte.

    På siden **abonnementer** kontrollerer du at statusen for **Business Preview for Microsoft 365** viser **deaktivert**.

    ![Bekreft at statusen for forhåndsvisning av abonnement er suspendert](images/pc_customer_m365bpreview_suspend_confirm.png)

9. Alternativt kan du også validere lisensavtalen. Hvis du vil gjøre dette, følger du denne fremgangsmåten:
    1. Velg **brukere og lisenser** fra firmaets **abonnementer** -side.
    2. Velg en bruker på siden **brukere og lisenser** .
    3. Se delen **Tilordne lisenser** på brukerens side, og Bekreft at den viser **Microsoft 365 Business**.

        ![Bekreft at Microsoft 365 Business-lisensen er tilordnet til brukeren](images/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Innvirkning på kunder og brukere under og etter overgangen

Det er ingen innvirkning på kunder og brukere under overgangen og etter overgangen.

## <a name="impact-to-customers-who-dont-transition"></a>Innvirkning på kunder som ikke overgang

Tabellen nedenfor oppsummerer innvirkningen på kunder som ikke går fra et Microsoft 365 Business Preview-abonnement til et Microsoft 365 Business-abonnement.

|       | T-0 til T + 30     | T + 30 til T + 60 | T + 60 til T + 120 | Utover T + 120  |
|-------|-----------------|--------------|---------------|---------------|
| **Tilstand** | I nåde perioden | Utløpt      | Deaktivert      | Deprovisioned |
| **Virkninger på tjenesten**                                                        |
| **Microsoft 365 bedrifts administrasjonsportal** | Ingen innvirkning på funksjonaliteten | Ingen innvirkning på funksjonaliteten | Kan legge til/slette brukere, kjøpe abonnementer.</br> Kan ikke tilordne/tilbakekalle lisenser. | Kundens abonnement og alle data slettes. Administrator kan administrere andre betalte abonnementer. |
| **Office-programmer**                         | Ingen sluttbruker innvirkning | Ingen sluttbruker innvirkning | Office går inn i redusert funksjonalitetsmodus.</br> Brukere kan bare vise filer. | Office går inn i redusert funksjonalitetsmodus.</br> Brukere kan bare vise filer. |
| **Skytjenester (SharePoint Online, Exchange Online, Skype, Teams og mer)** | Ingen sluttbruker innvirkning | Ingen sluttbruker innvirkning | Sluttbrukere og administratorer har ingen tilgang til data i skyen. | Kundens abonnement og alle data slettes. |
| **EM + S-komponenter** | Ingen administrator innvirkning</br> Ingen sluttbruker innvirkning | Ingen administrator innvirkning</br> Ingen sluttbruker innvirkning | Kapasiteten håndheves ikke lenger.</br> Se [innvirkning på mobilenheter når abonnementet utløper](#mobile-device-impacts-upon-subscription-expiration) , og [Windows 10-PC påvirker når abonnementet utløper](#windows-10-pc-impacts-upon-subscription-expiration) for mer informasjon. | Kapasiteten håndheves ikke lenger.</br> Se [innvirkning på mobilenheter når abonnementet utløper](#mobile-device-impacts-upon-subscription-expiration) , og [Windows 10-PC påvirker når abonnementet utløper](#windows-10-pc-impacts-upon-subscription-expiration) for mer informasjon. |
| **Windows 10 Business** | Ingen administrator innvirkning</br> Ingen sluttbruker innvirkning | Ingen administrator innvirkning</br> Ingen sluttbruker innvirkning | Kapasiteten håndheves ikke lenger.</br> Se [innvirkning på mobilenheter når abonnementet utløper](#mobile-device-impacts-upon-subscription-expiration) , og [Windows 10-PC påvirker når abonnementet utløper](#windows-10-pc-impacts-upon-subscription-expiration) for mer informasjon. | Kapasiteten håndheves ikke lenger.</br> Se [innvirkning på mobilenheter når abonnementet utløper](#mobile-device-impacts-upon-subscription-expiration) , og [Windows 10-PC påvirker når abonnementet utløper](#windows-10-pc-impacts-upon-subscription-expiration) for mer informasjon. |
| **Azure AD-pålogging til en Windows 10-PC** | Ingen administrator innvirkning</br> Ingen sluttbruker innvirkning | Ingen administrator innvirkning</br> Ingen sluttbruker innvirkning | Ingen administrator innvirkning</br> Ingen sluttbruker innvirkning | Når leieren er slettet, kan en bruker bare logge på med lokal legitimasjon. Re-image enheten hvis det ikke er noen lokal legitimasjon. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Mobilenheter påvirker når abonnementet utløper

Tabellen nedenfor oppsummerer innvirkningen på App Management-policyene på mobile enheter.

|                            | Fullt lisensiert erfaring                      | T + 60 dager etter utløp          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Slett arbeidsfiler fra en inaktiv enhet** | Arbeidsfiler fjernes etter utvalgte dager | Arbeidsfiler forblir på brukerens personlige enheter |
| **Tvinge brukere til å lagre alle arbeidsfiler til OneDrive for Business** | Arbeidsfiler kan bare lagres i OneDrive for Business | Arbeidsfiler kan lagres hvor som helst |
| **Kryptere arbeidsfiler** | Arbeidsfiler krypteres | Arbeidsfiler krypteres ikke lenger.</br> Sikkerhetspolicyer fjernes, og Office-data på apper fjernes. |
| **Krev PIN eller fingeravtrykk for å få tilgang til Office-apper** | Begrenset tilgang til apper | Ingen tilgangsbegrensning på App-nivå |
| **Tilbakestill PIN-kode når påloggingen mislykkes** | Begrenset tilgang til apper | Ingen tilgangsbegrensning på App-nivå |
| **Krev at brukere logger på på nytt etter at Office-apper har vært inaktive** | Pålogging kreves | Ingen pålogging kreves |
| **Avslå tilgang til arbeidsfiler på enheter som er jailbreaket eller rootet** | Arbeidsfiler kan ikke nås på jailbroken/forankret enheter | Arbeid filer kan nås på jailbroken/forankret enheter |
| **Tillat brukere å kopiere innhold fra Office-apper til personlige apper** | Kopier/Lim inn begrenset til apper som er tilgjengelige som en del av Microsoft 365 Business-abonnement | Kopier/Lim inn tilgjengelig for alle apper |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>PC-en med Windows 10 påvirker når abonnementet utløper

Tabellen nedenfor oppsummerer innvirkningen på enhets konfigurasjons policyene for Windows 10.

|                            | Fullt lisensiert erfaring                      | T + 60 dager etter utløp          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Bidra til å beskytte PC-er mot trusler ved hjelp av Windows Defender** | Slå på/av er utenfor brukerkontroll | Brukeren kan slå på/av Windows Defender på Windows 10-PC-en |
| **Beskytte PC-er fra nettbaserte trusler i Microsoft Edge** | PC-beskyttelse i Microsoft Edge | Brukeren kan slå på/av PC-beskyttelse i Microsoft Edge |
| **Slå av enhetsskjermen når inaktiv** | Administrator definerer intervall policy for tidsavbrudd for skjerm | Tidsavbrudd for skjerm kan konfigureres av sluttbrukeren |
| **Tillat brukere å laste ned apper fra Microsoft Store** | Administrator definerer om en bruker kan laste ned apper fra Microsoft store | Brukeren kan laste ned apper fra Microsoft store når som helst |
| **Gi brukere tilgang til Cortana** | Admin definerer retningslinjer for bruker tilgang til Cortana | Bruker enheter for å slå på/av Cortana |
| **Tillat brukere å motta tips og reklame fra Microsoft** | Admin definerer retningslinjer for brukeren motta tips og annonser fra Microsoft | Bruker kanne skru på/av drikkepenger og annonsene fra Microsoft |
| **Tillat at brukere kan kopiere innhold fra Office-apper til personlige apper** | Admin definerer policy for å holde Windows 10-enheter oppdatert | Brukere kan bestemme når de vil oppdatere Windows |
