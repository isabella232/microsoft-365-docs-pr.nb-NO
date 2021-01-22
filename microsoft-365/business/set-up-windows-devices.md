---
title: Konfigurere Windows-enheter for Brukere av Microsoft 365 Business Premium
f1.keywords:
- CSH
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
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- TRN_M365B
- OKR_SMB_Videos
- seo-marvel-mar
- AdminSurgePortfolio
- okr_smb
search.appverid:
- BCS160
- MET150
ms.assetid: 2d7ff45e-0da0-4caa-89a9-48cabf41f193
description: Lær hvordan du konfigurerer Windows-enheter som kjører Windows 10 Pro for Brukere av Microsoft 365 Business Premium, slik at sentralisert administrasjon og sikkerhetskontroller aktiveres.
ms.openlocfilehash: b1877d83f113a2ba23d0db374967e0afcd7fe067
ms.sourcegitcommit: 855719ee21017cf87dfa98cbe62806763bcb78ac
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/22/2021
ms.locfileid: "49928728"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Konfigurere Windows-enheter for Brukere av Microsoft 365 Business Premium

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a>Forutsetninger for å konfigurere Windows-enheter for brukere av Microsoft 365 Business Premium

Før du kan konfigurere Windows-enheter for brukere av Microsoft 365 Business Premium, må du kontrollere at alle Windows-enheter kjører Windows 10 Pro, versjon 1703 (Creators Update). Windows 10 Pro er en forutsetning for å distribuere Windows 10 Business, som er et sett med skytjenester og muligheter for enhetsbehandling som utfyller Windows 10 Pro og aktiverer de sentraliserte administrasjons- og sikkerhetskontrollene av Microsoft 365 Business Premium.
  
Hvis du har Windows-enheter som kjører Windows 7 Pro, Windows 8 Pro eller Windows 8.1 Pro, gir Microsoft 365 Business Premium-abonnementet deg en oppgradering til Windows 10.
  
Hvis du vil ha mer informasjon om hvordan du oppgraderer Windows-enheter til Windows 10 Pro Creators Update, følger du fremgangsmåten i dette emnet: [Oppgradere Windows-enheter til Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).
  
