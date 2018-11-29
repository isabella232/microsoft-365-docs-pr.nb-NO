---
title: Validere innstillingene for appbeskyttelse på Windows 10-datamaskiner
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Lær hvordan du validerer Microsoft 365 Business app innstillinger i Windows 10 enheter.
ms.openlocfilehash: f00dd380103ad9498d77b0e8814bace3de168df4
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983296"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Validere innstillingene for appbeskyttelse på Windows 10-datamaskiner

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Kontroller at brukere ikke kan kopiere firmadata til personlige filer på bedriftens enheter

Etter at du [har konfigurert policyer for appbeskyttelse](protection-settings-for-windows-10-devices.md), kan det ta opptil noen timer før policyen trer i kraft på brukernes enheter. Hvis du har slått **På** innstillingen **Hindre brukere i å kopiere firmadata til personlige filer, og tving dem til å lagre arbeidsfiler på OneDrive for Business** for firmaeide enheter, kan du kontrollere dette på brukernes enheter etter de har koblet til Azure AD og logget seg på. 
  
 **Kontrollere tilkoblingsinnstillinger**
  
1. Når du logger på med legitimasjon for Microsoft 365 Business og koble til Azure AD som beskrevet i [konfigurere Windows-enheter for forretningsbrukere som Microsoft 365](set-up-windows-devices.md), gå til **Innstillinger for Windows** \> **kontoer** \> **Access arbeid eller skole **. Velg **koblet til \<leier navn\> Azure AD**, og velg deretter **informasjon**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. Du kan se **Tilkoblingsinformasjon** på \< \>tenant name****-siden som inneholder en **Adresse for administrasjonsserver**, som illustrert i denne figuren. 
    
    ![Managed by page shows connection info of the device manager URL.](media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Kontroller at du ikke kan lime inn firmadata til en ikke-administrert app**
  
1. Åpne Outlook 2016 som ble installert av Microsoft 365 Business.
    
2. Åpne en e-postmelding og kopier noe av innholdet fra den.
    
    Åpne Notisblokk, og prøv å lime inn innholdet.
    
    Du får en feilmelding som sier at appen ikke får tilgang til innholdet.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Du kan imidlertid lime inn det samme innholdet i Word 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Kontroller at brukere ikke kan kopiere firmadata til personlige filer på personlige enheter

 **Kontrollere tilkoblingsinnstillinger**
  
1. Gå til **Windows-innstillinger**, og klikk eller trykk på **Kontoer** \> **Få tilgang til jobb eller skole** på den personlige Windows 10-enheten, hvor du er logget på som lokal bruker.
    
2. Velg **Koble til** under **Få tilgang til jobb eller skole**.
    
3. Skriv inn Microsoft 365 Business legitimasjonen i dialogboksen **Konfigurer en jobb- eller skolekonto** \> **Logg på**.
    
4. Velg **Få tilgang til jobb- eller skolekonto** på siden **Få tilgang til arbeidsplassen eller skolen**, og velg deretter **Informasjon**.
    
    ![Click or tap Info on the Work or school account dalog.](media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Se **Tilkoblingsinformasjon** på siden **Få tilgang jobb eller skole** som inneholder en **Adresse for administrasjonsserver** som er illustrert i følgende figur. Denne inkluderer ordene  *wip*  og  *mam*  . 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Kontroller at du ikke kan lime inn firmadata til en ikke-administrert app**
  
1. Åpne Outlook 2016 og legg til Microsoft 365 Business-kontoen hvis nødvendig, og logg på med Microsoft 365 Business-legitimasjonen.
    
2. Åpne en e-postmelding og kopier noe av innholdet fra den.
    
    Åpne Notisblokk, og prøv å lime inn innholdet.
    
    Du får en feilmelding som sier at appen ikke får tilgang til innholdet.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Du kan imidlertid lime inn det samme innholdet i Word 2016.
    

