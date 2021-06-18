---
title: Overgang til et CSP-abonnement for Microsoft 365 Business
description: Finn ut hvordan du kan gå over et microsoft 365 Business CSP-abonnement fra forhåndsvisning til generell tilgjengelighet (GA).
author: jasongroce
f1.keywords:
- NOCSH
ms.custom:
- seo-marvel-mar
- AdminSurgePortfolio
ms.author: jasongroce
ms.topic: article
manager: jasonh
ms.prod: microsoft-365-business
localization_priority: Normal
audience: microsoft-business
keywords: Microsoft 365 Business, Microsoft 365, SMB, CSP-abonnement for overgang
ms.date: 11/01/2017
ms.openlocfilehash: 3f6c71edb50cc3c5509e61a83efb64185c10648d
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925007"
---
# <a name="transition-a-microsoft-365-business-csp-subscription"></a>Overgang til et CSP-abonnement for Microsoft 365 Business

Hvis du har et CSP-abonnement for Microsoft 365 Business Preview, følger du denne veiledningen for å finne ut hvordan du kan gå over det eksisterende forhåndsvisningsabonnementet til Microsoft 365 Business GA (generell tilgjengelighet).

**Slik går du over et forhåndsversjonsabonnement til GA**

1. Logg på <a href="https://partnercenter.microsoft.com" target="_blank">Partnersenter</a>.
2. Velg Kunder på **instrumentbordet,** og finn og velg deretter firmanavnet.

    Abonnementene for firmaet vil bli oppført.

    ![Kundens abonnementer i Partnersenter](../../media/pc_customer_subscriptions_1.png)
    
3. Velg Legg til abonnement på **firmaets** **Abonnementer-side.**
4. Velg Small **Business** på Nytt **abonnement-siden,** og velg deretter Microsoft **365 Business** fra listen.
5. Legg til antall lisenser, og velg deretter **Neste: Se** gjennom for å se gjennom abonnementet, og velg deretter **Send inn**.

    ![Se gjennom det nye abonnementet på Microsoft 365 Business](../../media/pc_customer_reviewnewsubscription.png)

    De **lisensbaserte abonnementene** viser **Microsoft 365 Business Preview** og Microsoft **365 Business.** Du stopper forhåndsversjonen av abonnementet.

6. Velg **Microsoft 365 Business Preview**.
7. Velg Utestengt på siden Forhåndsvisning av **Microsoft 365 Business** for **å** stoppe forhåndsversjonen av abonnementet.

    ![Stoppe abonnementet på Microsoft 365 Business Preview](../../media/pc_customer_m365bpreview_suspend.png)

8. Velg **Send for** å bekrefte.

    Bekreft **at forhåndsvisningsstatusen** for **Microsoft 365 Business viser** Deaktivert på Abonnementer-siden. 

    ![Bekreft at statusen for Forhåndsvis abonnement er deaktivert](../../media/pc_customer_m365bpreview_suspend_confirm.png)

9. Du kan også validere lisensavtalen. Dette gjør du slik:
    1. Velg **Brukere og lisenser** fra **firmaets Abonnementer-side.**
    2. Velg en **bruker på** Siden Brukere og lisenser.
    3. Merk av for Tilordne lisenser på **brukerens** side, og bekreft at den viser **Microsoft 365 Business.**

        ![Bekreft at Microsoft 365 Business-lisensen er tilordnet brukeren](../../media/pc_customer_userslicenses_m365b_validate.png)

## <a name="impact-to-customers-and-users-during-and-after-transition"></a>Innvirkning for kunder og brukere under og etter overgangen

Det har ingen innvirkning på kunder og brukere under overgangen og etter overgangen.

## <a name="impact-to-customers-who-dont-transition"></a>Innvirkning på kunder som ikke har overgang

Tabellen nedenfor oppsummerer virkningen for kunder som ikke går over fra et Microsoft 365 Business Preview-abonnement til et Microsoft 365 Business-abonnement.

