---
title: Overføre et Microsoft 365 Business CSP-abonnement 
description: Finn ut hvordan du kan overføre Microsoft 365 Business CSP-abonnementet fra forhåndsvisning til GA. 
author: jasongroce
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Business, Microsoft 365, SMB, overgang CSP-abonnement
ms.date: 11/01/2017
ms.openlocfilehash: 8109c0b00f06a15c12bbccf89e7f49dc3fa4b34a
ms.sourcegitcommit: e491c4713115610cbe13d2fbd0d65e1a41c34d62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/16/2019
ms.locfileid: "26982486"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Overføre et Microsoft 365 Business CSP-abonnement

Hvis du har et Microsoft 365 Business forhåndsvisning CSP-abonnement, kan du følge denne veiledningen for å finne ut hvordan du kan bytte det eksisterende abonnementet for forhåndsvisning til Microsoft 365 Business GA (generell tilgjengelighet).

**Hvordan du går over et abonnement for forhåndsvisning til GA**

1. Logg på <a href="https://partnercenter.microsoft.com" target="_blank">Partner Center</a>.
2. Fra dashboard, utvalgte **Kunder**, og Finn og velg firmanavnet.

    Abonnementer for selskapet vises.

    ![Kundens abonnementer i Partner Center](images/pc_customer_subscriptions_1.png)
    
3. Velg **Legg til abonnement**i selskapets **abonnementer** -siden.
4. **Nytt abonnement** -siden velger du **små bedrifter** , og velg deretter **Microsoft 365 Business** fra listen.
5. Legge til antall lisenser, og velg deretter **Neste: Se gjennom** til å gå gjennom abonnementet, og velg deretter **Send**.

    ![Se gjennom nye abonnementet på Microsoft 365 Business](images/pc_customer_reviewnewsubscription.png)

    **Lisens-baserte abonnementer** viser **Microsoft 365 Business forhåndsvisning** og **Microsoft 365 Business**. Du må stoppe abonnementet på Forhåndsvisning av neste.

6. Velg **Microsoft 365 Business forhåndsvisning**.
7. Velg **Suspended** for å stoppe abonnementet på Forhåndsvisning i **Microsoft 365 Business Preview** -siden.

    ![Stoppe abonnementet på Microsoft 365 Business Preview](images/pc_customer_m365bpreview_suspend.png)

8. Velg **Send** for å bekrefte.

    Bekreft at **Microsoft 365 Business Preview** statusen viser **Suspended**på siden **abonnementer** .

    ![Bekreft forhåndsvisning abonnementet statusen er stoppet](images/pc_customer_m365bpreview_suspend_confirm.png)

