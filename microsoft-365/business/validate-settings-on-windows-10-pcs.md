---
title: Validere innstillinger for appbeskyttelse for Pc-er med Windows 10
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
description: Lær hvordan du kontrollerer at beskyttelsesinnstillingene for Microsoft 365 for business-apper trer i kraft på brukernes Windows 10-enheter.
ms.openlocfilehash: 464a246a0da65dcffeb70946287ce4fa0e67ae7c
ms.sourcegitcommit: be929f79751c0c52dfa6bd98a854432a0c63faf0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/14/2021
ms.locfileid: "52925263"
---
# <a name="validate-device-protection-settings-for-windows-10-pcs"></a>Validere innstillinger for enhetsbeskyttelse for Windows 10-PC-er

## <a name="verify-that-windows-10-device-policies-are-set"></a>Kontroller at windows 10-enhetspolicyer er angitt

Når du [har konfigurert policyer](protection-settings-for-windows-10-pcs.md)for enheter, kan det ta opptil et par timer før policyen trer i kraft på brukernes enheter. Du kan bekrefte at policyene trer i kraft ved å se på ulike Skjermbilder for Windows-innstillinger på brukernes enheter. Fordi brukerne ikke kan endre Windows Update- og Windows Defender Antivirus-innstillingene på Windows 10-enhetene sine, vil mange alternativer være nedtonet.
  
1. Gå til **Innstillinger** \> **Oppdater &amp; sikkerhetsalternativer** \> **for Windows Update Start** på \> **nytt,** og bekreft at alle innstillingene er nedtonet. 
    
    ![Alle alternativene for Omstart er nedtonet.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Gå til **Innstillinger Oppdater** \> **sikkerhet &amp; Windows** \> **Update** \> **Avanserte alternativer** og bekreft at alle innstillingene er nedtonet. 
    
    ![Alternativer for avanserte oppdateringer i Windows er nedtonet.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Gå til **Innstillinger Oppdater** \> **sikkerhet &amp; Windows** \> **Update** \> **Avanserte alternativer** \> **Velg hvordan oppdateringer skal leveres**.
    
    Bekreft at du kan se meldingen (i rødt) om at noen innstillinger er skjult eller administrert av organisasjonen, og at alle alternativene er nedtonet.
    
    ![Velg hvordan oppdateringer leveres-siden angir at innstillingene er skjult eller administrert av organisasjonen.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Hvis du vil åpne Windows Defender Sikkerhetssenter, går du til Innstillinger  Oppdater sikkerhet Windows Defender og klikker Åpne Windows \> **&amp;** \>  \> **Defender Security Center** Virus thread \> **&amp; protection** Virus threat protection \> **&amp; settings**. 
    
5. Kontroller at alle alternativene er nedtonet. 
    
    ![Innstillingene for virus- og trusselbeskyttelse er nedtonet.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Beslektede emner

[Dokumentasjon og ressurser for Microsoft 365 for bedrifter](./index.yml)
  
[Komme i gang med Microsoft 365 for bedrifter](microsoft-365-business-overview.md)
  
[Administrere Microsoft 365 for bedrifter](manage.md)
  
[Angi enhetskonfigurasjoner for PC-er med Windows 10](protection-settings-for-windows-10-pcs.md)
