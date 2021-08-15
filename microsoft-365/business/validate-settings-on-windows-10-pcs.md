---
title: Validere innstillinger for appbeskyttelse for Windows 10 PC-er
f1.keywords:
- NOCSH
ms.author: sharik
author: skjerland
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Lær hvordan du kontrollerer at Microsoft 365 for bedriftsappbeskyttelse trer i kraft på brukernes Windows 10 enheter.
ms.openlocfilehash: 0b896ae21139adcc425295f31de9232f65380d692a46bd1ef9f81d4516e0e9ec
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53861657"
---
# <a name="validate-device-protection-settings-for-windows-10-pcs"></a>Validere innstillinger for enhetsbeskyttelse for Windows 10 PC-er

## <a name="verify-that-windows-10-device-policies-are-set"></a>Kontroller at Windows 10 er angitt

Når du [har konfigurert policyer](protection-settings-for-windows-10-pcs.md)for enheter, kan det ta opptil et par timer før policyen trer i kraft på brukernes enheter. Du kan bekrefte at policyene trer i kraft ved å se på Windows Innstillinger på brukernes enheter. Fordi brukerne ikke kan endre innstillingene Windows Oppdatering og Windows Defender Antivirus på sine Windows 10 enheter, vil mange alternativer være nedtonet.
  
1. Gå til **Innstillinger** Oppdater sikkerhetsinnstillinger Windows oppdater omstartsalternativene, \> **&amp;** \>  \>  og bekreft at alle innstillingene er nedtonet. 
    
    ![Alle alternativene for Omstart er nedtonet.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Gå til **Innstillinger** oppdater sikkerhetsinnstillingene Windows oppdater avanserte alternativer, og bekreft at alle innstillingene \> **&amp;** \>  \>  er nedtonet. 
    
    ![Windows Avanserte oppdateringsalternativer er nedtonet.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Gå til **Innstillinger** Oppdater \> **&amp; Windows** Alternativer for \>  \>  \> **oppdaterings avansert Velg hvordan oppdateringer skal leveres**.
    
    Bekreft at du kan se meldingen (i rødt) om at noen innstillinger er skjult eller administrert av organisasjonen, og at alle alternativene er nedtonet.
    
    ![Velg hvordan oppdateringer leveres-siden angir at innstillingene er skjult eller administrert av organisasjonen.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Hvis du vil åpne Windows Defender Sikkerhetssenter, kan du gå til Innstillinger Oppdateringssikkerhet  Windows Defender klikk Åpne Windows Defender \> **&amp;** \>  \> **Sikkerhetssenter Virustrådbeskyttelse** \> **&amp;** \> **&amp;** For beskyttelse mot virustrusler . 
    
5. Kontroller at alle alternativene er nedtonet. 
    
    ![Innstillingene for virus- og trusselbeskyttelse er nedtonet.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Beslektede emner

[Microsoft 365 for forretningsdokumentasjon og -ressurser](./index.yml)
  
[Kom i gang med Microsoft 365 for bedrifter](microsoft-365-business-overview.md)
  
[Administrere Microsoft 365 for bedrifter](manage.md)
  
[Angi enhetskonfigurasjoner for PC-er med Windows 10](protection-settings-for-windows-10-pcs.md)
