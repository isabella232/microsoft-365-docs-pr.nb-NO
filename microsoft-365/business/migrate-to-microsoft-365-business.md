---
title: Oppgrader til Microsoft 365 Business fra Office 365 Business Premium
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
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Trinn som oppgraderer bedriften fra Office 365 Business Premium til Microsoft 365 Business.
ms.openlocfilehash: 61da9148ccb87654aa2391ff90c4f086a4cbbe24
ms.sourcegitcommit: 3c296126ba69a32af07e339f2f1eacdd8e5b878e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/14/2020
ms.locfileid: "41120145"
---
# <a name="upgrade-to-microsoft-365-business-from-office-365-business-premium"></a>Oppgrader til Microsoft 365 Business fra Office 365 Business Premium

Hvis du har en [office 365 for forretnings abonnement](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2), for eksempel Office 365 Business Premium, kan du enkelt oppgradere til Microsoft 365 Business. Oppgrader til Microsoft 365 Business hvis du vil legge til: 
- Windows 10 Pro (til PC-er som kjører Windows 8 eller nyere)
- Enkle kontroller som administrerer forretningsdata på enheter
- Avanserte sikkerhetsfunksjoner.
Finn ut mer om Microsoft 365 Business på [Microsoft.com](https://www.microsoft.com/microsoft-365/business)

## <a name="whats-the-difference-between-office-365-business-premium-and-microsoft-365-business"></a>Hva er forskjellen mellom Office 365 Business Premium og Microsoft 365 Business?
Vi har lagt til en side-ved-side-sammenligning av disse to planene til [Microsoft 365 Business service Description](https://docs.microsoft.com/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description). 

## <a name="before-you-get-started"></a>Før du kommer i gang

- **Når bør jeg velge å oppgradere?** Oppgradering er det riktige valget når du vil oppgradere **alle brukere** som er tilordnet en enkelt plan. Når du velger oppgradering, blir alle plan brukerne byttet til en annen plan samtidig. Hvis du ikke vil oppgradere alle som er tilordnet en enkelt plan, kjøper du lisenser for den nye planen (i dette tilfellet Microsoft 365 Business), og [tilordner disse lisensene individuelt](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) til hver bruker du vil oppgradere. 
- **Noen tilleggsprogrammer kan hindre oppgraderingen** Hvis du prøver å starte en oppgradering, og du har et tillegg som hindrer deg i å fortsette, kan du fjerne tillegget først og deretter legge det til på nytt senere hvis du fortsatt trenger det. 
- **Hvis du har forhåndsbetalt abonnementet** Det finnes ingen enkel oppgraderingsbane for forhåndsbetalte planer. Du vet om du har en forhåndsbetalt Plan fordi du har konfigurert planen med en produkt-ID som du kanskje har kjøpt i en butikk. Kontakt en partner, gå til Microsoft store, eller vent til den forhåndsbetalte planen utløper for å bytte til en ny plan.

## <a name="upgrade-to-microsoft-365-business"></a>Oppgrader til Microsoft 365 Business
Kjøp lisensene ved å følge disse trinnene i det [nye administrasjonssenteret](https://docs.microsoft.com/office365/admin/microsoft-365-admin-center-preview):
1. Logg på administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a>.
2. Gå til navigasjonsruten, og velg **fakturerings** \> **produkter & tjenester**. Finn abonnementet på Office 365, og velg det for å vise detaljene. 

    ![Et skjermbilde viser hvordan du finner og velger abonnementet i administrasjonssenteret.](media/FindYourSubscription.png)

3. Velg **Oppgrader**på neste side. 

      ![Et skjermbilde viser hvor du kan velge Oppgrader i administrasjonssenteret.](media/SelectUpgrade.png)

  > [!NOTE]
  > Hvis du ser en melding om at **oppgradering av abonnementet ikke støttes med gruppebasert lisensiering i Azure Active Directory**, kan du trygt ignorere dette med mindre du har en veldig stor organisasjon. Organisasjoner som har valgt dette alternativet, er klar over at de brukergruppe BAS ert lisensiering.

4. Deretter kan du vise en liste over Office-planer som du kan oppgradere til. I dette tilfellet finner du Microsoft 365 forretningsplan. Du kan rulle nedover hvis du vil vise alle Office-appene og-tjenestene som er inkludert i denne planen. Under **Microsoft 365 Business**velger du **Oppgrader** for å legge til Microsoft 365 Business i handlekurven.
5. I handlevognen:
    1. Vi tar automatisk med lisenser for alle dine nåværende brukere. Hvis du trenger flere eller færre lisenser, må du [kjøpe og tilordne disse lisensene enkeltvis](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users).  
    2. Du kan justere hvordan du ønsker å betale: månedlig eller årlig. Velg rullegardinmenyen for å gjøre ditt valg.
6. Velg **gå til kassen** der du ser et sammendrag av kjøpet, inkludert betalingsmåten for denne kontoen. Du kan også legge til en promo-kode her hvis du har en.
7. Velg **Bestill** for å fullføre kjøpet.
Det tar Microsoft noen minutter å sette opp nye Service planer. Hvis du vil kontrollere fremdriften, velger du **Kontroller oppgraderingsstatus**. 
1. Når planen er klar, må du kanskje fullføre noen ekstra konfigurasjonstrinn i administrasjonssenteret. I navigasjonsruten velger du **hjem** for å fullføre eventuelle ekstra konfigurasjonstrinn.

> [!NOTE]
> Du vil motta en forholdsmessig refusjon for Office 365-lisensene du ikke lenger trenger. Bankkontoen eller kredittkortet blir belastet omtrent to dager etter at du har konfigurert den nye planen.
  
## <a name="protect-user-devices-and-files"></a>Beskytt bruker enheter og filer

Nå som Microsoft 365 Business-lisenser er tilordnet, må du fullføre trinnene for å begynne å beskytte enheter og filer. Du skal bruke noen nye alternativer som er inkludert i navigasjonsruten i administrasjonssenteret.
  
1. Gå til **enhetens** \> **policyer**i navigasjonsruten i Administrasjonssenter.
    
2. Velg **Legg til**på siden **enhetspolicyer** .
    
3. I **Legg til policy** -ruten gi policyen et navn (for eksempel Beskytt arbeidsfiler), og velg deretter en **PolicyType** fra rullegardinlisten. 
    
    Du kan konfigurere programpolicyer for å beskytte filer på Android-og iPhone-enheter, i tillegg til Windows 10, og du kan konfigurere policyer for enhetskonfigurasjon for firmaets eide Windows 10-enheter. Se følgende koblinger for mer informasjon:
    
  - [Angi innstillinger for appbeskyttelse på Android- eller iOS-enheter](app-protection-settings-for-android-and-ios.md)
    
  - [Angi innstillinger for appbeskyttelse for Windows 10-enheter](protection-settings-for-windows-10-devices.md)
    
  - [Angi innstillinger for enhetsbeskyttelse for Windows 10-PCer](protection-settings-for-windows-10-pcs.md)
    
  
4. Når du har konfigurert policyer, kan du og de ansatte konfigurere enheter:
    
  - Hvis Windows-enhetene dine ikke allerede bruker Windows Pro Creator-oppdateringen, må du [oppgradere dem til Windows Pro Creators Update](upgrade-to-windows-pro-creators-update.md).
    
  - Se [konfigurere Windows-enheter for Microsoft 365 Business-brukere](set-up-windows-devices.md) for trinn for Windows-enheter. 
    
  - Se [konfigurere mobile enheter for Microsoft 365 Business-brukere](set-up-mobile-devices.md) for trinn for Android-telefoner og iPhone. 
