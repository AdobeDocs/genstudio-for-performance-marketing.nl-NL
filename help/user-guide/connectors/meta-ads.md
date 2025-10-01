---
title: Verbinding maken met Meta-advertenties
description: Sluit een Meta Ads-account aan om uw advertenties en media te activeren en te controleren met Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
recommendations: noDisplay
feature: Reporting and Insights
exl-id: 78110edf-947b-4e05-a3f1-de4b1eabda44
source-git-commit: fb5fe4885340639f8179c8de6944ac21bfe009ec
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Verbinding maken met Meta-advertenties

Op deze pagina wordt uitgelegd hoe u een verbinding tot stand kunt brengen tussen uw Meta Ads-profielaccount en uw Ads-profielaccount kunt beheren met GenStudio for Performance Marketing om campagnes te beheren, inhoud te exporteren en toegang te krijgen tot advertentiegegevens voor uw actieve campagnes.

>[!BEGINSHADEBOX]

**Eerste vereisten**:

- Aanmelden bij Facebook/Meta voor toegang tot alle Meta-services

- _Volledige controle_ over de Bedrijfs Portfolio van Meta en Advertentierekeningen, die omvatten:

   - Campagnes beheren
   - Prestaties weergeven
   - Creative Hub-modellen beheren
   - Geavanceerde analysemogelijkheden

- Pop-upblokkeerprogramma&#39;s in uw browser uitschakelen

>[!ENDSHADEBOX]

## Een Meta-advertentieaccount verbinden

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

     ![&#x200B; de selecties van het Overzicht &#x200B;](/help/assets/meta/meta-review-selections.png " Selecties van het Overzicht "){width="400" zoomable="yes"}

1. Klik op **[!UICONTROL Got it]** wanneer u hebt gecontroleerd of uw account is verbonden.

   Deze stap zorgt ervoor dat GenStudio for Performance Marketing toegang krijgt tot alle advertenties, metagegevens en meetgegevens voor optimale prestaties.

1. Selecteer in _[!UICONTROL Meta Ads]_&#x200B;een of meer accounts die u wilt opnemen in [!DNL Insights] en klik op **[!UICONTROL Select]**.

1. Zodra u a _Platform verbonden_ bevestiging ontvangt, klik **[!UICONTROL View accounts]**.

   In de weergave _[!UICONTROL Meta Ads accounts]_&#x200B;worden de `Account name` , `Added by` , `Date added` en `Status` weergegeven.

   ![&#x200B; de rekeningenlijst van Meta &#x200B;](/help/assets/meta/meta-accounts-list.png " Lijst van verbonden rekeningen van Meta "){zoomable="yes"}

Gebruik **[!UICONTROL Add account]** om meer accounts aan de lijst toe te voegen. De machtigingsstroom kan enigszins afwijken wanneer u accounts toevoegt die zijn gekoppeld aan hetzelfde Meta Business-profiel. U selecteert alleen de nieuwe Meta Ads-accounts tijdens het verbindingsproces.

## Verbinding maken en problemen oplossen bij de integratie met Meta Ads

Soms wordt een GenStudio for Performance Marketing-exemplaar onjuist verbonden met een Meta Ads-account. Veelvoorkomende instellingen die problemen kunnen veroorzaken zijn:

- Een Instagram-account is geselecteerd zonder de bijbehorende Facebook-pagina te selecteren
- Ingetrokken machtigingen voor een gebruiker die de eerste verbinding heeft uitgevoerd

In deze situaties is het beter om de Meta Ad-account opnieuw te verbinden met het GenStudio for Performance Marketing-exemplaar. Eerst moet de gebruiker de integratie van de app rechtstreeks verwijderen uit de Meta Business Manager en een schone lei maken voor het opnieuw instellen van machtigingen. Hiervoor hebt u beheerderstoegang tot de Meta Business Manager nodig.

Deze stappen ontruimen caching toestemmingen en stellen de integratiestroom opnieuw in:

1. Heb toegang tot [&#x200B; Van Bedrijfs Meta Manager &#x200B;](https://business.facebook.com) door de website van Facebook te bezoeken.
1. Meld u aan bij uw account. De account moet beheerdersrechten hebben voor de Business Manager.
1. Klik op het cogopictogram **[!UICONTROL Settings]** linksonder om naar uw Business Portfolio-instellingen te navigeren.
1. Klik in het linkermenu op **[!UICONTROL Integrations]** .
1. Selecteer **[!UICONTROL Connected Apps]**. Adobe GenStudio wordt weergegeven in de lijst met verbonden apps.
   ![&#x200B; Van Bedrijfs Meta Manager Verbonden Apps &#x200B;](./meta-connected-apps.png " Meta Business Manager Verbonden Apps ruit ")
1. Klik op de naam van de toepassing.
1. Klik op **[!UICONTROL Remove]**.
1. Bevestig de verwijdering wanneer daarom wordt gevraagd.

U kunt nu opnieuw verbinding maken met uw Meta-advertentieaccounts, Instagram-profielen en Facebook-pagina&#39;s.
