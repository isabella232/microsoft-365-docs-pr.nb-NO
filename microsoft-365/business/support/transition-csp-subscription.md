---
title: Overføre et CSP-abonnement for Microsoft 365 Business 
description: Finn ut hvordan du kan overføre et Microsoft 365 Business CSP-abonnement fra forhåndsvisning til GA. 
author: jasongroce
f1.keywords:
- NOCSH
ms.author: jasgro
ms.topic: article 
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business 
keywords: Microsoft 365 Business, Microsoft 365, SMB, overgang CSP-abonnement
ms.date: 11/01/2017
ms.openlocfilehash: 4aadfa24bec8728c7e011ac6da48a8e30516e145
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2020
ms.locfileid: "41595049"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Overføre et CSP-abonnement for Microsoft 365 Business

Hvis du har et CSP-abonnement for Microsoft 365 Business Preview, følger du denne veiledningen for å finne ut hvordan du kan overføre det eksisterende forhåndsvisningsabonnementet til Microsoft 365 Business GA (generell tilgjengelighet).

**Slik overfører du et forhåndsvisningsabonnement til GA**

1. Logg på <a href="https://partnercenter.microsoft.com" target="_blank">Partnersenter</a>.
2. Velg **Kunder**på instrumentbordet, og finn og velg deretter firmanavnet.

    Tegningene for selskapet vil bli oppført.

    ![Kundens abonnementer i Partnersenter](images/pc_customer_subscriptions_1.png)
    
3. Velg **Legg til abonnement**på selskapets **Abonnementer-side.**
4. Velg **Småbedrifter** på **Ny abonnement-siden,** og velg deretter Microsoft **365 Business** fra listen.
5. Legg til antall lisenser, og velg deretter **Neste: Se gjennom** for å se gjennom abonnementet, og velg deretter **Send .**

    ![Se gjennom det nye abonnementet på Microsoft 365 Business](images/pc_customer_reviewnewsubscription.png)

    **Lisensbaserte abonnementer** viser **Microsoft 365 Business Preview** og **Microsoft 365 Business**. Du suspenderer Forhåndsvisning-abonnementet neste gang.

6. Velg **Microsoft 365 Business Preview**.
7. Velg **Suspendert** på siden Forhåndsvisning av **Microsoft 365 for** business for å suspendere forhåndsvisningsabonnementet.

    ![Suspendere Abonnementet for Microsoft 365 Business Preview](images/pc_customer_m365bpreview_suspend.png)

8. Velg **Send** for å bekrefte.

    På **Abonnementer-siden** bekrefter du at statusen For forhåndsvisning av **Microsoft 365** viser **Suspendert**.

    ![Bekreft at statusen forhåndsvisning av abonnement er suspendert](images/pc_customer_m365bpreview_suspend_confirm.png)

