---
title: Verbinding maken met Meta-advertenties
description: Sluit een Meta Ads-account aan om uw advertenties en media te activeren en te controleren met Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
recommendations: noDisplay
feature: Reporting and Insights
exl-id: 78110edf-947b-4e05-a3f1-de4b1eabda44
source-git-commit: dce3d9bbf3ed2d26872b324c04ab7e78bbb034dc
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---

# Verbinding maken met Meta-advertenties

Op deze pagina wordt uitgelegd hoe u een verbinding tot stand kunt brengen tussen uw Meta Ads-profielaccount en uw Ads-profielaccount kunt beheren met GenStudio for Performance Marketing om campagnes te beheren, inhoud te exporteren en toegang te krijgen tot advertentiegegevens voor uw actieve campagnes.

>[!BEGINSHADEBOX]

**Eerste vereisten**:

- Een Facebook/Meta-aanmelding die toegang biedt tot alle Meta-services
- _Volledige controle_ over de Bedrijfs Portfolio van Meta en Advertentierekeningen, die omvatten:
   - Campagnes beheren
   - Prestaties weergeven
   - Creative Hub-modellen beheren
   - Geavanceerde analysemogelijkheden
- Pop-upblokkeerprogramma&#39;s in uw browser uitschakelen
- Controleer of er koppelingen naar installateurspagina&#39;s zijn in Meta Business Manager voordat u verbinding maakt
- Beheerderstoegang bevestigen voor alle middelen die worden verbonden

>[!ENDSHADEBOX]

## Een Meta Ads-account verbinden

1. Klik op **[!UICONTROL More]** > **[!UICONTROL Settings]** .

1. In de _schakelaars van Gegevens_ sectie, klik **[!UICONTROL Connect]** op _Meta Adds_ kaart.

1. Log in bij je Facebook account.

   U moet mogelijk de pop-upblokkeerprogramma&#39;s verwijderen en vervolgens **[!UICONTROL Refresh]** gebruiken om het opnieuw te proberen.

1. Volg de Facebook-verificatieinstructies, controleer de accountgegevens en klik op **[!UICONTROL Continue as ...]**

1. Ga in _[!UICONTROL Facebook Login for Business]_(symbool Meta naar Adobe) door de volgende selecties om GenStudio for Performance Marketing toegang te verlenen:

   - Selecteer een of meer Meta Business-profielen en klik op **[!UICONTROL Continue]**
   - Selecteer een of meer Meta-pagina&#39;s en klik op **[!UICONTROL Continue]**
   - Selecteer een of meer Instagram-accounts en klik op **[!UICONTROL Continue]**
   - Selecties bekijken en klikken **[!UICONTROL Save]**

     ![ de selecties van het Overzicht ](/help/assets/meta/meta-review-selections.png " Selecties van het Overzicht "){width="400" zoomable="yes"}

1. Klik op **[!UICONTROL Got it]** wanneer u hebt gecontroleerd of uw account is verbonden.

   Deze stap zorgt ervoor dat GenStudio for Performance Marketing toegang krijgt tot alle advertenties, metagegevens en meetgegevens voor optimale prestaties.

1. Selecteer in _[!UICONTROL Meta Ads]_een of meer accounts die u wilt opnemen in [!DNL Insights] en klik op **[!UICONTROL Select]**.

1. Zodra u a _Platform verbonden_ bevestiging ontvangt, klik **[!UICONTROL View accounts]**.

   In de weergave _[!UICONTROL Meta Ads accounts]_worden de `Account name` , `Added by` , `Date added` en `Status` weergegeven.

   ![ de rekeningenlijst van Meta ](/help/assets/meta/meta-accounts-list.png " Lijst van verbonden rekeningen van Meta "){zoomable="yes"}

Gebruik **[!UICONTROL Add account]** om meer accounts aan de lijst toe te voegen. De machtigingsstroom kan enigszins afwijken wanneer u accounts toevoegt die zijn gekoppeld aan hetzelfde Meta Business-profiel. U selecteert alleen de nieuwe Meta Ads-accounts tijdens het verbindingsproces.

## Aanbevolen werkwijzen voor verbindingen

