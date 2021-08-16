---
title: Oppgrader til Microsoft 365 Business Premium fra Microsoft 365 Business Standard
f1.keywords:
- NOCSH
ms.author: cmcatee
author: cmcatee-MSFT
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
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
ms.assetid: 5b4ba843-24b8-4526-8e1f-f9b9eab89d06
description: Lær forskjellen mellom Microsoft 365 Business Standard og Microsoft 365 Business Premium og hvordan du kan oppgradere til Microsoft 365 Business Premium.
ms.openlocfilehash: 563df2610351e2c025c618086c038750999c03df60b93b757865f76fbf86c834
ms.sourcegitcommit: a1b66e1e80c25d14d67a9b46c79ec7245d88e045
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53906731"
---
# <a name="upgrade-to-microsoft-365-business-premium-from-microsoft-365-business-standard"></a>Oppgrader til Microsoft 365 Business Premium fra Microsoft 365 Business Standard

Hvis du har et [Microsoft 365 for bedrifter-abonnement,](https://products.office.com/compare-all-microsoft-office-products-4-column?activetab=tab:primaryr2)for eksempel Microsoft 365 Business Standard, kan du enkelt oppgradere til Microsoft 365 Business Premium. Oppgrader Microsoft 365 Business Premium hvis du vil legge til:

- Windows 10 Pro (til PC-er som kjører Windows 8 eller nyere)

- Enkle kontroller som administrerer forretningsdata på enheter

- Avanserte sikkerhetsfunksjoner.
Finn ut mer om Microsoft 365 Business Premium på [Microsoft.com](https://www.microsoft.com/microsoft-365/business)

## <a name="whats-the-difference-between-microsoft-365-business-standard-and-microsoft-365-business-premium"></a>Hva er forskjellen mellom Microsoft 365 Business Standard og Microsoft 365 Business Premium?

Vi har lagt til en side-ved-side-sammenligning av disse to planene i Microsoft 365 Business Premium [Tjenestebeskrivelse](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-business-service-description). 

## <a name="before-you-begin"></a>Før du starter

- **Når bør jeg velge å oppgradere?** Oppgradering er det riktige valget når du vil oppgradere **alle brukere som** er tilordnet til ett enkelt abonnement. Når du velger oppgradering, byttes alle planbrukere til et annet abonnement samtidig. Hvis du ikke vil oppgradere alle som er tilordnet til ett enkelt abonnement, kan du kjøpe [](../admin/manage/assign-licenses-to-users.md) lisenser for det nye abonnementet (i dette tilfellet Microsoft 365 Business Premium), og tilordne disse lisensene enkeltvis til hver bruker du vil oppgradere.

- **Noen tillegg kan hindre oppgraderingen** Hvis du prøver å starte en oppgradering og du har et tillegg som hindrer deg i å fortsette, kan du fjerne tillegget først og deretter legge det til på nytt senere hvis du fremdeles trenger det.

- **Hvis du har forhåndsbetalt abonnementet** Det finnes ikke en enkel oppgraderingsbane for forhåndsbetalte planer. Du vet om du har et forhåndsbetalt abonnement fordi du konfigurerer abonnementet ved hjelp av en produkt-ID som du kanskje har kjøpt i en butikk. Kontakt en partner, gå til Microsoft Store, eller vent til det forhåndsbetalte abonnementet utløper for å bytte til et nytt abonnement.

## <a name="upgrade-to-microsoft-365-business-premium"></a>Oppgrader til Microsoft 365 Business Premium

1. Logg på administrasjonssenteret på <a href="https://go.microsoft.com/fwlink/p/?linkid=837890" target="_blank">https://admin.microsoft.com</a> .

2. Gå til navigasjonsruten, og velg **Fakturering** \> **av produkter**. Finn det gjeldende abonnementet, og velg det for å vise detaljene.

3. Velg Oppgrader på neste **side.**

  > [!NOTE]
  > Hvis du ser en melding om at oppgradering av abonnementet ikke støttes med gruppebasert **lisensiering** i Azure Active Directory, kan du trygt ignorere dette med mindre du har en svært stor organisasjon. Organisasjoner som har valgt dette alternativet, vil være oppmerksomme på at de bruker gruppebasert lisensiering.

4. Deretter kan du vise en liste over planer som du kan oppgradere til. I dette tilfellet finner du Microsoft 365 Business Premium planen. Du kan rulle nedover hvis du vil se alle appene og tjenestene som er inkludert i denne planen. Under **Microsoft 365 Business Premium** velger du **Oppgrader** for å legge Microsoft 365 Business Premium i handlekurven.

5. I handlekurven:

    1. Vi inkluderer automatisk lisenser for alle gjeldende brukere. Hvis du trenger flere eller færre lisenser, må du kjøpe [og tilordne disse lisensene enkeltvis.](../admin/manage/assign-licenses-to-users.md)  
    2. Du kan justere hvordan du vil betale: månedlig eller årlig. Velg rullegardinmenyen for å velge.

6. Velg **Gå til kassen** der du vil se et sammendrag av kjøpet, inkludert betalingsmåten for denne kontoen. Du kan også legge til en kampanjekode her hvis du har en.

7. Velg **Legg inn bestilling** for å fullføre kjøpet.\
Det tar Microsoft noen minutter å konfigurere de nye tjenesteplanene. Hvis du vil kontrollere fremdriften, **velger du Kontroller oppgraderingsstatus**.

8. Når planen er klar, må du kanskje fullføre noen ekstra konfigurasjonstrinn i administrasjonssenteret. Velg Hjem i navigasjonsruten **for** å fullføre eventuelle ekstra konfigurasjonstrinn.

> [!NOTE]
> Du vil motta en prorated refundering for Microsoft 365 lisenser som du ikke lenger trenger. Bankkontoen eller kredittkortet belastes omtrent to dager etter at du har konfigurert det nye abonnementet.
  
## <a name="protect-user-devices-and-files"></a>Beskytt brukerenheter og filer

Nå som Microsoft 365 Business Premium lisenser er tilordnet, kan du fullføre trinnene for å begynne å beskytte enheter og filer. Du bruker noen nye alternativer som er inkludert i navigasjonsruten i administrasjonssenteret.
  
1. Gå til Enheter policyer i navigasjonsruten i  \> **administrasjonssenteret.**

2. Velg Legg **til på siden Enhetspolicyer.** 

3. Gi **policyen et** navn (for eksempel Beskytt arbeidsfiler) i Legg til policy-ruten, og velg deretter en **policytype** fra rullegardinlisten.

    Du kan konfigurere programpolicyer for å beskytte filer på Android- og iPhone-enheter samt Windows 10, og du kan konfigurere policyer for enhetskonfigurasjon for firmaeide Windows 10 enheter. Se følgende koblinger for mer informasjon:

    - [Angi innstillinger for appbeskyttelse på Android- eller iOS-enheter](app-protection-settings-for-android-and-ios.md)

    - [Angi innstillinger for appbeskyttelse for Windows 10-enheter](protection-settings-for-windows-10-devices.md)

    - [Angi innstillinger for enhetsbeskyttelse for Windows 10 PC-er](protection-settings-for-windows-10-pcs.md)

4. Når du har konfigurert policyer, kan du og de ansatte konfigurere enheter:

    - Hvis Windows ikke allerede bruker Windows Pro Creator-oppdateringen, må du oppgradere dem til Windows Pro [Creators Update](upgrade-to-windows-pro-creators-update.md).

    - Se [Konfigurere Windows for Microsoft 365 Business Premium for](set-up-windows-devices.md) trinn for Windows enheter.

    - Se [Konfigurere mobile enheter for Microsoft 365 Business Premium for](set-up-mobile-devices.md) trinn for Android-telefoner og iPhone.