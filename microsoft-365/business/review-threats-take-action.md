---
title: Se gjennom oppdagede trusler og gjør noe
f1.keywords: NOCSH
ms.author: sharik
author: SKjerland
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- Adm_O365
- Adm_TOC
ms.custom: AdminSurgePortfolio
search.appverid: MET150
description: Lær hvordan du går gjennom og administrerer trusler som oppdages Microsoft Defender Antivirus på Windows 10 enheter.
ms.openlocfilehash: 15e99fb75e4a3ac1af842ca7d0b900e02cbc6bd4
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "53465429"
---
# <a name="review-detected-threats-and-take-action"></a>Se gjennom oppdagede trusler og gjør noe

Så snart en ondsinnet fil eller programvare oppdages, Microsoft Defender Antivirus den og hindrer den i å kjøre. Og med skyleveringsbeskyttelse aktivert, legges nylig oppdagede trusler til antivirus- og beskyttelsesmotoren, slik at de andre enhetene og brukerne også er beskyttet.

Microsoft Defender Antivirus oppdager og beskytter mot følgende typer trusler:

- Virus, skadelig programvare og nettbaserte trusler på enheter
- Phishing-forsøk
- Datatyveriforsøk

Som IT-tekniker/administrator kan du vise informasjon om gjenkjenning av trusler på Windows 10 enheter som er registrert i [Intune](/mem/intune/enrollment/device-enrollment) i Administrasjonssenter for Microsoft 365. Du ser sammendragsinformasjon, for eksempel:

- Hvor mange enheter trenger antivirusbeskyttelse
- Hvor mange enheter er ikke i samsvar med sikkerhetspolicyer
- Hvor mange trusler er aktive, begrensede eller løste for øyeblikket

Du har flere alternativer for å vise spesifikk informasjon om gjenkjenning av trusler og enheter:

