---
title: Konfigurere Windows enheter for Microsoft 365 Business Premium brukere
f1.keywords:
- CSH
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
description: Lær hvordan du konfigurerer Windows enheter som kjører Windows 10 Pro for Microsoft 365 Business Premium, slik at sentralisert administrasjon og sikkerhetskontroller aktiveres.
ms.openlocfilehash: 3e268d81ff6fb7113b7e0b0fe5d0545ff5c72b1e
ms.sourcegitcommit: ff20f5b4e3268c7c98a84fb1cbe7db7151596b6d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/06/2021
ms.locfileid: "52244780"
---
# <a name="set-up-windows-devices-for-microsoft-365-business-premium-users"></a>Konfigurere Windows enheter for Microsoft 365 Business Premium brukere

## <a name="prerequisites-for-setting-up-windows-devices-for-microsoft-365-business-premium-users"></a>Forutsetninger for å konfigurere Windows enheter for Microsoft 365 Business Premium brukere

Før du kan konfigurere Windows-enheter for Microsoft 365 Business Premium-brukere, må du kontrollere at alle Windows-enhetene kjører Windows 10 Pro, versjon 1703 (Creators Update). Windows 10 Pro er en forutsetning for å distribuere Windows 10 Business, som er et sett med skytjenester og funksjoner for enhetsbehandling som utfyller Windows 10 Pro og aktiverer sentralisert administrasjon og sikkerhetskontroller for Microsoft 365 Business Premium.
  
Hvis du Windows enheter som kjører Windows 7 Pro, Windows 8 Pro eller Windows 8.1 Pro, gir Microsoft 365 Business Premium-abonnementet deg tilgang til en Windows 10 oppgradering.
  
Hvis du vil ha mer informasjon om hvordan du oppgraderer Windows-enheter til Windows 10 Pro Creators Update, følger du fremgangsmåten i dette emnet: [Oppgradere Windows-enheter til Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).
  
Se [Kontrollere at enheten er koblet til Azure AD](#verify-the-device-is-connected-to-azure-ad) for å bekrefte at du har oppgraderingen, eller for å sikre at oppgraderingen fungerte.

Se en kort video om hvordan du kobler Windows til Microsoft 365.<br><br>

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3yXh3] 

Hvis du synes at denne videoen er nyttig, kan du se den [fullstendige opplæringsserien for små bedrifter og de som er nybegynnere i Microsoft 365](../business-video/index.yml).
  
## <a name="join-windows-10-devices-to-your-organizations-azure-ad"></a>Slå sammen Windows 10-enheter med organisasjonens Azure AD

Når alle Windows-enheter i organisasjonen enten har blitt oppgradert til Windows 10 Pro Creators Update eller allerede kjører Windows 10 Pro Creators Update, kan du bli med i disse enhetene til organisasjonens Azure Active Directory. Når enhetene er koblet til, oppgraderes de automatisk til Windows 10 Business, som er en del av Microsoft 365 Business Premium abonnementet.
  
### <a name="for-a-brand-new-or-newly-upgraded-windows-10-pro-device"></a>Hvis du har en helt ny eller nylig oppgradert Windows 10 Pro-enhet

Hvis du har en helt ny enhet som kjører Windows 10 Pro Creators Update eller en enhet som ble oppgradert til Windows 10 Pro Creators Update, men ikke har gått gjennom konfigurasjon for Windows 10-enheter, følger du disse trinnene.
  
1. Gå gjennom konfigurasjonen for Windows 10-enheter frem til **Hvordan vil du konfigurere?**-siden. 
    
    ![On the How would you like to set up page, choose Set up for an organization](../media/1b0b2dba-00bb-4a99-a729-441479220cb7.png)
  
2. Her velger du **Konfigurer for en organisasjon, og** deretter skriver du inn brukernavnet og passordet for Microsoft 365 Business Premium. 
    
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
  
5. Skriv inn **jobb-** eller skolekontoen neste på siden La oss få deg logget \> **på.**
  
   Skriv inn **passordet** Logg på på Skriv inn \> **passord-siden.**
  
   ![Enter your work or school email on the Let's get you signed in page](../media/f70eb148-b1d2-4ba3-be38-7317eaf0321a.png)
  
6. Kontroller at **informasjonen er** riktig på kontroller at dette er organisasjonens side, og velg Bli **med**.
  
   På **You're all set!** side, chosse **Done**.
  
   ![Velg Bli med på skjermen Kontroller at dette er organisasjonen](../media/c749c0a2-5191-4347-a451-c062682aa1fb.png)
  
Hvis du har lastet opp filer til OneDrive for Business, synkroniser dem tilbake. Hvis du brukte et tredjepartsverktøy til å overføre profil og filer, synkroniserer du også disse til den nye profilen.
  
## <a name="verify-the-device-is-connected-to-azure-ad"></a>Kontroller at enheten er koblet til Azure AD

Hvis du vil bekrefte synkroniseringsstatusen, går du til **jobb- eller skolesiden i** **Innstillinger** og velger området Tilkoblet **_** _ for å vise knappene \<organization name\> **Informasjon** og **Koble fra**. Velg **Informasjon for** å få synkroniseringsstatusen. 
  
Velg **Synkroniser på** Synkroniseringsstatus-siden **for** å få de nyeste policyene for administrasjon av mobilenheter til PC-en.
  
Hvis du vil begynne å Microsoft 365 Business Premium kontoen, går  du til startknappen Windows, høyreklikker det gjeldende kontobildet, og deretter **bytter du konto**. Logg på ved hjelp av organisasjons e-post og passord.
  
![Click Info button to view synchronization status](../media/818f7043-adbf-402a-844a-59d50034911d.png)
  
## <a name="verify-the-pc-is-upgraded-to-windows-10-business"></a>Kontroller at PC-en er oppgradert til Windows 10 Business

Kontroller at Azure AD-Windows 10 er oppgradert til Windows 10 Business som en del av Microsoft 365 Business Premium abonnementet.
  
1. Gå til **Innstillinger** \> **System** \> **Om**.
    
2. Kontroller at **Versjon** viser **Windows 10 Business**.
    
    ![Verify that Windows edition is Windows 10 Business.](../media/ff660fc8-d3ba-431b-89a5-f5abded96c4d.png)
  
## <a name="next-steps"></a>Neste trinn

Hvis du vil konfigurere mobile enheter, kan du se Konfigurere mobile enheter [for Microsoft 365 Business Premium](set-up-mobile-devices.md)- Hvis du vil angi policyer for beskyttelse av enheter eller appbeskyttelse, kan du se Administrere Microsoft 365 [for bedrifter](manage.md).
  
## <a name="for-more-on-setting-up-and-using-microsoft-365-business-premium"></a>Hvis du vil ha mer informasjon om hvordan du konfigurerer og bruker Microsoft 365 Business Premium

[Microsoft 365 opplæringsvideoer for bedrifter](../business-video/index.yml)