9. Du kan eventuelt også validere lisensavtalen. Hvis du vil gjøre dette, gjør du følgende:
    1. Velg **Brukere og lisenser** fra selskapets **Abonnementer-side.**
    2. Velg en bruker på **Brukere og lisenser-siden.**
    3. Kontroller delen **Tilordne lisenser** på brukerens side, og bekreft at den viser **Microsoft 365 Business**.

        ![Bekreft at Microsoft 365 Business-lisensen er tilordnet til brukeren](images/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Innvirkning på kunder og brukere under og etter overgang

Det er ingen innvirkning på kunder og brukere under overgang og innleggsovergang.

## <a name="impact-to-customers-who-dont-transition"></a>Innvirkning på kunder som ikke går over

Tabellen nedenfor oppsummerer virkningen for kunder som ikke går fra et Microsoft 365 Business Preview-abonnement til et Microsoft 365 Business-abonnement.

|       | T-0 til T+30     | T+30 til T+60 | T+60 til T+120 | Utover T+120  |
|-------|-----------------|--------------|---------------|---------------|
| **Tilstand** | I gyldighetsperiode | Utløpt      | Deaktivert      | Deprovisioned |
| **Innvirkning er**                                                        |
| **Administrasjonsportal for Microsoft 365 Business** | Ingen innvirkning på funksjonalitet | Ingen innvirkning på funksjonalitet | Kan legge til / slette brukere, kjøpe abonnementer.</br> Kan ikke tilordne/tilbakekalle lisenser. | Kundens abonnement og alle data slettes. Administrator kan administrere andre betalte abonnementer. |
| **Office-apper**                         | Ingen innvirkning på sluttbrukeren | Ingen innvirkning på sluttbrukeren | Office går inn i modus for redusert funksjonalitet.</br> Brukere kan bare vise filer. | Office går inn i modus for redusert funksjonalitet.</br> Brukere kan bare vise filer. |
| **Skytjenester (SharePoint Online, Exchange Online, Skype, Teams og mer)** | Ingen innvirkning på sluttbrukeren | Ingen innvirkning på sluttbrukeren | Sluttbrukere og administratorer har ingen tilgang til data i skyen. | Kundens abonnement og alle data slettes. |
| **EM+S-komponenter** | Ingen innvirkning på administratorer</br> Ingen innvirkning på sluttbrukeren | Ingen innvirkning på administratorer</br> Ingen innvirkning på sluttbrukeren | Funksjonen håndheves ikke lenger.</br> Se [Innvirkninger på mobilenheter ved utløp av abonnementet](#mobile-device-impacts-upon-subscription-expiration) og Windows [10 PC-innvirkninger ved utløp av abonnementet](#windows-10-pc-impacts-upon-subscription-expiration) for mer informasjon. | Funksjonen håndheves ikke lenger.</br> Se [Innvirkninger på mobilenheter ved utløp av abonnementet](#mobile-device-impacts-upon-subscription-expiration) og Windows [10 PC-innvirkninger ved utløp av abonnementet](#windows-10-pc-impacts-upon-subscription-expiration) for mer informasjon. |
| **Windows 10-bedrift** | Ingen innvirkning på administratorer</br> Ingen innvirkning på sluttbrukeren | Ingen innvirkning på administratorer</br> Ingen innvirkning på sluttbrukeren | Funksjonen håndheves ikke lenger.</br> Se [Innvirkninger på mobilenheter ved utløp av abonnementet](#mobile-device-impacts-upon-subscription-expiration) og Windows [10 PC-innvirkninger ved utløp av abonnementet](#windows-10-pc-impacts-upon-subscription-expiration) for mer informasjon. | Funksjonen håndheves ikke lenger.</br> Se [Innvirkninger på mobilenheter ved utløp av abonnementet](#mobile-device-impacts-upon-subscription-expiration) og Windows [10 PC-innvirkninger ved utløp av abonnementet](#windows-10-pc-impacts-upon-subscription-expiration) for mer informasjon. |
| **Azure AD-pålogging til en Windows 10-PC** | Ingen innvirkning på administratorer</br> Ingen innvirkning på sluttbrukeren | Ingen innvirkning på administratorer</br> Ingen innvirkning på sluttbrukeren | Ingen innvirkning på administratorer</br> Ingen innvirkning på sluttbrukeren | Når leieren er slettet, kan en bruker bare logge på med lokal legitimasjon. Re-bilde enheten hvis det ikke er noen lokal legitimasjon. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Innvirkning på mobilenheter ved utløp av abonnementet

Tabellen nedenfor oppsummerer virkningen på retningslinjene for appadministrasjon på mobilenheter.

|                            | Fullt lisensiert opplevelse                      | T+60 dager etter utløp          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Slette arbeidsfiler fra en inaktiv enhet** | Arbeidsfiler fjernes etter valgte dager | Arbeidsfiler forblir på brukerens personlige enheter |
| **Tvinge brukere til å lagre alle arbeidsfiler til OneDrive for Business** | Arbeidsfiler kan bare lagres på OneDrive for Business | Arbeidsfiler kan lagres hvor som helst |
| **Kryptere arbeidsfiler** | Arbeidsfiler krypteres | Arbeidsfiler krypteres ikke lenger.</br> Sikkerhetspolicyer fjernes og Office-data på apper fjernes. |
| **Krev PIN-kode eller fingeravtrykk for å få tilgang til Office-apper** | Begrenset tilgang til apper | Ingen tilgangsbegrensning på appnivå |
| **Tilbakestill PIN-kode når påloggingen mislykkes** | Begrenset tilgang til apper | Ingen tilgangsbegrensning på appnivå |
| **Kreve at brukere logger på igjen etter at Office-apper har vært inaktive** | Pålogging kreves | Ingen pålogging kreves |
| **Avslå tilgang til arbeidsfiler på enheter som er jailbreaket eller rootet** | Arbeidsfiler kan ikke nås på jailbroken /rooted enheter | Arbeidsfiler kan nås på jailbroken /rooted enheter |
| **Tillat brukere å kopiere innhold fra Office-apper til Personlige apper** | Kopiere/lime inn begrenset til apper som er tilgjengelige som en del av Microsoft 365 Business-abonnementet | Kopier/lim inn tilgjengelig for alle apper |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Windows 10 PC-effekter ved utløp av abonnementet

Tabellen nedenfor oppsummerer virkningen på konfigurasjonspolicyene for Windows 10-enheten.

|                            | Fullt lisensiert opplevelse                      | T+60 dager etter utløp          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Bidra til å beskytte PCer mot trusler ved hjelp av Windows Defender** | Slå av/på er utenfor brukerkontrollen | Brukeren kan aktivere/deaktivere Windows Defender på Windows 10-PCen |
| **Beskytte PC-er fra nettbaserte trusler i Microsoft Edge** | PC-beskyttelse i Microsoft Edge | Brukeren kan aktivere/deaktivere PC-beskyttelse i Microsoft Edge |
| **Slå av enhetsskjermen når den er inaktiv** | Administrator definerer policy for intervallfor tidsavbrudd for skjermen | Tidsavbruddet for skjerm kan konfigureres av sluttbrukeren |
| **Tillat brukere å laste ned apper fra Microsoft Store** | Administrator definerer om en bruker kan laste ned apper fra Microsoft Store | Brukeren kan laste ned apper fra Microsoft Store når som helst |
| **Gi brukere tilgang til Cortana** | Administrator definerer policy for brukertilgang til Cortana | Brukerenheter for å slå på/av Cortana |
| **Tillat brukere å motta tips og annonser fra Microsoft** | Administrator definerer policy på brukeren motta tips og annonser fra Microsoft | Brukeren kan aktivere/deaktivere tips og annonser fra Microsoft |
| **Tillat at brukere kan kopiere innhold fra Office-apper til personlige apper** | Administrator definerer policy en slik at Windows 10-enheter skal være oppdatert | Brukere kan bestemme når de skal oppdatere Windows |
