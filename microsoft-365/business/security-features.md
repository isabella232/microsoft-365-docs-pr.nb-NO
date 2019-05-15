---
title: Sikkerhetsfunksjonene i Microsoft 365 Business
ms.author: sirkkuw
author: Sirkkuw
manager: scotv
audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ms.collection:
- M365-subscription-management
- M365-security-compliance
ms.custom:
- Core_O365Admin_Migration
- MiniMaven
- MSB365
search.appverid:
- BCS160
- MET150
ms.assetid: c123694a-1efb-459e-a8d5-2187975373dc
description: Lær mer om sikkerhetsfunksjonene som følger med Microsoft 365 Business.
ms.openlocfilehash: 6ce69f387461edc0eea6c705f15a9083547698ff
ms.sourcegitcommit: 66bb5af851947078872a4d31d3246e69f7dd42bb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/15/2019
ms.locfileid: "34074534"
---
# <a name="microsoft-365-business-security-features"></a>Sikkerhetsfunksjonene i Microsoft 365 Business

Microsoft 365 Business tilbyr forenklet sikkerhetsfunksjoner til å beskytte dine data på PCer, telefoner og tavler.
    
## <a name="microsoft-365-business-admin-center-security-features"></a>Sikkerhetsfunksjonene i Microsoft 365 Business admin center

