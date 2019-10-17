---
title: Validere innstillingene for appbeskyttelse på Windows 10-datamaskiner
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- Adm_O365
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Lær hvordan du validerer innstillinger for Microsoft 365 for Business-app i Windows 10-enheter.
ms.openlocfilehash: 5fed2278856f40233b142d3c7c4bc623e3777799
ms.sourcegitcommit: bd52f7b662887f552f90c46f69d6a2a42fb66914
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/17/2019
ms.locfileid: "37575472"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Validere innstillinger for enhetsbeskyttelse på Windows 10-PCer

## <a name="verify-that-windows-10-device-policies-are-set"></a>Kontroller at enhets policyene for Windows 10 er angitt

Når du har [konfigurert retningslinjer for enheter](protection-settings-for-windows-10-pcs.md), kan det ta noen timer for policyen å tre i kraft på brukernes enheter. Du kan bekrefte at policyene trer i kraft ved å se på forskjellige Windows Settings-skjermer på brukernes enheter. Fordi det brukernes wont ' være i stand til endre det Vinduer oppdatere og Vinduer Forsvare antivirus innfatningene opp på deres Vinduer 10 anordninger, en masse dem valgmulighetene ville være grå ut.
  
1. Gå til **innfatningene** \> **oppdatere &amp; garanti** \> **Vinduer oppdatere** \> **hvile valgmulighetene** og anerkjenne det alle innfatningene er grå ut. 
    
    ![Alle hvile valgmulighetene er grå ut.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Gå til **innfatningene** \> **oppdatere &amp; garanti** \> **Vinduer oppdatere** \> **Avansert Valgmulighetene** og anerkjenne det alle innfatningene er grå ut. 
    
    ![Vinduer avansert oppdaterer valgmulighetene er alle grå ut.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Gå til **Innstillinger** \> **Oppdater &amp; sikkerhet** \> **Windows Update** \> **Avanserte alternativer** \> **Velg hvordan oppdateringer skal leveres**.
    
    Bekreft at du kan se meldingen (i rødt) at noen innstillinger er skjult eller administrert av organisasjonen, og at alle alternativene er nedtonet.
    
    ![Velg hvordan oppdateringer leveres siden, angir at innstillingene er skjult eller administrert av organisasjonen.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Hvis du vil åpne Windows Defender Sikkerhetssenter, gå **til innstillinger** \> ** &amp; oppdatere sikkerhet** \> \> **Windows Defender** Klikk **åpne Windows Defender Sikkerhetssenter** \> **virus &amp; tråd ** \> **Innstillinger for &amp; beskyttelse virus trusselbeskyttelse**. 
    
5. Kontroller at alle alternativene er nedtonet. 
    
    ![Innstillingene for virus-og trusselbeskyttelse er nedtonet.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Beslektede emner

[Microsoft 365 Business dokumentasjon og ressurser](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Komme i gang med Microsoft 365 Business](microsoft-365-business-overview.md)
  
[Administrere Microsoft 365 Business](manage.md)
  
[Angi enhetskonfigurasjoner for PC-er med Windows 10](protection-settings-for-windows-10-pcs.md)
  

