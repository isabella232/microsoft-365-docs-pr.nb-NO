---
title: Konfigurere Windows-enheter for Microsoft 365 Business-brukere
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
ms.custom: OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: 'Lær hvordan du konfigurerer Windows-enheter som kjører Windows 10 Pro for Microsoft 365 Business-brukere. '
ms.openlocfilehash: c4edd09d952ed1c98be8f41f6bcbaff8a16319a7
ms.sourcegitcommit: 6003d6da0a85c97357eb3dba3918eb145f381fe1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/27/2019
ms.locfileid: "37288479"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-users"></a>Konfigurere Windows-enheter for Microsoft 365 Business-brukere

## <a name="prerequisites"></a>Forutsetninger

Før du kan konfigurere Windows-enheter for brukere av Microsoft 365 Business, må du kontrollere at alle Windows-enheter kjører Windows 10 Pro, versjon 1703 (Creators Update). Windows 10 Pro er en forutsetning for å distribuere Windows 10 Business, som er et sett med skytjenester og muligheter for enhetsbehandling som utfyller Windows 10 Pro og aktiverer de sentraliserte administrasjons- og sikkerhetskontrollene av Microsoft 365 Business.
  
Hvis du har Windows-enheter som kjører Windows 7 Pro, Windows 8 Pro eller Windows 8.1 Pro, gir Microsoft 365 Business-abonnementet deg en oppgradering til Windows 10.
  
Hvis du vil ha mer informasjon om hvordan du oppgraderer Windows-enheter til Windows 10 Pro Creators Update, følger du fremgangsmåten i dette emnet: [Oppgradere Windows-enheter til Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).
  
Se [kontrollere at enheten er koblet til Azure ad](#verify-the-device-is-connected-to-azure-ad) for å bekrefte at du har oppgraderingen, eller for å kontrollere at oppgraderingen fungerte. 
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Slå sammen Windows 10-enheter med organisasjonens Azure AD

Når alle Windows-enheter i organisasjonen enten har blitt oppgradert til Windows 10 Pro Creators Update eller allerede kjører Windows 10 Pro Creators Update, kan du slå sammen disse enhetene med organisasjonens Azure Active Directory. Når enhetene er slått sammen, vil de automatisk bli oppgradert til Windows 10 Business, som er en del av Microsoft 365 Business-abonnementet.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Hvis du har en helt ny eller nylig oppgradert Windows 10 Pro-enhet

Hvis du har en helt ny enhet som kjører Windows 10 Pro Creators Update eller en enhet som ble oppgradert til Windows 10 Pro Creators Update, men ikke har gått gjennom konfigurasjon for Windows 10-enheter, følger du disse trinnene.
  
1. Gå gjennom konfigurasjonen for Windows 10-enheter frem til **Hvordan vil du konfigurere?**-siden. 
    
    ![On the How would you like to set up page, choose Set up for an organization](media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Her velger du **Konfigurer for en organisasjon**, og deretter angir du brukernavnet og passordet for Microsoft 365 Business. 
    
3. Fullfør konfigurasjonen for Windows 10-enheter.
    
   Når du er ferdig, vil brukeren bli koblet til organisasjonens Azure AD. Se [Kontroller at enheten er koblet til Azure AD](#verify-the-device-is-connected-to-azure-ad) for å være sikker. 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>Hvis du har en enhet som allerede er konfigurert og kjører Windows 10 Pro

 **Koble brukere til Azure AD:**
  
1. I brukerens Windows-PC som kjører Windows 10 Pro, versjon 1703 (Creators Update) (se [forhåndskrav](pre-requisites-for-data-protection.md)), klikk på Windows-logoen og deretter på Innstillinger-ikonet.
  
   ![In the Start menu, click Windows Settings icon](media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. Gå til **Kontoer** i **Innstillinger**.
  
   ![In Windows Settings, go to Accounts](media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. Klikk på **Tilgang jobb eller skole******\> på **Din informasjon**-side.
  
   ![Choose Connect under Access work or school](media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. Velg **Legg denne enheten til Azure Active Directory** under **Alternative handlinger** på **Konfigurer en arbeids- eller skolekonto** -dialogboksen.
  
   ![Click Join this device to Azure Active Directory](media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. På **La oss få deg pålogget** side, Skriv inn jobb eller skole konto \> **neste**.
  
   \> **Skriv inn**passordet ditt på siden **Skriv inn passord** .
  
   ![Enter your work or school email on the Let's get you signed in page](media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. På **Kontroller at dette er din organisasjon** siden, kontroller at informasjonen er riktig, og klikk **bli med**.
  
   Klikk på **Ferdig** på **Alt er klart**-siden.
  
   ![On the Make sure this is your organization screen, click Join](media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Hvis du har lastet opp filer til OneDrive for Business, synkroniser dem tilbake. Hvis du brukte et tredjepartsverktøy til å overføre profil og filer, synkroniserer du disse også mot den nye profilen.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Kontroller at enheten er koblet til Azure AD

For å bekrefte synkroniseringsstatus, på siden **tilgangs arbeid eller skole** i **Innstillinger**, klikker du i **koblet til** _ \<organisasjons\> navn _-området for å vise knappene **info** og **Koble fra**. Klikk på **info** for å få synkroniseringsstatus. 
  
Klikk på Synkronisering på Synkroniseringsstatus-siden for å få de nyeste policyene for administrasjon av mobilenheter på PCen.
  
Gå til **Start**-knappen for Windows, og høyreklikk på det gjeldende kontobildet, og deretter **Bytt konto**, for å begynne å bruke Microsoft 365 Business-kontoen. Logg på ved hjelp av organisasjons e-post og passord.
  
![Click Info button to view synchronization status](media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-device-is-upgraded-to-windows-10-business"></a>Kontrollere at enheten er oppgradert til Windows 10 Business

Kontroller at Windows 10-enhetene som ble slått sammen med Azure AD ble oppgradert til Windows 10 Business, som er en del av Microsoft 365 Business-abonnementet.
  
1. Gå til **Innstillinger** \> **System** \> **Om**.
    
2. Kontroller at **Versjon** viser **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Neste trinn

Hvis du vil konfigurere mobile enheter, kan du se [Konfigurere mobile enheter for brukere av Microsoft 365 Business](set-up-mobile-devices.md). Hvis du vil konfigurere beskyttelse av enheten eller beskyttelsespolicyer for appen, kan du se [Administrere Microsoft 365 Business](manage.md).
  