![Banner som peker til https://aka.ms/aboutM365preview.](media/m365admincenterchanging.png)

Du kan behandle mange av sikkerhetsfunksjonene for Microsoft 365 Business i administrasjonssenteret, som gir deg en enklere måte å slå disse funksjonene på eller av. I administrasjonssenteret kan du gjøre følgende:
  
![Screenshot of the Devices card in the admin center](media/9982e784-dbf9-4a76-a159-bb3e2e5aa23f.png)
  
- [Angi innstillinger for programmet for Android eller iOS-enheter](app-protection-settings-for-android-and-ios.md) . 
    
    Disse innstillingene omfatter sletter filer fra en inaktiv enheten etter en angitt periode, kryptere arbeidsfiler, som krever at brukere angir en PIN-kode, og så videre.
    
- [Angi innstillinger for programmet for Windows 10 enheter](protection-settings-for-windows-10-devices.md) . 
    
    Disse innstillingene kan brukes til firmadataene på begge eies av firmaet eller personlig eies enheter.
    
- [Angi innstillinger for enhet for Windows 10 enheter](protection-settings-for-windows-10-pcs.md) . 
    
    Du kan aktivere [BitLocker](https://go.microsoft.com/fwlink/p/?linkid=871405) -kryptering til å beskytte dataene i tilfelle en enhet er mistet eller stjålet, og aktiverer [Windows utnytte Guard](https://go.microsoft.com/fwlink/p/?linkid=871404) til gir avansert beskyttelse mot ransomware. 
    
- [Fjerne firmadata fra enheter](remove-company-data.md)
    
    Du kan tørke firmadata eksternt hvis en enhet blir stjålet, eller en ansatt forlater firmaet.
    
- [Tilbakestille Windows-10 enheter til fabrikkinnstillinger](reset-devices-to-factory-settings.md) . 
    
    Du kan tilbakestille Windows 10-enheter som har Enhetsinnstillinger for databeskyttelse brukes.
    
## <a name="additional-security-features"></a>Ekstra sikkerhetsfunksjoner 

Avanserte funksjoner i Microsoft 365 Business er tilgjengelig for å hjelpe deg med å beskytte bedriften mot cyber trusler og beskytte sensitiv informasjon.
  
- **[Office 365 avanserte Threat Protection](https://support.office.com/article/e100fe7c-f2a1-4b7d-9e08-622330b83653)**
    
    Avansert Threat Protection (ATP) verne bidrar til å bedriften mot avanserte phishing og ransomware angrep som er laget for å bryte ansatt eller kundeinformasjon. Funksjoner:
    
  - Avanserte vedlegg skanning og AI-drevet analyse for å oppdage og fjerne farlige meldinger.
    
  - Automatisk kontrollerer web-koblinger i e-post for å vurdere om de er en del av et phishing-forsøk. Dette holder deg sikker tilgang til usikre webområder.
    
- **[Oversikt over datapolicyer tap forebygging](https://support.office.com/article/1966b2a7-d1e2-4d92-ab61-42efbb137f5e)** (DLP). 
    
    Du kan definere DLP til å automatisk gjenkjenne sensitiv informasjon, som kredittkortnumre, personnummer, etc. å forhindre deres utilsiktet deling utenfor firmaet.
    
- **[Exchange Online Archiving](https://products.office.com/exchange/microsoft-exchange-online-archiving-email)**
    
    Exchange Online-arkivering lisens gjør at meldingene kan lett bli arkivert med sammenhengende data backup. Den lagrer alt i en brukers e-postmeldinger, inkludert Slettede elementer, i tilfelle de kreves for gjenkjenning eller gjenoppretting senere. Du kan også bruke ulike oppbevaringspolicyer å beholde e-data for rettstvist sperringer, eDiscovery, eller for å oppfylle krav til samsvar.
    
- **[Azure informasjonsbeskyttelse](https://go.microsoft.com/fwlink/p/?linkid=871406)**
    
    Informasjon om beskyttelse hjelper du styre tilgang til sensitiv informasjon i e-post og dokumenter med kontroller som "Ikke Videresend" og "Kopieres ikke". Du kan klassifisere sensitiv informasjon som "Konfidensielt", og du kan angi hvordan klassifisert informasjon kan deles utenfor og innenfor virksomheten. Bedriftsnivå kryptering er enkelt å bruke e-post og dokumenter til å holde informasjonen din privat. Microsoft 365 Business inneholder alle funksjonene i [Azure informasjon beskyttelse Plan 1](https://go.microsoft.com/fwlink/p/?linkid=871407). Du kan også installere tillegget for beskyttelse mot Azure-informasjon-klienten for Office-programmer. Hvis du vil ha mer informasjon, kan du se [Azure informasjonsbeskyttelse klienten administratoren guide](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide).
    
- **[Alle egenskapene i Intune i Azure portal](https://go.microsoft.com/fwlink/p/?linkid=871403)**
    
    Tilgang til Intune administrasjonssenteret i Azure portal kan du definere ytterligere sikkerhetsfunksjoner, for eksempel administrasjon av MacOS enheter, iPhone og Android enheter sammen med avansert Enhetsbehandling for Windows, som ikke er tilgjengelige via Microsoft 365 business administrasjonssenteret.
    
De neste avsnittene beskriver hvordan du kan administrere disse funksjonene i sikkerheten &amp; overholdelsessenteret og Intune administrasjonssenteret. Forenklet kontrollene vil bli lagt til administrasjonssenteret for Microsoft 365 Business over tid.
  
    
## <a name="faq"></a>Vanlige spørsmål

 ### <a name="are-these-security-features-available-in-all-markets"></a>Er disse sikkerhetsfunksjonene som er tilgjengelige i alle markeder?
  
Ja, disse funksjonene er tilgjengelige i alle land der Microsoft 365 Business selges.
  
### <a name="how-do-i-find-the-security-amp-compliance-center"></a>Hvordan finner jeg sikkerheten &amp; overholdelsessenteret?
  
1. [Logg på Microsoft 365 Business](https://portal.microsoft.com/) ved hjelp av admin-rettigheter. 
    
2. I den venstre nav, Finn **centers Admin** og utvide den. 
    
    ![Velg Admin-sentre i den venstre nav i administrasjonssenteret for Microsoft 365.](media/fa4484f8-c637-45fd-a7bd-bdb3abfd6c03.png)
  
3. Velg **Sikkerhet &amp; kompatibilitet** å gå til sikkerhet &amp; overholdelsessenteret.