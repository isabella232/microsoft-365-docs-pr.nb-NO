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
description: Lær hvordan du bruker Windows AutoPilot til å konfigurere nye Windows 10-enheter for bedriften din slik at de er klare for bruk i ansatte.
ms.openlocfilehash: f263cc90656ae5e7be1a89e3c7f56bfb2d0e3651
ms.sourcegitcommit: 3b369a44b71540c8b8214ce588a7aa6f47c3bb1e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/04/2021
ms.locfileid: "50099754"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Bruk veiledningen som forklarer trinn for trinn hvordan du legger til AutoPilot-enheter og -profil

Du kan bruke Windows AutoPilot til å konfigurere nye **Windows** 10-enheter for bedriften din slik at de er klare til bruk når du gir dem til de ansatte.
  
## <a name="device-requirements"></a>Enhetskrav

Enheter må oppfylle disse kravene:
  
- Windows 10, versjon 1703 eller nyere
    
- Nye enheter som ikke har vært gjennom Windows out-of-box experience
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Bruk installasjonsveiledningen til å opprette enheter og profiler

[![Etikett for å gi deg beskjed om at administrasjonssenteret endres. Du finner mer informasjon på aka.ms/aboutM365preview.](../media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Hvis du ikke har opprettet enhetsgrupper eller profiler ennå, er den beste måten å komme i gang ved hjelp av den trinnvise veiledningen. Du kan også [legge til enheter](create-and-edit-autopilot-devices.md) og tilordne [profiler](create-and-edit-autopilot-profiles.md) til dem uten å bruke veiledningen. 
  
1. Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> på.

2. Velg Enheter AutoPilot  i venstre \> **navigasjonsrute.**

    ![Velg enheter og deretter AutoPilot i administrasjonssenteret.](../media/AutoPilot.png)
  
2. Klikk eller trykk **startveiledningen på AutoPilot-siden.** 
    
    ![Click Start guide for step-by-step instructions for Autopilot.](../media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Bla til et sted der du har den klargjorte, på siden Last opp **CSV-fil** med listen over enheter. CSV-fil, og **deretter Åpne** \> **neste.** Filen må ha tre topptekster:
    
    - Kolonne A: Enhetens serienummer
    
    - Kolonne B: Produkt-ID for Windows
    
    - Kolonne C: Maskinvarens hash
    
    Du kan få denne informasjonen fra leverandøren av maskinvaren, eller du kan bruke [Get-WindowsAutoPilotInfo PowerShell-skriptet](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) til å generere en CSV-fil. 
    
    Se [CSV-fil med enhetsliste](https://docs.microsoft.com/microsoft-365/admin/misc/device-list) hvis du vil ha mer informasjon. Du kan også laste ned en eksempelfil på siden **Laste opp .csv-fil med liste over enheter**. 
    
> [!NOTE]
> Dette skriptet bruker WMI til å hente egenskaper som en kunde trenger for å registrere en enhet med Windows Autopilot. Vær oppmerksom på at det er vanlig at CSV-filen ikke samler inn en Windows-produkt-ID-verdi (PKID), siden dette ikke er nødvendig for å registrere en enhet og at PKID er NULL i utdata-CSV-filen. Bare serienummeret og maskinvare-hash-en fylles ut.
    
4. Du kan **velge en eksisterende profil** eller opprette en ny profil på siden Tilordne en profil. Hvis du ikke har en ennå, blir du bedt om å opprette en. 
    
    En profil er en samling innstillinger som kan brukes på én enkelt enhet eller en gruppe enheter.
    
    Standardfunksjonene er obligatoriske og angis automatisk. Standardfunksjoner er:
    
    - Hopp over Cortana-, OneDrive- og OEM-registrering.
    
    - Opprett påloggingsopplevelse med firmamerket ditt.
    
    - Koble enhetene dine til Azure Active Directory-kontoer, og registrere dem automatisk slik at de administreres av Microsoft 365 Business Premium.
    
    Hvis du vil ha mer informasjon, kan du se [Om innstillinger for AutoPilot-profil.](autopilot-profile-settings.md) 
    
5. De andre innstillingene er **Hopp over personverninnstillinger** og **Ikke tillat brukeren å bli lokal administrator**. Dette er satt til **Av** som standard. 
    
    Velg **Neste**.
    
6. **Når du er ferdig,** indikerer det at profilen du opprettet (eller valgte) blir brukt på enhetsgruppen du opprettet, ved å laste opp listen over enheter. Innstillingene trer i kraft når enhetenes brukere logger på neste gang. Velg **Lukk**.
    
