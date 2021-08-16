---
title: Trusler som oppdages av Microsoft Defender Antivirus
f1.keywords: CSH
ms.author: sharik
author: SKjerland
manager: scotv
audience: Admin
ms.topic: conceptual
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- Adm_O365
- Adm_TOC
ms.custom: AdminSurgePortfolio
search.appverid: MET150
description: Lær hvordan Microsoft Defender Antivirus beskytter Windows enheter mot programvaretrusler, for eksempel virus, skadelig programvare og spionprogrammer.
ms.openlocfilehash: 79ec44a44c3939a4a868b98d75ab4f24eaf949fcd9bbafb7c0a3173e267f4680
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53896307"
---
# <a name="threats-detected-by-microsoft-defender-antivirus"></a>Trusler som oppdages av Microsoft Defender Antivirus

Microsoft Defender Antivirus beskytter Windows-enheter mot programvaretrusler, for eksempel virus, skadelig programvare og spionprogrammer.

- Virus spres vanligvis ved å legge ved koden til andre filer på enheten eller nettverket, og kan føre til at infiserte programmer fungerer feil.
- Skadelig programvare omfatter skadelige filer, programmer og kode som kan forårsake skade og forstyrre normal bruk av enheter. Skadelig programvare kan også tillate uautorisert tilgang, bruke systemressurser, stjele passord og kontoinformasjon, låse deg ute av datamaskinen og be om løsepenger og mer.
- Spionprogrammer samler inn data, for eksempel nettlesingsaktivitet, og sender dataene til eksterne servere.
 
For å gi trusselbeskyttelse bruker Microsoft Defender Antivirus flere metoder. Disse metodene omfatter skybasert beskyttelse, sanntidsbeskyttelse og dedikerte beskyttelsesoppdateringer.

- Skybasert beskyttelse bidrar til å gi umiddelbar gjenkjenning og blokkering av nye og fremvoksende trusler.
- Skanning som alltid er på, bruker overvåking av fil- og prosessatferd og andre teknikker (også kjent *som sanntidsbeskyttelse).*
- Dedikerte beskyttelsesoppdateringer er basert på maskinlæring, menneskelig og automatisert stordataanalyse og grundig forskning på trusselmotstand. 

Hvis du vil lære mer om skadelig Microsoft Defender Antivirus, kan du se følgende artikler: 

- [Forstå skadelig programvare & andre trusler](/windows/security/threat-protection/intelligence/understanding-malware)
- [Slik identifiserer Microsoft skadelig programvare og potensielt uønskede programmer](/windows/security/threat-protection/intelligence/criteria)
- [Neste generasjons beskyttelse i Windows 10](/windows/security/threat-protection/microsoft-defender-antivirus/microsoft-defender-antivirus-in-windows-10)

## <a name="what-happens-when-a-non-microsoft-antivirus-solution-is-used"></a>Hva skjer når en antivirusløsning fra andre enn Microsoft brukes? 

Microsoft Defender Antivirus er en del av operativsystemet og er aktivert på enheter som kjører Windows 10. Hvis du imidlertid bruker en antivirusløsning som ikke er fra Microsoft, og du ikke bruker [Microsoft Defender for](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-advanced-threat-protection)endepunkt, går Microsoft Defender Antivirus automatisk i deaktivert modus.  

Når de er i deaktivert modus, kan brukere og kunder fortsatt bruke Microsoft Defender Antivirus for planlagte eller behovskrevne skanninger for å identifisere trusler; Men Microsoft Defender Antivirus ikke lenger:

- brukes som standard antivirusapp.
- aktivt skanne filer etter trusler.
- utbedre eller løse trusler.

Hvis du avinstallerer antivirusløsningen som ikke er fra Microsoft, går Microsoft Defender Antivirus automatisk i aktiv modus for å beskytte Windows enheter mot trusler.

> [!TIP]
> - Hvis du bruker Microsoft 365, bør du vurdere å Microsoft Defender Antivirus som primær antivirusløsning. Integrering kan gi bedre beskyttelse. Se [Bedre sammen: Microsoft Defender Antivirus og Office 365](/windows/security/threat-protection/microsoft-defender-antivirus/office-365-microsoft-defender-antivirus).
> - Pass på at du Microsoft Defender Antivirus oppdatert, selv om du bruker en antivirusløsning som ikke er fra Microsoft.

