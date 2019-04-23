---
title: Validere innstillingene for appbeskyttelse på Windows 10-datamaskiner
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
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
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Lær hvordan du validerer Microsoft 365 Business app innstillinger i Windows 10 enheter.
ms.openlocfilehash: 5ab91d65fa7bd40ebc118df217c9711b7bbfe7a4
ms.sourcegitcommit: 81273a9df49647286235b187fa2213c5ec7e8b62
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32286758"
---
# <a name="validate-device-protection-settings-on-windows-10-pcs"></a>Valider beskyttelse enhetsinnstillinger i Windows PC-10

## <a name="verify-that-windows-10-device-policies-are-set"></a>Kontroller at retningslinjer for Windows 10-enheten er satt

Når du [definerer policyer for enheter](protection-settings-for-windows-10-pcs.md), kan det ta et par timer for policyen trer i kraft på brukernes enheter. Du kan bekrefte at policyene tok effekt ved å se på ulike innstillinger for Windows-skjermer på brukernes enheter. Fordi brukere vil ikke kunne endre innstillingene for Windows Update og Windows Defender Antivirus på Windows 10 enheter, mange av disse alternativene valgbar.
  
1. Gå til **Innstillinger for** \> **oppdatering &amp; sikkerhet** \> **Windows Update** \> **Alternativer for omstart** , og Bekreft at alle innstillingene er grået ut. 
    
    ![Alle alternativer for omstart er grået ut.](media/31308da9-18b0-47c5-bbf6-d5fa6747c376.png)
  
2. Gå til **Innstillinger for** \> **oppdatering &amp; sikkerhet** \> **Windows Update** \> **Avanserte alternativer** , og Bekreft at alle innstillingene er grået ut. 
    
    ![Windows avanserte alternativer for oppdateringer er grået ut.](media/049cf281-d503-4be9-898b-c0a3286c7fc2.png)
  
3. Gå til **Innstillinger for** \> **oppdatering &amp; sikkerhet** \> **Windows Update** \> **Avanserte alternativer** \> **Velg hvordan oppdateringer leveres**.
    
    Bekreft at du kan se meldingen (i rødt) som noen av innstillingene er skjult eller administrert av organisasjonen, og alle alternativene er grået ut.
    
    ![Velg hvordan oppdateringer leveres siden angir innstillingene er skjult eller administrert av organisasjonen.](media/6b3e37c5-da41-4afd-9983-b4f406216b59.png)
  
4. For å åpne Sikkerhetssenter for Windows Defender, kan du gå til **Innstillinger for** \> **oppdatering &amp; sikkerhet** \> **Windows Defender** \> Klikk **Åpne Sikkerhetssenter i Windows Defender** \> **Virus &amp; tråd beskyttelse mot** \> **Virus &amp; trusselen beskyttelsesinnstillingene**. 
    
5. Kontroller at alle alternativene er grået ut. 
    
    ![Innstillingene for Virus og threat protection er grået ut.](media/9ca68d40-a5d9-49d7-92a4-c581688b5926.png)
  
## <a name="related-topics"></a>Beslektede emner

[Microsoft 365 Business dokumentasjon og ressurser](https://go.microsoft.com/fwlink/p/?linkid=853701)
  
[Komme i gang med Microsoft 365 Business](microsoft-365-business-overview.md)
  
[Administrere Microsoft 365 Business](manage.md)
  
[Angi enhetskonfigurasjoner for PC-er med Windows 10](protection-settings-for-windows-10-pcs.md)
  