Als u fouten wilt voorkomen, moet u rekening houden met de volgende aanbevolen procedures bij het instellen van verbindingen:

- [ ] Beginnen met minimale selectie van elementen (alleen één pagina) voor de eerste verbinding
- [ ] Voeg alleen Instagram-accounts toe nadat u hebt bevestigd dat toegang tot de pagina werkt
- [ ] Controleer of Instagram-accounts correct zijn gekoppeld aan de geselecteerde Facebook-pagina in Meta Business Manager
- [ ] Gebruik een gefaseerde aanpak: maak eerst een basisverbinding en vouw vervolgens elementen uit
- [ ] Controleer de beheerdersmachtigingen voor alle elementen voordat u verbinding probeert

## Verbinding maken en problemen oplossen bij de integratie met Meta Ads

Soms wordt een GenStudio for Performance Marketing-exemplaar onjuist verbonden met een Meta Ads-account. Veelvoorkomende instellingen die problemen kunnen veroorzaken zijn:

- Een Instagram-account is geselecteerd zonder de bijbehorende Facebook-pagina te selecteren
- Ingetrokken machtigingen voor een gebruiker die de eerste verbinding heeft uitgevoerd

In deze situaties is het beter om de Meta Ad-account opnieuw te verbinden met het GenStudio for Performance Marketing-exemplaar. Eerst moet de gebruiker de integratie van de app rechtstreeks verwijderen uit de Meta Business Manager en een schone lei maken voor het opnieuw instellen van machtigingen. Hiervoor hebt u beheerderstoegang tot de Meta Business Manager nodig.

Deze stappen ontruimen caching toestemmingen en stellen de integratiestroom opnieuw in:

1. Heb toegang tot [ Van Bedrijfs Meta Manager ](https://business.facebook.com) door de website van Facebook te bezoeken.
1. Meld u aan bij uw account. De account moet beheerdersrechten hebben voor de Business Manager.
1. Klik op het cogopictogram **[!UICONTROL Settings]** linksonder om naar uw Business Portfolio-instellingen te navigeren.
1. Klik in het linkermenu op **[!UICONTROL Integrations]** .
1. Selecteer **[!UICONTROL Connected Apps]**. Adobe GenStudio wordt weergegeven in de lijst met verbonden apps.
   ![ Van Bedrijfs Meta Manager Verbonden Apps ](./meta-connected-apps.png " Meta Business Manager Verbonden Apps ruit ")
1. Klik op de naam van de toepassing.
1. Klik op **[!UICONTROL Remove]**.
1. Bevestig de verwijdering wanneer daarom wordt gevraagd.

U kunt nu opnieuw verbinding maken met Meta Ad Accounts, Instagram-profielen en Facebook-pagina&#39;s.

## Verbindingsproblemen met een Instagram-account

Problemen kunnen optreden wanneer Instagram-accounts worden geselecteerd zonder een gekoppelde Facebook-pagina te verbinden tijdens het instellen van de verbinding. Dit kan fouten veroorzaken zoals:

- Kan geen verbinding maken met {Page_Name} of generieke verbindingsfouten.
- Time-outs voor verbinding tijdens Facebook-aanmelding voor bedrijfsstroom.
- Stille fouten wanneer meerdere elementen zijn geselecteerd.
- Verbinding mislukt wanneer u tegelijkertijd Installagram en Pagina- en Advertentieaccount selecteert.

### Stappen voor resolutie:

1. Navigeer aan [ BedrijfsManager van Meta ](https://business.facebook.com) > Integraties > Verbonden Toepassingen.
1. Verwijder de bestaande &quot;Adobe GenStudio&quot;-integratie, als die er is. Klik **verwijderen**.
1. Ga terug naar GenStudio en probeer het verbindingsproces opnieuw.
1. Selecteer ALLEEN de doel-Facebook-pagina tijdens de eerste verbinding.
1. Selecteer NIET het Instagram-account tijdens de eerste verbindingspoging.
1. Controleer of de verbinding tot stand is gebracht voordat u andere elementen toevoegt.
1. Als de verbinding met de pagina stabiel is, voegt u afzonderlijke Instagram-accounts toe.


