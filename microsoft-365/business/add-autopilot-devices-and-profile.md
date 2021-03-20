---
title: Bruk veiledningen som forklarer trinn for trinn hvordan du legger til AutoPilot-enheter og -profil
f1.keywords:
- NOCSH
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
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Lær hvordan du bruker Windows AutoPilot til å konfigurere nye Windows 10-enheter for bedriften, slik at de er klare til bruk for ansatte.
ms.openlocfilehash: 75cc51b889f8673de8dba2357c777de47fd0d296
ms.sourcegitcommit: 27b2b2e5c41934b918cac2c171556c45e36661bf
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "50913506"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Bruk veiledningen som forklarer trinn for trinn hvordan du legger til AutoPilot-enheter og -profil

Du kan bruke Windows AutoPilot til å konfigurere nye **Windows** 10-enheter for bedriften, slik at de er klare til bruk når du gir dem til de ansatte.
  
## <a name="device-requirements"></a>Enhetskrav

Enheter må oppfylle disse kravene:
  
- Windows 10, versjon 1703 eller nyere
    
- Nye enheter som ikke har vært gjennom Windows-opplevelsen
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Bruk installasjonsveiledningen til å opprette enheter og profiler

[![Etikett for å gi deg beskjed om at administrasjonssenteret endres. Du finner mer informasjon på aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](/office365/admin/microsoft-365-admin-center-preview)

Hvis du ikke har opprettet enhetsgrupper eller profiler ennå, er den beste måten å komme i gang på ved hjelp av den trinnvise veiledningen. Du kan også [legge til enheter](create-and-edit-autopilot-devices.md) og tilordne [profiler](create-and-edit-autopilot-profiles.md) til dem uten å bruke veiledningen. 
  
1. Gå til administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .

2. Velg Enheter AutoPilot  i den venstre \> **navigasjonsruten.**

    ![Velg enheter i administrasjonssenteret, og velg deretter AutoPilot.](../media/AutoPilot.png)
  
2. Klikk eller **trykk startveiledning på AutoPilot-siden.** 
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Gå til en plassering der du har klargjort , på siden Last opp **CSV-fil** med listen over enheter. CSV-fil, og **deretter Åpne** \> **Neste**. Filen må ha tre overskrifter:
    
    - Kolonne A: Enhetens serienummer
    
    - Kolonne B: Produkt-ID for Windows
    
    - Kolonne C: Maskinvarens hash
    
    Du kan få denne informasjonen fra maskinvareleverandøren, eller du kan bruke [Get-WindowsAutoPilotInfo PowerShell-skriptet](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) til å generere en CSV-fil. 
    
    Se [CSV-fil med enhetsliste](../admin/misc/device-list.md) hvis du vil ha mer informasjon. Du kan også laste ned en eksempelfil på siden **Laste opp .csv-fil med liste over enheter**. 
    
> [!NOTE]
> Dette skriptet bruker WMI til å hente egenskaper som en kunde trenger for å registrere en enhet med Windows Autopilot. Vær oppmerksom på at det er vanlig at CSV-filen ikke samler inn en Windows-produkt-ID (PKID)-verdi siden dette ikke er nødvendig for å registrere en enhet, og PKID som NULL i utdata-CSV er helt greit. Bare serienummeret og maskinvarenummeret fylles ut.
    
4. På siden **Tilordne en profil** kan du enten velge en eksisterende profil eller opprette en ny. Hvis du ikke har en ennå, blir du bedt om å opprette en. 
    
    En profil er en samling innstillinger som kan brukes på én enkelt enhet eller en gruppe enheter.
    
    Standardfunksjonene er obligatoriske og angis automatisk. Standardfunksjoner er:
    
    - Hopp over Cortana-, OneDrive- og OEM-registrering.
    
    - Opprett påloggingsopplevelse med firmamerket ditt.
    
    - Koble enhetene dine til Azure Active Directory-kontoer, og registrere dem automatisk for å bli administrert av Microsoft 365 Business Premium.
    
    Hvis du vil ha mer informasjon, [kan du se Om innstillinger for AutoPilot-profil](autopilot-profile-settings.md). 
    
5. De andre innstillingene er **Hopp over personverninnstillinger** og **Ikke tillat brukeren å bli lokal administrator**. Dette er satt til **Av** som standard. 
    
    Velg **Neste**.
    
6. **Du er ferdig angir** at profilen du opprettet (eller valgte) vil bli brukt på enhetsgruppen du opprettet ved å laste opp listen over enheter. Innstillingene trer i kraft når brukerne av enheten logger på neste gang. Velg **Lukk**.
