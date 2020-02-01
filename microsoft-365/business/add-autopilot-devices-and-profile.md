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
search.appverid:
- BCS160
- MET150
- MOE150
ms.assetid: be5b6d90-3344-4c5e-bf40-5733eb845beb
description: Finn ut hvordan du bruker Windows AutoPilot til å konfigurere nye Windows 10-enheter for bedriften din.
ms.openlocfilehash: 1fd0abb76d16b79dd11ef27b6b27a87894d89ef9
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2020
ms.locfileid: "41593277"
---
# <a name="use-the-step-by-step-guide-to-add-autopilot-devices-and-profile"></a>Bruk veiledningen som forklarer trinn for trinn hvordan du legger til AutoPilot-enheter og -profil

Du kan bruke Windows AutoPilot til å konfigurere **nye** Windows 10-enheter for bedriften, slik at de er klare til bruk når du gir dem til de ansatte.
  
## <a name="device-requirements"></a>Enhetskrav

Enheter må oppfylle disse kravene:
  
- Windows 10, versjon 1703 eller nyere
    
- Nye enheter som ikke har vært gjennom Windows-opplevelsen
    
## <a name="use-the-setup-guide-to-create-devices-and-profiles"></a>Bruk installasjonsveiledningen til å opprette enheter og profiler

[![Etikett for å gi deg beskjed om at administrasjonssenteret endres. Du finner mer informasjon på aka.ms/aboutM365preview.](media/m365admincenterchanging.png)](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview)

Hvis du ikke har opprettet enhetsgrupper eller profiler ennå, er den beste måten å komme i gang på ved å bruke den trinnvise veiledningen. Du kan også [legge til enheter](create-and-edit-autopilot-devices.md) og tilordne [profiler](create-and-edit-autopilot-profiles.md) til dem uten å bruke veiledningen. 
  
1. Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>på .

2. Velg **Enheter** \> **AutoPilot**i navigasjonsruten til venstre.

    ![Velg enheter og deretter AutoPilot i administrasjonssenteret.](media/AutoPilot.png)
  
2. Klikk eller trykk **startveiledning**på **AutoPilot-siden.**
    
    ![Click Start guide for step-by-step instructions for Autopilot.](media/31662655-d1e6-437d-87ea-c0dec5da56f7.png)
  
3. Bla **** til en plassering der du har forberedt . CSV-fil, og **deretter Åpne** \> **Neste**. Filen må ha tre overskrifter:
    
    - Kolonne A: Enhetens serienummer
    
    - Kolonne B: Produkt-ID for Windows
    
    - Kolonne C: Maskinvarens hash
    
    Du kan få denne informasjonen fra maskinvareleverandøren, eller du kan bruke [Get-WindowsAutoPilotInfo PowerShell-skriptet](https://www.powershellgallery.com/packages/Get-WindowsAutoPilotInfo) til å generere en CSV-fil. 
    
    Se [CSV-fil med enhetsliste](https://support.office.com/article/932e3676-2491-49f0-9177-d893d2f5276e) hvis du vil ha mer informasjon. Du kan også laste ned en eksempelfil på siden **Laste opp .csv-fil med liste over enheter**. 
    
4. På **tilordne en profil-siden** kan du enten velge en eksisterende profil eller opprette en ny. Hvis du ikke har en ennå, blir du bedt om å opprette en. 
    
    En profil er en samling innstillinger som kan brukes på én enkelt enhet eller en gruppe enheter.
    
    Standardfunksjonene kreves og angis automatisk. Standardfunksjoner er:
    
    - Hopp over Cortana-, OneDrive- og OEM-registrering.
    
    - Opprett påloggingsopplevelse med firmamerket ditt.
    
    - Koble enhetene dine til Azure Active Directory-kontoer, og registrer dem automatisk for å administreres av Microsoft 365 Business.
    
    Hvis du vil ha mer informasjon, kan du se Om innstillinger for [AutoPilot-profil](autopilot-profile-settings.md). 
    
5. De andre innstillingene er **Hopp over personverninnstillinger** og **Ikke tillat brukeren å bli lokal administrator**. Dette er satt til **Av** som standard. 
    
    Velg **Neste**.
    
6. **Du er ferdig,** og angir at profilen du opprettet (eller valgte) skal brukes på enhetsgruppen du opprettet, ved å laste opp listen over enheter. Innstillingene trer i kraft når enhetsbrukerne logger på neste. Velg **Lukk**.
    