|       | T-0 til T+30     | T+30 til T+60 | T+60 til T+120 | Utover T+120  |
|-------|-----------------|--------------|---------------|---------------|
| **Tilstand** | I løpeperioden | Utløpt      | Deaktivert      | Deprovisioned |
| **Tjenestepåvirkninger**                                                        |
| **Administrasjonsportal for Microsoft 365 Business** | Ingen innvirkning på funksjonaliteten | Ingen innvirkning på funksjonaliteten | Kan legge til/slette brukere, kjøpe abonnementer.</br> Kan ikke tilordne/oppheve lisenser. | Kundens abonnement og alle data slettes. Administrator kan administrere andre betalte abonnementer. |
| **Office-apper**                         | Ingen innvirkning på sluttbrukeren | Ingen innvirkning på sluttbrukeren | Office går inn i modus for redusert funksjonalitet.</br> Brukere kan bare vise filer. | Office går inn i modus for redusert funksjonalitet.</br> Brukere kan bare vise filer. |
| **Skytjenester (SharePoint Online, Exchange Online, Skype, Teams og mer)** | Ingen innvirkning på sluttbrukeren | Ingen innvirkning på sluttbrukeren | Sluttbrukere og administratorer har ingen tilgang til data i skyen. | Kundens abonnement og alle data slettes. |
| **EM+S-komponenter** | Ingen administratorpåvirkning</br> Ingen innvirkning på sluttbrukeren | Ingen administratorpåvirkning</br> Ingen innvirkning på sluttbrukeren | Funksjonaliteten håndheves ikke lenger.</br> Hvis [du vil ha mer informasjon,](#mobile-device-impacts-upon-subscription-expiration) kan du se Innvirkning på mobilenhet når abonnementet utløper og Windows [10-PC-en](#windows-10-pc-impacts-upon-subscription-expiration) påvirker utløpet av abonnementet. | Funksjonaliteten håndheves ikke lenger.</br> Hvis [du vil ha mer informasjon,](#mobile-device-impacts-upon-subscription-expiration) kan du se Innvirkning på mobilenhet når abonnementet utløper og Windows [10-PC-en](#windows-10-pc-impacts-upon-subscription-expiration) påvirker utløpet av abonnementet. |
| **Windows 10 Business** | Ingen administratorpåvirkning</br> Ingen innvirkning på sluttbrukeren | Ingen administratorpåvirkning</br> Ingen innvirkning på sluttbrukeren | Funksjonaliteten håndheves ikke lenger.</br> Hvis [du vil ha mer informasjon,](#mobile-device-impacts-upon-subscription-expiration) kan du se Innvirkning på mobilenhet når abonnementet utløper og Windows [10-PC-en](#windows-10-pc-impacts-upon-subscription-expiration) påvirker utløpet av abonnementet. | Funksjonaliteten håndheves ikke lenger.</br> Hvis [du vil ha mer informasjon,](#mobile-device-impacts-upon-subscription-expiration) kan du se Innvirkning på mobilenhet når abonnementet utløper og Windows [10-PC-en](#windows-10-pc-impacts-upon-subscription-expiration) påvirker utløpet av abonnementet. |
| **Azure AD-pålogging til en PC med Windows 10** | Ingen administratorpåvirkning</br> Ingen innvirkning på sluttbrukeren | Ingen administratorpåvirkning</br> Ingen innvirkning på sluttbrukeren | Ingen administratorpåvirkning</br> Ingen innvirkning på sluttbrukeren | Når leieren er slettet, kan en bruker bare logge på med lokal legitimasjon. Ta bilde av enheten på nytt hvis det ikke er noen lokal legitimasjon. |

## <a name="mobile-device-impacts-upon-subscription-expiration"></a>Innvirkning på mobilenhet når abonnementet utløper

Tabellen nedenfor oppsummerer innvirkningen på policyene for appbehandling på mobile enheter.

|                            | Fullstendig lisensiert opplevelse                      | T+60 dager etter utløp          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Slette arbeidsfiler fra en inaktiv enhet** | Arbeidsfiler fjernes etter valgte dager | Arbeidsfiler forblir på brukerens personlige enheter |
| **Tvinge brukere til å lagre alle arbeidsfiler til OneDrive for Business** | Arbeidsfiler kan bare lagres i OneDrive for Business | Arbeidsfiler kan lagres hvor som helst |
| **Kryptere arbeidsfiler** | Arbeidsfiler krypteres | Arbeidsfiler krypteres ikke lenger.</br> Sikkerhetspolicyer fjernes, og Office-data på apper fjernes. |
| **Krev PIN-kode eller fingeravtrykk for å få tilgang til Office-apper** | Begrenset tilgang til apper | Ingen tilgangsbegrensning på appnivå |
| **Tilbakestill PIN-kode når påloggingen mislykkes** | Begrenset tilgang til apper | Ingen tilgangsbegrensning på appnivå |
| **Kreve at brukere logger på igjen etter at Office-apper har vært inaktive** | Pålogging kreves | Ingen pålogging kreves |
| **Avslå tilgang til arbeidsfiler på enheter som er jailbreaket eller rootet** | Arbeidsfiler er ikke tilgjengelig på enheter med jailbroken/rooted | Arbeidsfiler kan nås på jailbroken/rooted devices |
| **Tillat brukere å kopiere innhold fra Office-apper til Personlige apper** | Kopier/lim inn begrenset til apper som er tilgjengelige som en del av Microsoft 365-abonnementet | Kopier/lim inn tilgjengelig for alle apper |

## <a name="windows-10-pc-impacts-upon-subscription-expiration"></a>Pc-en med Windows 10 påvirker utløpet av abonnementet

Tabellen nedenfor oppsummerer innvirkningen på konfigurasjonspolicyene for Windows 10-enheter.

|                            | Fullstendig lisensiert opplevelse                      | T+60 dager etter utløp          |
|----------------------------|------------------------------------------------|------------------------------------|
| **Bidra til å beskytte PC-er mot trusler ved hjelp av Windows Defender** | Aktiver/deaktiver er utenfor brukerkontrollen | Bruker kan aktivere/deaktivere Windows Defender på Windows 10-PC-en |
| **Beskytte PC-er fra nettbaserte trusler i Microsoft Edge** | PC-beskyttelse i Microsoft Edge | Bruker kan aktivere/deaktivere PC-beskyttelse i Microsoft Edge |
| **Slå av enhetsskjermen når den er inaktiv** | Administrator definerer policy for intervall for skjermtidsavbrudd | Skjermtidsavbrudd kan konfigureres av sluttbruker |
| **Tillat brukere å laste ned apper fra Microsoft Store** | Administrator definerer om en bruker kan laste ned apper fra Microsoft Store | Brukeren kan laste ned apper fra Microsoft Store når som helst |
| **Gi brukere tilgang til Cortana** | Administrator definerer policy for brukertilgang til Cortana | Brukerenheter for å aktivere/deaktivere Cortana |
| **Tillat brukere å motta tips og annonser fra Microsoft** | Administrator definerer policy for bruker mottar tips og annonser fra Microsoft | Brukeren kan aktivere/deaktivere tips og annonser fra Microsoft |
| **Tillat at brukere kan kopiere innhold fra Office-apper til personlige apper** | Administrator definerer policy for å holde Windows 10-enheter oppdatert | Brukere kan bestemme når windows skal oppdateres |
