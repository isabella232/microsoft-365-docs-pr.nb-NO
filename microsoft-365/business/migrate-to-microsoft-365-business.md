---
title: Migrere til Microsoft 365 Business fra Office 365 Business Premium
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Lær hvordan å flytte bedriften til Microsoft 365 Business.
ms.openlocfilehash: fd6f18c02453e6751d6163ab79e726eae9c951a9
ms.sourcegitcommit: eb1a77e4cc4e8f564a1c78d2ef53d7245fe4517a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/28/2018
ms.locfileid: "26983496"
---
# <a name="migrate-to-microsoft-365-business-from-office-365-business-premium"></a>Migrere til Microsoft 365 Business fra Office 365 Business Premium

Hvis du allerede har et Office 365 for business-abonnement, for eksempel Office 365 Business Premium, kan du enkelt legge til lisenser i Microsoft 365 Business, og tilordne dem til noen eller alle brukere.
  
> [!NOTE]
> Du kan ikke bruke knappen [Bytt planer](https://support.office.com/article/73318661-8f33-478b-bcc7-fb8d69dbb22a?.aspx#switchbutton) for å oppgradere til Microsoft 365 Business ennå. 
  
## <a name="add-microsoft-365-business-licenses"></a>Legg til lisenser for Microsoft 365 Business

Du har to måter å få Microsoft 365 Business. Hvis du har en partner, kan han eller hun kjøpe Microsoft 365 Business du fra [Microsoft Partner Center](get-microsoft-365-business.md). Partneren kan også hjelpe deg med overgangen til Microsoft 365 Business.
  
Hvis du administrerer din egen abonnement, kan du [kontakte salg](https://www.microsoft.com/microsoft-365/business) for å kjøpe Microsoft 365 Business lisenser. 
  
Se [legge til, endre, eller slette et abonnement advisor-partner](https://support.office.com/article/f86e8177-936e-491e-9024-44dea2b296ff) for å finne ut hvordan du kan starte arbeidet med en partner. 
  
Hvis du får en kobling for å kjøpe dine lisenser, leder gjennom en veiviser som den nedenfor. Velg **Ja, legge den til Min konto**. Du kan også velge antall lisenser og betalingsmåten.
  
![Kjøpe kobling på Microsoft 365 Business direkte, kan du velge å legge til den gjeldende kontoen eller opprette en ny konto.](media/8bc54fd1-9cab-44d5-af91-c471e89aea46.png)
  
## <a name="assign-microsoft-365-licenses"></a>Tilordne lisenser for Microsoft 365

1. Når du har kjøpt nye lisenser, og dette er første gang du gjorde, viser banneret installasjonsprogrammet for Microsoft 365 Business på administrasjonssenteret.
    
    > [!NOTE]
    > Oppsett av banneret er en mulighet til å legge til nye brukere, et nytt domene, og overføre e-post for nye brukere. Hvis du ikke har tenkt å gjøre, bør du likevel gå gjennom veiviseren og velger standardalternativer for å gjøre det forsvinner fra hjemmesiden til admin. 
  
   ![Velg Start installasjonsprogrammet på Microsoft 365 Business er klar til å sette opp banneret.](media/8d3b0d97-7cca-497f-9364-4b00ad670209.png)
  
    Velg **Start konfigurasjon**.
    
2. På siden **Tilpass påloggingen og e-post** , kan du legge til et domene ved å velge **koble til et domene du allerede eier** Hvis du vil bruke denne muligheten til å legge til et annet domene i abonnementet. 
    
    Hvis du allerede har definert et domene, det andre feltet angir som og står **Fortsett å bruke** \< _domenenavnet_ \> **for e-post og logger på**. Hvis du ikke har satt opp et domene med du abonnementet, det vil si **Fortsett å bruke** \< _firma-name.onmicrosoft.com_ \> **for e-post og logger på**.    
    
    Velg **Neste**.
    
    ![På siden Tilpass påloggingen og e-post, kan du velge å legge til et domene, eller bruk den som du har brukt.](media/c3f5cfb2-1189-4d2f-803b-c9feb008a7a3.png)
  
3. På siden **Legg til nye brukere** , kan du legge til nye brukere, hvis du har nye ansatte som du vil tilordne lisenser for Microsoft 365 Business å. 
    
    Hvis du ikke har nye ansatte til å legge til og vil tilordne lisenser til eksisterende brukere, velger du **Neste**.
    
4. På den ** Overfør e-postmeldinger ** siden kan du velge å overføre e-post til noen av de nye brukerne som du la til i trinn 3. Du kan også hoppe over dette trinnet. Velg **Neste**.
    
5. På den siste siden, velg **Gå til administrasjonssenteret**, og fortsette installasjonen det.
    
6. Gå til **brukere** i administrasjonssenteret, \> **aktive brukere**.
    
7. Velg brukeren du vil tilordne **Microsoft 365 Business** -lisens til, og velg deretter **Rediger** ved siden av **Produktlisenser**.
    
    ![I bruker-kortet, velger du Rediger ved siden av produktlisenser.](media/be0fe2d8-7ff8-447c-88f6-d212ed78451c.png)
  
8. I **produktlisenser** lysbilde **Microsoft 365 Business** **på** \> **Lagre**, og deretter **Lukk**.
    
Når du har kjøpt den opprinnelige lisensen for Microsoft 365 Business, kan du nå også legge mer i **Fakturering** \> **Kjøp tjenester**. På siden **kjøper tjenester,** kan du klikke på ellipser på visittkortet **Microsoft 365** og velge **Endre lisensen antall** til å kjøpe mer. 
  
## <a name="protect-user-devices-and-files"></a>Beskytte Brukerenheter og filer

Når du har tilordnet lisenser Microsoft 365 Business, kan du begynne å beskytte brukernes enheter og filer.
  
1. Gå til **enheter** i administrasjonssenteret i venstre nav, \> **policyer**.
    
2. På siden **policyer for enheten** , velger du **Legg til**.
    
3. Gi et navn for policyen i ruten **Legg til policy** , og velg deretter en **Policy-type** fra rullegardinlisten. 
    
    Du kan definere programpolicyer for å beskytte filer på Android og iPhone-enheter, i tillegg til Windows-10, og du kan definere policyer for enheten konfigurasjonen for firma som eies av Windows 10 enheter. Se følgende koblinger for mer informasjon:
    
  - [Angi innstillinger for appbeskyttelse på Android- eller iOS-enheter](app-protection-settings-for-android-and-ios.md)
    
  - [Angi innstillinger for appbeskyttelse for Windows 10-enheter](protection-settings-for-windows-10-devices.md)
    
  - [Angi beskyttelsesinnstillinger for Windows 10 PC-er](protection-settings-for-windows-10-pcs.md)
    
   ![I ruten Legg til policy, skriver du inn et navn for den, og velg hvilken Policy fra på rullegardinmenyen.](media/76ef37e4-1d18-4f34-8a0f-391ab1d0ae2b.png)
  
4. Når du definerer policyer, kan du og dine ansatte angi enheter:
    
  - Hvis Windows ikke allerede er på Pro Creator for Windows update, må du oppgradere [dem oppgradere Windows Pro skapere](upgrade-to-windows-pro-creators-update.md).
    
  - Se [konfigurere Windows-enheter for forretningsbrukere som Microsoft 365](set-up-windows-devices.md) for fremgangsmåten for Windows-enheter. 
    
  - Se [definere mobile enheter for forretningsbrukere som Microsoft 365](set-up-mobile-devices.md) for trinnene for Android telefoner og iPhones. 
    
5. Hvis du vil installere Office-klientprogrammer automatisk, kan du se [Klargjør for distribusjon av Office-klienten ved Microsoft 365 Business](prepare-for-office-client-deployment.md) og [automatisk installere eller avinstallere Office på Windows 10 enheter](auto-install-or-uninstall-office.md).
    


