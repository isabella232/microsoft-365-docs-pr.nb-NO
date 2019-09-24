---
title: Bruk veiledningen som forklarer trinn for trinn hvordan du legger til AutoPilot-enheter og -profil
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection:
- M365-subscription-management
- M365-identity-device-management
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Finn ut hvordan du bruker Windows AutoPilot til å konfigurere nye Windows 10-enheter for bedriften din.
ms.openlocfilehash: ee4b4a9b06c08b8f9456822b680542665c27baf3
ms.sourcegitcommit: 7690c8bfdea6e6d245cfa7c5b09b913b092cde0a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/23/2019
ms.locfileid: "37121202"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Bruk veiledningen som forklarer trinn for trinn hvordan du legger til AutoPilot-enheter og -profil

Du kan bruke Windows AutoPilot til å konfigurere **nye** Windows 10-enheter for bedriften din, slik at de er klare for produktiv bruk så snart du gir dem til de ansatte.
  
## <a name="device-requirements"></a>Enhetskrav

Enheter må oppfylle disse kravene:
  
- Windows 10 versjon 1703 eller senere.
    
- Nye enheter som ikke har vært gjennom Windows out-of-box experience.
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Bruk installasjonsveiledningen til å opprette enheter og profiler

[![Label å fortelle deg at Administrasjonssenteret er i endring, og du kan finne mer informasjon på aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Hvis du ikke har opprettet noen enhetsgrupper eller profiler ennå, er den beste måten å komme i gang ved hjelp av den trinnvise veiledningen, men du kan også [legge til enheter](create-and-edit-autopilot-devices.md) og [tilordne profiler](create-and-edit-autopilot-profiles.md) til dem uten å bruke veiledningen. 
  
1. Gå til administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.

2. På venstre NAV velger **Devices** \> **autopilot**.

    ![I administrasjonssenteret velger du enheter og deretter AutoPilot.](media/AutoPilot.png)
  
2. Klikk eller trykk på **Start veiledning**på **autopilot** -siden.
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Bla til der du har den klargjorte CSV-filen på siden **Last opp .csv-fil med en liste over enheter**, og velg **Åpne** \> **Neste**. Filen skal ha tre topptekster:
    
  - Kolonne A: Enhetens serienummer
    
  - Kolonne B: Produkt-ID for Windows
    
  - Kolonne C: Maskinvarens hash
    
    Du får denne informasjonen fra leverandøren av maskinvaren, eller du kan bruke [Get-WindowsAutoPilotInfo PowerShell-skriptet](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo), som genererer en CSV-fil. 
    
    Se [CSV-fil med enhetsliste](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) hvis du vil ha mer informasjon. Du kan også laste ned en eksempelfil på siden **Laste opp .csv-fil med liste over enheter**. 
    
4. Du kan velge en eksisterende profil, eller du kan lage en ny profil, på siden **Tilordne en profil**. Hvis du ikke har en ennå, vil du bli bedt om å opprette en ny. 
    
    En profil er en samling innstillinger som kan brukes på én enkelt enhet eller en gruppe enheter.
    
    Standardfunksjoner er påkrevd, og angis automatisk. Standardfunksjoner er:
    
  - Cortana-, OneDrive- og OEM-registrering hoppes over.
    
  - Opprett påloggingsopplevelse med firmamerket ditt.
    
  - Enhetene dine skal bli koblet til kontoer for Azure Active Directory, og automatisk registrert for å administreres av Microsoft 365 Business.
    
    Hvis du vil ha mer informasjon, kan du se
    
    [Om innstillinger for AutoPilot-profil](autopilot-profile-settings.md) . 
    
5. De andre innstillingene er **Hopp over personverninnstillinger** og **Ikke tillat brukeren å bli lokal administrator**. Dette er satt til **Av** som standard. 
    
    Velg **Neste**.
    
6. Siden **Du er ferdig** indikerer at profilen du opprettet (eller valgte) brukes på den enhetsgruppen du opprettet, ved å laste opp på listen over enheter. Disse innstillingene blir aktive når enhetenes brukere senere logger på. Velg **Lukk**.
    