Se [Kontrollere at enheten er koblet til Azure AD](#verify-the-device-is-connected-to-azure-ad) for å bekrefte at du har oppgraderingen, eller for å kontrollere at oppgraderingen fungerte.

Se en kort video om hvordan du kobler Windows til Microsoft 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Hvis du synes at denne videoen er nyttig, kan du se den [fullstendige opplæringsserien for små bedrifter og de som er nybegynnere i Microsoft 365](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Slå sammen Windows 10-enheter med organisasjonens Azure AD

Når alle Windows-enheter i organisasjonen enten har blitt oppgradert til Windows 10 Pro Creators Update eller allerede kjører Windows 10 Pro Creators Update, kan du slå sammen disse enhetene med organisasjonens Azure Active Directory. Når enhetene er koblet sammen, oppgraderes de automatisk til Windows 10 Business, som er en del av Microsoft 365 Business Premium-abonnementet.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Hvis du har en helt ny eller nylig oppgradert Windows 10 Pro-enhet

Hvis du har en helt ny enhet som kjører Windows 10 Pro Creators Update eller en enhet som ble oppgradert til Windows 10 Pro Creators Update, men ikke har gått gjennom konfigurasjon for Windows 10-enheter, følger du disse trinnene.
  
1. Gå gjennom konfigurasjonen for Windows 10-enheter frem til **Hvordan vil du konfigurere?**-siden. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Her velger du **Konfigurer for en organisasjon,** og deretter skriver du inn brukernavnet og passordet for Microsoft 365 Business Premium. 
    
3. Fullfør konfigurasjonen for Windows 10-enheter.
    
   Når du er ferdig, vil brukeren bli koblet til organisasjonens Azure AD. Se [Kontroller at enheten er koblet til Azure AD](#verify-the-device-is-connected-to-azure-ad) for å være sikker. 
  
### <a name="for-a-device-already-set-up-and-running-windows-10-pro"></a>Hvis du har en enhet som allerede er konfigurert og kjører Windows 10 Pro

 **Koble brukere til Azure AD:**
  
1. I brukerens Windows-PC som kjører Windows 10 Pro, versjon 1703 (Creators Update) (se [forhåndskrav](pre-requisites-for-data-protection.md)), klikk på Windows-logoen og deretter på Innstillinger-ikonet.
  
   ![In the Start menu, click Windows Settings icon](../media/74e1ce9a-1554-4761-beb9-330b176e9b9d.png)
  
2. Gå til **Kontoer** i **Innstillinger**.
  
   ![In Windows Settings, go to Accounts](../media/472fd688-d111-4788-9fbb-56a00fbdc24d.png)
  
3. Klikk på **Tilgang jobb eller skole**\> på **Din informasjon**-side.
  
   ![Choose Connect under Access work or school](../media/af3a4e3f-f9b9-4969-b3e2-4ef99308090c.png)
  
4. Velg **Legg denne enheten til Azure Active Directory** under **Alternative handlinger** på **Konfigurer en arbeids- eller skolekonto** -dialogboksen.
  
   ![Click Join this device to Azure Active Directory](../media/fb709a1b-05a9-4750-9cb9-e097f4412cba.png)
  
5. Skriv inn **jobb-** eller skolekontoen din neste på siden La oss få deg pålogget. \> 
  
   Skriv inn **passordet ditt** på siden Skriv inn \> **passord.**
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. Kontroller at **informasjonen er** riktig på siden Kontroller at dette er organisasjonen din, og velg Bli **med.**
  
   Alt **er i gang!** side, chosse **Ferdig.**
  
   ![På skjermen Kontroller at dette er organisasjonen din velger du Bli med](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Hvis du har lastet opp filer til OneDrive for Business, synkroniser dem tilbake. Hvis du brukte et tredjepartsverktøy til å overføre profil og filer, synkroniserer du disse også med den nye profilen.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Kontroller at enheten er koblet til Azure AD

Hvis du vil bekrefte synkroniseringsstatusen, velger du  tilkoblet ___-området på jobb- eller skolesiden for **Access** i Innstillinger for å vise knappene \<organization name\> **Informasjon** og **Koble fra.** Velg **Informasjon for** å få synkroniseringsstatus. 
  
Velg **Synkroniser på** **Synkroniseringsstatus-siden** for å få de nyeste policyene for administrasjon av mobilenheter på PC-en.
  
Hvis du vil begynne å bruke Microsoft 365 Business Premium-kontoen, kan du gå til **Start-knappen** i Windows, høyreklikke på det gjeldende kontobildet og deretter bytte **konto.** Logg på ved hjelp av organisasjons e-post og passord.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a>Kontroller at PC-en er oppgradert til Windows 10 Business

Kontroller at Windows 10-enhetene som er koblet til Azure AD, er oppgradert til Windows 10 Business som en del av Microsoft 365 Business Premium-abonnementet.
  
1. Gå til **Innstillinger** \> **System** \> **Om**.
    
2. Kontroller at **Versjon** viser **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Neste trinn

Hvis du vil konfigurere de mobile enhetene dine, kan du se Konfigurere mobile enheter for brukere av [Microsoft 365 Business Premium.](set-up-mobile-devices.md)Hvis du vil angi beskyttelsespolicyer for enheten eller beskyttelsespolicyer for appen, kan du se Administrere [Microsoft 365 for bedrifter.](manage.md)
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a>Hvis du vil ha mer informasjon om hvordan du konfigurerer og bruker Microsoft 365 Business Premium

[Opplæringsvideoer for Microsoft 365 for bedrifter](https://support.microsoft.com/office/6ab4bbcd-79cf-4000-a0bd-d42ce4d12816)
