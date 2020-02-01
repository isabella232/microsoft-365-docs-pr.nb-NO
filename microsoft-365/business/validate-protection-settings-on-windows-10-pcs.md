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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Finn ut hvordan du validerer innstillingene for beskyttelse av Microsoft 365 Business-apper i Windows 10-enheter.
ms.openlocfilehash: 6573519ee2fe2d1eb82545755fa98b8c018e08ff
ms.sourcegitcommit: 1c91b7b24537d0e54d484c3379043db53c1aea65
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2020
ms.locfileid: "41594999"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Validere innstillingene for appbeskyttelse på Windows 10-datamaskiner

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Kontroller at brukere ikke kan kopiere firmadata til personlige filer på bedriftens enheter

Etter at du [har konfigurert policyer for appbeskyttelse](protection-settings-for-windows-10-devices.md), kan det ta opptil noen timer før policyen trer i kraft på brukernes enheter. Hvis du har slått **På** **Hindre brukere i å kopiere firmadata til personlige filer og tvinge dem til å lagre arbeidsfiler i OneDrive for Business-innstillingen** for firmaeide enheter, kan du sjekke dette på brukerens enhet etter at de har koblet til Azure AD og logget på. 
  
 **Bekrefte tilkoblingsinnstillinger**
  
1. After you sign in with Microsoft 365 Business credentials and connect to Azure AD as described in [Set up Windows devices for Microsoft 365 Business users](set-up-windows-devices.md), go to **Windows Settings** \> **Accounts** \> **Access work or school**. Choose **Connected to \<tenant name\> Azure AD**, and then choose **Info**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. På siden **Administrert** \<\> av leiernavn kan du se **tilkoblingsinformasjonen** som inneholder en **Management Server-adresse,** for eksempel den som vises i figuren nedenfor. 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Kontroller at du ikke kan lime inn firmadata i en ikke-administrert app**
  
1. Åpne Outlook 2016 som ble installert av Microsoft 365 Business.
    
2. Åpne en e-postmelding og kopier noe av innholdet fra den.
    
    Åpne Notisblokk, og prøv å lime inn innholdet.
    
    Du får en feilmelding som sier at appen ikke får tilgang til innhold.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Du kan imidlertid lime inn det samme innholdet i Word 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Kontroller at brukere ikke kan kopiere firmadata til personlige filer på personlige enheter

 **Kontrollere tilkoblingsinnstillinger**
  
1. Gå til **Windows-innstillinger**på den personlige enheten for Windows 10 der du er logget på som lokal bruker, og klikk eller trykk **Kontoer** \> **tilgang til arbeid eller skole**.
    
2. Velg **Koble til** under **Få tilgang til jobb eller skole**.
    
3. Skriv inn Microsoft 365 Business legitimasjonen i dialogboksen **Konfigurer en jobb- eller skolekonto** \> **Logg på**.
    
4. Velg **Få tilgang til jobb- eller skolekonto** på siden **Få tilgang til arbeidsplassen eller skolen**, og velg deretter **Informasjon**.
    
    ![Klikk eller trykk på Informasjon i dialogboksen Jobb- eller skolekonto.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. På siden **Access-arbeid eller skole** kan du se **tilkoblingsinformasjonen** som inneholder en **Management Server-adresse** som den som vises i figuren nedenfor, og inneholder ordene *tørke* og *mabene* i. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Kontroller at du ikke kan lime inn firmadata i en ikke-administrert app**
  
1. Åpne Outlook 2016 og legg til Microsoft 365 Business-kontoen hvis nødvendig, og logg på med Microsoft 365 Business-legitimasjonen.
    
2. Åpne en e-postmelding og kopier noe av innholdet fra den.
    
    Åpne Notisblokk, og prøv å lime inn innholdet.
    
    Du får en feilmelding som sier at App ikke får tilgang til innhold.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Du kan imidlertid lime inn det samme innholdet i Word 2016.
    

