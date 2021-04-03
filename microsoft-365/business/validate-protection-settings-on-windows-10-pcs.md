---
title: Validere innstillingene for appbeskyttelse på Windows 10-datamaskiner
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
- M365-subscription-management
- M365-identity-device-management
ms.custom:
- Adm_O365
- Core_O365Admin_Migration
- MSB365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: fae8819d-7235-495f-9f07-d016f545887f
description: Valider innstillinger for appbeskyttelse for Microsoft 365 Business Premium på Windows 10-enheter, og kontroller at brukere ikke kan kopiere firmadata til personlige filer eller ikke-administrerte apper.
ms.openlocfilehash: e319ffa5149f055b5de45078facc8899acffc223
ms.sourcegitcommit: 53acc851abf68e2272e75df0856c0e16b0c7e48d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/02/2021
ms.locfileid: "51579866"
---
# <a name="validate-app-protection-settings-on-windows-10-pcs"></a>Validere innstillingene for appbeskyttelse på Windows 10-datamaskiner

## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-corporate-devices"></a>Kontroller at brukere ikke kan kopiere firmadata til personlige filer på bedriftens enheter

Etter at du [har konfigurert policyer for appbeskyttelse](protection-settings-for-windows-10-devices.md), kan det ta opptil noen timer før policyen trer i kraft på brukernes enheter. Hvis du  har aktivert innstillingen Hindre brukere i å kopiere firmadata til personlige filer og tvinge dem til å lagre arbeidsfiler i **OneDrive for Business** for firmaeide enheter, kan du kontrollere dette på brukerens enhet etter at de har koblet til Azure AD og logget på. 
  
 **Kontrollere tilkoblingsinnstillinger**
  
1. Når du har logget på med Microsoft 365 Business Premium-legitimasjon og koblet til Azure AD som beskrevet i Konfigurere [Windows-enheter for Microsoft 365 Business Premium-brukere,](set-up-windows-devices.md)går du til **Windows-innstillinger** Kontoer Tilgang til jobb \>  \> **eller skole**. Velg **Koblet til Azure \<tenant name\> AD**, og velg deretter **Informasjon**.
    
    ![Click or tap Info on the Connected to Azure AD dialog.](../media/a36ede2b-d1a0-4d4e-8ea7-af39b4b63890.png)
  
2. På **Administrert av-siden** kan du se tilkoblingsinformasjonen som inneholder en Adresse for administrasjonsserver, som den som \<tenant name\> vises i figuren nedenfor.   
    
    ![Managed by page shows connection info of the device manager URL.](../media/47515a8e-2d0c-4bea-99f0-6b2545b88a11.png)
  
 **Kontroller at du ikke kan lime inn firmadata i en ikke-administrert app**
  
1. Åpne Outlook 2016 som ble installert av Microsoft 365 Business Premium.
    
2. Åpne en e-postmelding og kopier noe av innholdet fra den.
    
    Åpne Notisblokk, og prøv å lime inn innholdet.
    
    Du får en feilmelding som sier at appen ikke har tilgang til innhold.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Du kan imidlertid lime inn det samme innholdet i Word 2016.
    
## <a name="verify-that-users-cannot-copy-company-data-to-personal-files-on-personal-devices"></a>Kontroller at brukere ikke kan kopiere firmadata til personlige filer på personlige enheter

 **Kontrollere tilkoblingsinnstillinger**
  
1. Gå til Windows-innstillinger på den personlige **Windows** 10-enheten der du er  logget på som en lokal bruker, og klikk eller trykk Kontoer Tilgang til jobb \> **eller skole.**
    
2. Velg **Koble til** under **Få tilgang til jobb eller skole**.
    
3. Skriv inn Microsoft 365 Business Premium-legitimasjonen i dialogboksen Konfigurer en jobb- eller **skolekonto** \> **Logg på**.
    
4. Velg **Få tilgang til jobb- eller skolekonto** på siden **Få tilgang til arbeidsplassen eller skolen**, og velg deretter **Informasjon**.
    
    ![Klikk eller trykk informasjon i dialogboksen Jobb- eller skolekonto.](../media/63bd8b32-cb32-4afa-8ce0-6070ac403abc.png)
  
5. Du kan se Tilkoblingsinformasjon som  inneholder en **Adresse** for administrasjonsserver, som den som vises i figuren nedenfor, på siden **Access-jobb** eller skole, og inneholder ordene *wip* og *mam* inni. 
    
    ![Managed by page shows connection info URL that includes the words mam and wpi.](../media/abd4eaf4-44fa-4538-a3e8-1e0d331dfe1e.png)
  
 **Kontroller at du ikke kan lime inn firmadata i en ikke-administrert app**
  
1. Åpne Outlook 2016, og legg til Microsoft 365 Business Premium-kontoen om nødvendig, og logg på med Microsoft 365 Business Premium-legitimasjonen.
    
2. Åpne en e-postmelding og kopier noe av innholdet fra den.
    
    Åpne Notisblokk, og prøv å lime inn innholdet.
    
    Du får en feilmelding om at appen ikke har tilgang til innhold.
    
    ![A dialog that states app can't access content when you paste into an unmanaged app.](../media/5e82b154-cf2f-43c8-ae80-b45d8ad80e56.png)
  
    Du kan imidlertid lime inn det samme innholdet i Word 2016.
    