- Aktive **enheter-siden** i <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">Administrasjonssenter for Microsoft 365</a>. Se [Behandle trusselgjenkjenninger på Aktive enheter-siden](#manage-threat-detections-on-the-active-devices-page) i denne artikkelen.
- Aktive **trusler-siden** i <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">Administrasjonssenter for Microsoft 365</a>. Se [Administrere trusselgjenkjenning på Aktive trusler-siden](#manage-threat-detections-on-the-active-threats-page) i denne artikkelen.
- **Antivirus-siden** i <a href="https://go.microsoft.com/fwlink/p/?linkid=2150463" target="_blank">Microsoft Endpoint Manager</a>. Se [Administrere trusselgjenkjenning i Microsoft Endpoint Manager](#manage-threat-detections-in-microsoft-endpoint-manager) i denne artikkelen.

Hvis du vil ha mer informasjon, kan [du se Trusler som oppdages av Microsoft Defender Antivirus](threats-detected-defender-av.md).

## <a name="manage-threat-detections-on-the-active-devices-page"></a>Administrere trusselgjenkjenning på **Aktive enheter-siden**

Fremgangsmåten nedenfor gjelder for kunder som har Microsoft 365 Business Premium.

1. Gå til Administrasjonssenter for Microsoft 365 <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> på, og logg på.

2. Velg Enheter aktive enheter på  >  **navigasjonssiden.** Du ser en liste over aktive enheter og detaljer, for eksempel beskyttelsesstatus, beskyttelsesstatus for antivirus (AV) og antall aktive trusler som oppdages.

3. Velg en enhet for å vise flere detaljer om denne enheten og tilgjengelige handlinger. En undermeny åpnes med anbefalinger og tilgjengelige handlinger, for eksempel Oppdateringspolicy, **Oppdater antivirus,** Kjør hurtigskanning, Kjør **full** skanning og mer.

## <a name="manage-threat-detections-on-the-active-threats-page"></a>Administrere trusseldeteksjoner på **Aktive trusler-siden**

Fremgangsmåten nedenfor gjelder for kunder som har Microsoft 365 Business Premium. [Windows 10-enheter må være sikret](./secure-win-10-pcs.md) og [registrert i Intune](/mem/intune/enrollment/windows-enrollment-methods).

> [!NOTE]
> Siden **Microsoft Defender Antivirus** og Aktive trusler **rulles** ut i faser, så du har kanskje ikke umiddelbar tilgang til dem.

1. Gå til Administrasjonssenter for Microsoft 365 <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> på, og logg på.

2. Velg **Microsoft Defender Antivirus** aktive trusler **på** kortet . (Alternativt kan du velge Tilstand i **navigasjonsruten**  >  **Trusler & antivirus**.)

3. Velg en **oppdaget trussel** på Aktive trusler-siden for å lære mer om den. En undermeny åpnes med detaljer om denne trusselen, inkludert hvilke enheter som berøres.

4. Velg en enhet på undermenyen for å vise tilgjengelige handlinger, for eksempel Oppdateringspolicy, **Oppdater antivirus,** **Kjør hurtigskanning** og mer.

## <a name="actions-you-can-take"></a>Handlinger du kan utføre

Når du viser detaljer om bestemte trusler eller enheter, ser du anbefalinger og én eller flere handlinger du kan utføre. Tabellen nedenfor beskriver handlinger som du kan se.<br><br>

| Handling | Beskrivelse |
|--|--|
| Konfigurere beskyttelse | Policyene for trusselbeskyttelse må konfigureres. Velg koblingen for å gå til konfigurasjonssiden for policyen.<br><br>Trenger du hjelp? Se [Administrere enhetssikkerhet med sikkerhetspolicyer for endepunkt i Microsoft Intune](/mem/intune/protect/endpoint-security-policy). |
| Oppdater policy | Antivirus- og sanntidsbeskyttelsespolicyene må oppdateres eller konfigureres. Velg koblingen for å gå til konfigurasjonssiden for policyen.<br><br>Trenger du hjelp? Se [Administrere enhetssikkerhet med sikkerhetspolicyer for endepunkt i Microsoft Intune](/mem/intune/protect/endpoint-security-policy). |
| Kjør hurtigskanning | Starter en rask antivirusskanning på enheten, med fokus på vanlige steder der skadelig programvare kan være registrert, for eksempel registernøkler og kjente Windows oppstartsmapper. |
| Kjør full skanning | Starter en fullstendig antivirusskanning på enheten, med fokus på vanlige plasseringer der skadelig programvare kan være registrert, og inkludert alle filer og mapper på enheten. Resultatene sendes til [Microsoft Endpoint Manager](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager). |
| Oppdatere antivirus | Krever at enheten får [sikkerhetsintelligensoppdateringer](https://go.microsoft.com/fwlink/?linkid=2149926) for antivirus- og beskyttelse mot skadelig programvare. |
| Start enheten på nytt | Tvinger en Windows 10 til å starte på nytt innen fem minutter.<br><br>**VIKTIG:** Eieren eller brukeren av enheten varsles ikke automatisk om omstarten og kan miste ulagret arbeid. |

## <a name="manage-threat-detections-in-microsoft-endpoint-manager"></a>Administrer trusseldeteksjoner i Microsoft Endpoint Manager

Du kan bruke Microsoft Endpoint Manager til å administrere trusselgjenkjenninger. Windows 10-enheter må være [registrert i Intune](/mem/intune/enrollment/windows-enrollment-methods) (en del av Microsoft Endpoint Manager).

1. Gå til Microsoft Endpoint Manager administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=2150463" target="_blank">https://endpoint.microsoft.com</a> på, og logg på.

2. Velg Endepunktsikkerhet i **navigasjonsruten.**

3. Velg **Antivirus** under **Behandle**. Du ser flere faner, for eksempel **Sammendrag,** Windows 10 usunne endepunkter **og** Windows 10 oppdaget **skadelig programvare.**

4. Se gjennom informasjonen på de tilgjengelige fanene, og gjør deretter eventuelle nødvendige handlinger.

Anta for eksempel at enheter er oppført på fanen Windows 10 **oppdaget skadelig** programvare. Når du velger en enhet, har du visse handlinger tilgjengelige, for eksempel Start på **nytt,** Hurtigskanning,  **Full** **skanning,** Synkroniser eller Oppdater **signaturer**. Velg en handling for denne enheten.

Tabellen nedenfor beskriver handlingene du kan se i Microsoft Endpoint Manager.<br><br>

| Handling | Beskrivelse |
|--|--|
| Start på nytt | Tvinger en Windows 10 til å starte på nytt innen fem minutter.<br><br>**VIKTIG:** Eieren eller brukeren av enheten varsles ikke automatisk om omstarten og kan miste ulagret arbeid. |
| Hurtigskanning | Starter en rask antivirusskanning på enheten, med fokus på vanlige steder der skadelig programvare kan være registrert, for eksempel registernøkler og kjente Windows oppstartsmapper. Resultatene sendes til [Microsoft Endpoint Manager](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager). |
| Full skanning | Starter en fullstendig antivirusskanning på enheten, med fokus på vanlige plasseringer der skadelig programvare kan være registrert, og inkludert alle filer og mapper på enheten. Resultatene sendes til [Microsoft Endpoint Manager](/mem/intune/fundamentals/tutorial-walkthrough-endpoint-manager). |
| Synkroniser | Krever at en enhet sjekker inn med Intune (en del av Microsoft Endpoint Manager). Når enheten sjekker inn, mottar enheten eventuelle ventende handlinger eller policyer som er tilordnet enheten. |
| Oppdatere signaturer | Krever at enheten får [sikkerhetsintelligensoppdateringer](https://go.microsoft.com/fwlink/?linkid=2149926) for antivirus- og beskyttelse mot skadelig programvare. |

> [!TIP]
> Hvis du vil ha mer informasjon, kan [du se Eksterne handlinger for enheter](/mem/intune/protect/endpoint-security-manage-devices#remote-actions-for-devices).

## <a name="how-to-submit-a-file-for-malware-analysis"></a>Slik sender du inn en fil for analyse av skadelig programvare

Hvis du har en fil som du tror ble gått glipp av eller feilaktig klassifisert som skadelig programvare, kan du sende inn filen til Microsoft for analyse av skadelig programvare. Brukere og IT-administratorer kan sende inn en fil for analyse. Gå [https://www.microsoft.com/wdsi/filesubmission](https://www.microsoft.com/wdsi/filesubmission) til .