9. Du kan eventuelt også validere lisensavtalen. Følg disse trinnene:
    1. Velg **brukere og lisenser** fra selskapets **abonnementer** -siden.
    2. Velg en bruker fra **brukere og lisenser** -siden.
    3. Bekreft at den viser **Microsoft 365 Business**i brukerens side, se delen **tilordne lisenser** .

        ![Bekrefte Microsoft 365 Business-lisensen er tilordnet til bruker](images/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Påvirkning på kunder og brukere under og etter overgang

Det er ingen innvirkning på kunder og brukere under overgangen og innlegget overgang.

## <a name="impact-to-customers-who-dont-transition"></a>Virkningen for kunder som ikke over

Tabellen nedenfor viser virkningene til kunder som ikke over fra et Microsoft 365 Business Preview-abonnement til et abonnement på Microsoft 365 Business.

|       | T-0 til T + 30     | T + 30 til T + 60 | T + 60 til T + 120 | Utover T + 120  |
|-------|-----------------|--------------|---------------|---------------|
| **Tilstand** | I gyldighetsperioden | Utløpt      | Deaktivert      | Deprovisioned |
| **Tjenesten innvirkninger**                                                        |
| **Microsoft 365 Business Administrasjonsportal** | Ingen innvirkning på funksjonaliteten | Ingen innvirkning på funksjonaliteten | Legge til eller slette brukere, kan kjøpe abonnementer.</br> Kan ikke tilordne/Opphev lisenser. | Kundens abonnement og alle data som er slettet. Admin kan behandle andre betalte abonnementer. |
| **Office-programmer**                         | Ingen innvirkning på sluttbrukeren | Ingen innvirkning på sluttbrukeren | Office går inn i modus for redusert funksjonalitet.</br> Brukere kan vise bare filer. | Office går inn i modus for redusert funksjonalitet.</br> Brukere kan vise bare filer. |
| **Cloud services (SharePoint Online, Exchange Online, Skype, grupper og mer)** | Ingen innvirkning på sluttbrukeren | Ingen innvirkning på sluttbrukeren | Sluttbrukere og administratorer har ikke tilgang til data i skyen. | Kundens abonnement og alle data slettet. |
| **EM + S komponenter** | Ingen innvirkning på admin</br> Ingen innvirkning på sluttbrukeren | Ingen innvirkning på admin</br> Ingen innvirkning på sluttbrukeren | Funksjonen vil slutte å bli gjennomført.</br> Se [mobilenhet påvirker når abonnementet utløper](#mobile-device-impacts-upon-subscription-expiration) og [Windows 10 PC innvirkninger på abonnementet utløper](#windows-10-pc-impacts-upon-subscription-expiration) for mer informasjon. | Funksjonen vil slutte å bli gjennomført.</br> Se [mobilenhet påvirker når abonnementet utløper](#mobile-device-impacts-upon-subscription-expiration) og [Windows 10 PC innvirkninger på abonnementet utløper](#windows-10-pc-impacts-upon-subscription-expiration) for mer informasjon. |
| **Windows 10 Business** | Ingen innvirkning på admin</br> Ingen innvirkning på sluttbrukeren | Ingen innvirkning på admin</br> Ingen innvirkning på sluttbrukeren | Funksjonen vil slutte å bli gjennomført.</br> Se [mobilenhet påvirker når abonnementet utløper](#mobile-device-impacts-upon-subscription-expiration) og [Windows 10 PC innvirkninger på abonnementet utløper](#windows-10-pc-impacts-upon-subscription-expiration) for mer informasjon. | Funksjonen vil slutte å bli gjennomført.</br> Se [mobilenhet påvirker når abonnementet utløper](#mobile-device-impacts-upon-subscription-expiration) og [Windows 10 PC innvirkninger på abonnementet utløper](#windows-10-pc-impacts-upon-subscription-expiration) for mer informasjon. |
| **Azure AD-pålogging til en Windows-PC for 10** | Ingen innvirkning på admin</br> Ingen innvirkning på sluttbrukeren | Ingen innvirkning på admin</br> Ingen innvirkning på sluttbrukeren | Ingen innvirkning på admin</br> Ingen innvirkning på sluttbrukeren | Når du leier er slettet, kan en bruker logge på med bare lokal legitimasjon. Image enheten på nytt hvis ingen lokal legitimasjon. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Mobil enhet innvirkninger på abonnementet utløper

Tabellen followint oppsummerer virkningen på app-policyer for informasjonsbehandling på mobile enheter.

|                            | Fullstendig lisensiert opplevelse                      | T + 60 dager etter utløp          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Slett arbeidsfiler fra en inaktiv-enhet** | Arbeidsfiler fjernes når valgt dager | Arbeidsfiler beholdes på brukerens personlige enheter |
| **Tvinge brukere til å lagre alle arbeidsfiler til OneDrive for Business** | Arbeidsfiler kan bare lagres på OneDrive for bedrifter | Arbeidsfiler kan lagres hvor som helst |
| **Kryptere arbeidsfiler** | Arbeidsfiler er krypterte. | Arbeidsfiler krypteres ikke lenger.</br> Sikkerhetspolicyer fjernes og Office data på apps er fjernet. |
| **Krev PIN-kode eller fingeravtrykk for å få tilgang til Office-programmer** | Begrenset tilgang til apps | Ingen app nivå tilgangsbegrensning |
| **Tilbakestill PIN-koden når påloggingen mislykkes** | Begrenset tilgang til apps | Ingen app nivå tilgangsbegrensning |
| **Brukere må logge på igjen etter at Office-programmer har blitt inaktiv** | Pålogging kreves | Ingen pålogging kreves for å få tilgang til programmer |
| **Avslå tilgang til arbeidsfiler på enheter som er jailbreaket eller rootet** | Får ikke tilgang til arbeidsfiler på jailbroken/rot enheter | Kan få tilgang til arbeidsfiler på jailbroken/rot enheter |
| **Tillat brukere å kopiere innhold fra Office-programmer til personlige apps** | Kopiere og lime inn begrenset til programmer som er tilgjengelige som en del av Microsoft 365 Business-abonnement | Kopiere og lime inn tilgjengelig for alle programmer |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Windows 10 PC innvirkninger på abonnementet utløper

Tabellen nedenfor viser virkningen på Windows 10 konfigurasjon-retningslinjer for enheten.

|                            | Fullstendig lisensiert opplevelse                      | T + 60 dager etter utløp          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Beskytte PC mot trusler ved hjelp av Windows Defender** | Slå på/av, er utenfor kontroll | Brukeren kan Aktiver/deaktiver Windows Defender i Windows 10 PC |
| **Beskytt PC-er fra nettbaserte trusler i Microsoft Edge** | PC-beskyttelse i Microsoft Edge | Brukeren kan slå på/av PC-beskyttelse i Microsoft Edge |
| **Slå av enhetsskjermen når inaktiv** | Admin definerer skjermen tidsavbrudd intervall policy | Skjermen tidsavbrudd kan konfigureres av sluttbruker |
| **Tillat brukere å laste ned apper fra Microsoft Store** | Admin angir om en bruker kan laste ned programmer fra Microsoft Store | Brukeren kan laste ned programmer fra Microsoft Store når som helst |
| **Gi brukere tilgang til Cortana** | Admin definerer policyen på brukertilgang til Cortana | Brukerenheter til å slå på/av Cortana |
| **Tillat brukere å motta tips og reklame fra Microsoft** | Admin definerer policyen på brukeren får tips og reklame fra Microsoft | Brukeren kan slå på/av tips og reklame fra Microsoft |
| **Tillat at brukere kan kopiere innhold fra Office-apper til personlige apper** | Admin definerer policyen for å holde det oppdatert Windows 10 enheter | Brukere kan bestemme når du vil oppdatere Windows |




