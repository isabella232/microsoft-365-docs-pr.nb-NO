---
title: Validere innstillingene for appbeskyttelse på Windows 10-datamaskiner
f1.keywords:
- NOCSH
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
- MARVEL_SEO_MAR
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Finn ut hvordan du kontrollerer at innstillingene for beskyttelse av Microsoft 365 Business-apper trådte i kraft på brukernes Windows 10-enheter.
ms.openlocfilehash: 1b661b41a8042e81f653463cbd32fc6bf6428b53
ms.sourcegitcommit: 26e4d5091583765257b7533b5156daa373cd19fe
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/06/2020
ms.locfileid: "42549961"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Validere innstillinger for enhetsbeskyttelse på Windows 10-PCer

## <a name="verify-that-windows-10-device-policies-are-set"></a>Kontroller at enhetspolicyer for Windows 10 er angitt

Når du [har konfigurert policyer](protection-settings-for-windows-10-pcs.md)for enheter , kan det ta opptil noen timer før retningslinjene trer i kraft på brukernes enheter. Du kan bekrefte at policyene trådte i kraft ved å se på ulike Windows-innstillinger-skjermbilder på brukernes enheter. Fordi brukerne ikke kan endre innstillingene for Windows Update og Windows Defender Antivirus på Windows 10-enhetene sine, blir mange alternativer nedtonet.
  
1. Gå til **Alternativer for omstart** \> av innstillinger **oppdatering av &amp; ** \> **Windows Update** \> **pånytt,** og bekreft at alle innstillingene er nedtonet. 
    
    ![Alle omstart-alternativene er nedtonet.](../media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Gå til **Innstillinger** \> **Update sikkerhet &amp; ** \> **Windows Update** \> Avanserte **alternativer** og bekreft at alle innstillingene er nedtonet. 
    
    ![Alternativer for Avanserte oppdateringer i Windows er alle nedtonet.](../media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Gå til **Innstillinger** \> **Oppdatering sikkerhet &amp; ** \> **Windows Update** \> **Avanserte alternativer** \> **Velg hvordan oppdateringer leveres**.
    
    Bekreft at du kan se meldingen (i rødt) at noen innstillinger er skjult eller administrert av organisasjonen, og at alle alternativene er nedtonet.
    
    ![Velg hvordan oppdateringer skal leveres siden angir at innstillingene er skjult eller administrert av organisasjonen.](../media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. Hvis du vil åpne Sikkerhetssenter for Windows Defender, går du til **Innstillinger** \> **Oppdateringssikkerhet &amp; ** \> **Windows Defender** \> klikk Åpne Windows Defender Security **Center** \> **Virus &amp; trådbeskyttelse** \> ** &amp; Virus trusselbeskyttelse**. 
    
5. Kontroller at alle alternativene er nedtonet. 
    
    ![Innstillingene for virus- og trusselbeskyttelse er nedtonet.](../media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Beslektede emner

[Microsoft 365 Business dokumentasjon og ressurser](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Komme i gang med Microsoft 365 Business](microsoft-365-business-overview.md)
  
[Administrere Microsoft 365 Business](manage.md)
  
[Angi enhetskonfigurasjoner for PC-er med Windows 10](protection-settings-for-windows-10-pcs.md)
  