## <a name="what-to-expect-when-threats-are-detected"></a>Hva du kan forvente når trusler oppdages

Når trusler oppdages av Microsoft Defender Antivirus, skjer følgende:

- Brukere mottar [varsler i Windows](https://support.microsoft.com/windows/8942c744-6198-fe56-4639-34320cf9444e). 
- Gjenkjenninger er oppført i [Windows Sikkerhet-appen](/windows/security/threat-protection/windows-defender-security-center/windows-defender-security-center) på **beskyttelsesloggsiden.**  
- Hvis du har sikret [Windows 10-enhetene](secure-win-10-pcs.md) og registrert dem i  [Intune](/mem/intune/enrollment/windows-enrollment-methods), og organisasjonen har registrert 800 eller færre enheter, ser du trusselgjenkjenninger og innsikt i <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">Administrasjonssenter for Microsoft 365</a> på siden Trusler og antivirus, som du kan få tilgang til fra **Microsoft Defender Antivirus-kortet** på hjemmesiden (eller fra navigasjonsruten ved å velge **Helsetrusler**  >  **& antivirus**).

    Hvis organisasjonen har mer enn 800 enheter registrert i Intune, blir du bedt om å vise trusselgjenkjenninger og innsikter fra [Microsoft Endpoint Manager](/mem/endpoint-manager-overview) i stedet for fra siden Trusler og **antivirus.**
 
    > [!NOTE]
    > Siden **Microsoft Defender Antivirus** og Trusler og **antivirus rulles** ut i faser, så du har kanskje ikke umiddelbar tilgang til dem.

I de fleste tilfeller trenger ikke brukerne å gjøre noe mer. Så snart en ondsinnet fil eller et program oppdages på en enhet, blokkerer Microsoft Defender Antivirus den og hindrer den i å kjøre. I tillegg legges nylig oppdagede trusler til antivirus- og beskyttelsesmotoren slik at også andre enheter og brukere er beskyttet.  

Hvis det er en handling en bruker må gjøre, for eksempel godkjenne fjerning av en ondsinnet fil, ser de dette i varselet de mottar. Hvis du vil lære mer om Microsoft Defender Antivirus som utføres på en brukers vegne, eller handlinger som brukere må utføre, kan du se [Beskyttelseslogg](https://support.microsoft.com/office/f1e5fd95-09b4-46d1-b8c7-1059a1e09708). Hvis du vil lære hvordan du administrerer trusselgjenkjenning som IT-tekniker/administrator, kan du se Se gjennom [oppdagede trusler og gjøre noe.](review-threats-take-action.md)

Hvis du vil lære mer om ulike trusler, <a href="https://www.microsoft.com/wdsi/threats" target="_blank">kan du gå til Microsoft Sikkerhetsintelligens trusselnettstedet</a>, der du kan utføre følgende handlinger: 

- Vis gjeldende informasjon om de største truslene.
- Vis de nyeste truslene for et bestemt område.
- Søk i trusselens leksikon for mer informasjon om en bestemt trussel.

## <a name="related-content"></a>Beslektet innhold

[Sikre Windows 10 enheter](secure-windows-10-devices.md) (artikkel)\
[Evaluer Microsoft Defender Antivirus](/windows/security/threat-protection/microsoft-defender-antivirus/evaluate-microsoft-defender-antivirus) (artikkel)\
[Slik aktiverer du antivirusbeskyttelse i sanntid](/mem/intune/user-help/turn-on-defender-windows#turn-on-real-time-and-cloud-delivered-protection) og skybasert antivirusbeskyttelse (artikkel)\
[Slik aktiverer og bruker du Microsoft Defender Antivirus fra](/windows/security/threat-protection/microsoft-defender-antivirus/microsoft-defender-security-center-antivirus) Windows Sikkerhet (artikkel)\
[Slik aktiverer du Microsoft Defender Antivirus ved hjelp av gruppepolicy](/mem/intune/user-help/turn-on-defender-windows#turn-on-windows-defender) (artikkel)\
[Slik oppdaterer du antivirusdefinisjonene](/mem/intune/user-help/turn-on-defender-windows#update-your-antivirus-definitions) (artikkel)\
[Slik sender du inn skadelig programvare og skadelig programvare til Microsoft for analyse](/microsoft-365/security/office-365-security/submitting-malware-and-non-malware-to-microsoft-for-analysis) (artikkel)
