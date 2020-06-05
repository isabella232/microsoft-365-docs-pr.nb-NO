---
title: Aktivere domene-sammenføyde Windows 10-enheter som skal administreres av Microsoft 365 for bedrifter
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
- Adm_O365
- Core_O365Admin_Migration
- MiniMaven
- MSB365
- OKR_SMB_M365
- seo-marvel-mar
- AdminSurgePortfolio
search.appverid:
- BCS160
- MET150
description: Lær hvordan du aktiverer Microsoft 365 til å beskytte lokale Active-Directory-tilkoblede Windows 10-enheter med bare noen få trinn.
ms.openlocfilehash: 857651081fb10856d28dd419333ebef655388407
ms.sourcegitcommit: e6e704cbd9a50fc7db1e6a0cf5d3f8c6cbb94363
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/04/2020
ms.locfileid: "44564954"
---
# <a name="enable-domain-joined-windows-10-devices-to-be-managed-by-microsoft-365-business-premium"></a>Aktivere domeneblede Windows 10-enheter som skal administreres av Microsoft 365 Business Premium

Hvis organisasjonen bruker lokal Windows Server Active Directory, kan du konfigurere Microsoft 365 Business Premium til å beskytte Windows 10-enhetene, samtidig som du opprettholder tilgangen til lokale ressurser som krever lokal godkjenning.
Hvis du vil konfigurere denne beskyttelsen, kan du implementere **Hybrid Azure AD sammenføyde enheter**. Disse enhetene er koblet til både den lokale Active Directory og Azure Active Directory.

Denne videoen beskriver fremgangsmåten for hvordan du konfigurerer dette for det vanligste scenariet, som også er beskrevet i trinnene som følger.

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE3C9hO]
  

## <a name="before-you-get-started-make-sure-you-complete-these-steps"></a>Før du kommer i gang, må du sørge for at du fullfører disse trinnene:
- Synkroniser brukere til Azure AD med Azure AD Connect.
- Fullfør Azure AD Connect Organizational Unit (OU)-synkronisering.
- Kontroller at alle domenebrukerne du synkroniserer, har lisenser til Microsoft 365 Business Premium.

Se [Synkronisere domenebrukere til Microsoft](manage-domain-users.md) for fremgangsmåten.

## <a name="1-verify-mdm-authority-in-intune"></a>1. Kontroller MDM-myndigheten i Intune

Gå til portal.azure.com og øverst på siden søker du etter Intune.
Velg **Enhetsregistrering** på Siden Microsoft Intune, og kontroller at **MDM-myndighet** er Intune på **Siden Microsoft** **Intune.**

- Hvis **MDM-myndighet** er **Ingen**, klikker du **MDM-myndigheten** for å sette den til **Intune**.
- Hvis **MDM-myndighet** er **Microsoft Office 365**, går du til **Enheter**  >  **Registrer enheter** og bruker dialogboksen Legg til **MDM-myndighet** til høyre for å legge til **Intune MDM-myndighet** (dialogboksen **Legg til MDM Authority** er bare tilgjengelig hvis **MDM Authority** er satt til Microsoft Office 365).

## <a name="2-verify-azure-ad-is-enabled-for-joining-computers"></a>2. Kontroller at Azure AD er aktivert for sammenføyning av datamaskiner

- Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> på, og velg **Azure Active Directory** (velg Vis alle hvis Azure Active Directory ikke er synlig) i listen over **administrasjonssentre.** 
- Gå til **Azure Active Directory** i **administrasjonssenteret**for Azure Active Directory , velg **Enheter** og deretter **Enhetsinnstillinger**.
- Kontroller at**brukere kan koble enheter til Azure AD** er aktivert 
    1. Hvis du vil aktivere alle brukere, setter du til **Alle**.
    2. Hvis du vil aktivere bestemte brukere, setter du til **Valgt** for å aktivere en bestemt gruppe brukere.
        - Legg til de ønskede domenebrukerne som er synkronisert i Azure AD i en [sikkerhetsgruppe](../admin/create-groups/create-groups.md).
        - Velg **Velg grupper** for å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.

## <a name="3-verify-azure-ad-is-enabled-for-mdm"></a>3. Kontroller at Azure AD er aktivert for MDM

- Gå til administrasjonssenteret <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">https://admin.microsoft.com</a> på, og velg **Endepunktsbehandler**t (velg **Vis alt** hvis **Endpoint Manager** ikke er synlig)
- Gå til **Enheter**Automatisk registrering av Windows **Microsoft Endpoint Manager admin center**  >  **Windows**  >  **Windows-registrering**  >  **Automatic Enrollment**i administrasjonssenteret for Microsoft Endpoint Manager .
- Kontroller at MDM-brukeromfang er aktivert.

    1. Hvis du vil registrere alle datamaskiner, kan du sette til **Alle** for å registrere alle brukerdatamaskiner som er koblet til Azure AD og nye datamaskiner når brukerne legger til en arbeidskonto i Windows.
    2. Sett til **Noen** for å registrere datamaskinene til en bestemt gruppe brukere.
        -  Legg til de ønskede domenebrukerne som er synkronisert i Azure AD i en [sikkerhetsgruppe](../admin/create-groups/create-groups.md).
        -  Velg **Velg grupper** for å aktivere MDM-brukeromfang for denne sikkerhetsgruppen.

## <a name="4-set-up-service-connection-point-scp"></a>4. Konfigurere tjenestetilkoblingspunkt (SCP)

Disse trinnene er forenklet fra [å konfigurere hybrid azure AD-sammenføyning](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains#configure-hybrid-azure-ad-join). For å fullføre trinnene må du bruke Azure AD Connect og Microsoft 365 Business Premium globale administrator og Active Directory admin passord.

1.  Start Azure AD Connect, og velg deretter **Konfigurer**.
2.  Velg **Konfigurer enhetsalternativer på**Flere **oppgaver-siden,** og velg deretter **Neste**.
3.  Velg **Neste**på **Oversikt-siden.**
4.  Angi legitimasjonen til en global administrator for Microsoft 365 Business Premium på siden **Koble til Azure AD.**
5.  Velg **Konfigurer Hybrid Azure AD-sammenføyning på**siden **Enhetsalternativer,** og velg deretter **Neste**.
6.  Fullfør **SCP** følgende trinn for hver skog der du vil at Azure AD Connect skal konfigurere SCP, fullføre følgende trinn for hver skog der du vil at Azure AD Connect skal konfigurere SCP, fullføre følgende trinn, og velg deretter **Neste:**
    - Merk av i boksen ved siden av skogsnavnet. Skogen skal være ad-domenenavnet ditt.
    - Åpne rullegardinlisten under **Godkjenningstjeneste-kolonnen,** og velg samsvarende domenenavn (det bør bare være ett alternativ).
    - Velg **Legg til** for å angi legitimasjonen for domeneadministrator.  
7.  Velg bare Windows 10 eller senere domenet som er sammenkoblet på siden **Enhetsoperativsystemer.**
8.  Velg **Konfigurer**på siden **Klar til å konfigurere.**
9.  Velg **Avslutt**på siden **Konfigurasjon fullført.**


## <a name="5-create-a-gpo-for-intune-enrollment--admx-method"></a>5. Opprett et gruppepolicyobjekt for Intune-registrering – ADMX-metoden

Bruke. ADMX-malfilen.

1.  Logg deg på AD-server, søk og åpne **Gruppepolicybehandling**for Server  >  **Manager-verktøy**  >  **Group Policy Management**.
2.  Velg domenenavnet ditt under **Domener,** og høyreklikk **Gruppepolicyobjekter** for å velge **Ny**.
3.  Gi det nye gruppepolicyobjektet et navn, for eksempel "*Cloud_Enrollment*" og velg deretter **OK**.
4.  Høyreklikk det nye Gruppepolicyobjektet under **Gruppepolicyobjekter,** og velg **Rediger**.
5.  I **redigeringsprogrammet for gruppepolicybehandling**går du til Administrative maler for **Computer Configuration**  >  **Policies**  >  **datamaskinkonfigurasjonspolicyer**  >  **Windows-komponenter**  >  **MDM**.
6. Høyreklikk **Aktiver automatisk MDM-registrering ved hjelp av standard Azure AD-legitimasjon,** og velg deretter **Aktivert**  >  **OK**. Lukk redigeringsvinduet.

> [!IMPORTANT]
> Hvis du ikke ser policyen **Aktiver automatisk MDM-registrering ved hjelp av standard Azure AD-legitimasjon**, kan du se [Få de nyeste administrative malene](#get-the-latest-administrative-templates).

## <a name="6-deploy-the-group-policy"></a>6. Distribuere gruppepolicyen

1.  I Serverbehandling, under **Domener** > gruppepolicyobjekter, velger du Gruppepolicyobjektene fra trinn 3 ovenfor, for eksempel "Cloud_Enrollment".
2.  Velg **Omfang-fanen** for gruppepolicyobjektet.
3.  Høyreklikk koblingen til domenet under **Koblinger**i kategorien Omfang i gruppepolicyobjektet.
4.  Velg **Fremtving** for å distribuere Gruppepolicyobjektet og deretter **OK** i bekreftelsesskjermbildet.

## <a name="get-the-latest-administrative-templates"></a>Få de nyeste administrative malene

Hvis du ikke ser policyen **Aktiver automatisk MDM-registrering ved hjelp av standard Azure AD-legitimasjon**, kan det skyldes at du ikke har ADMX installert for Windows 10, versjon 1803, versjon 1809 eller versjon 1903. Hvis du vil løse problemet, følger du denne fremgangsmåten (Merk: Den nyeste MDM.admx er bakoverkompatibel):

1.  Last ned: [Administrative maler (ADMX) for Windows 10 mai 2019 Oppdatering (1903)](https://www.microsoft.com/download/details.aspx?id=58495&WT.mc_id=rss_alldownloads_all).
2.  Installere pakken på den primære domenekontrolleren (PDC).
3.  Naviger, avhengig av hvilken versjon til mappen: **C:\Programfiler (x86)\Microsoft gruppepolicy\Windows 10 Mai 2019 Oppdatering (1903) v3**.
4.  Gi nytt navn til **policydefinisjoner-mappen** i banen ovenfor til **PolicyDefinitions**.
5.  Kopier **PolicyDefinitions-mappen** til **C:\Windows\SYSVOL\domain\Policies**. 
    -   Hvis du planlegger å bruke et sentralt policylager for hele domenet, legger du til innholdet i PolicyDefinitions der.
6.  Start den primære domenekontrolleren på nytt for at policyen skal være tilgjengelig. Denne prosedyren vil fungere for alle fremtidige versjoner også.

På dette tidspunktet bør du kunne se policyen **Aktiver automatisk MDM-registrering ved hjelp av standard Azure AD-legitimasjon** tilgjengelig.

