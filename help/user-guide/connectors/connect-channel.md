---
title: Betaalde media aansluiten
description: Verbind een kanaalaccount om uw advertenties en media te activeren en te controleren met Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: cf4be61925761c9630cb8ea5c995d017b3938a31
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Betaalde mediaaccounts verbinden

_[!DNL Data connectors]_&#x200B;maakt naadloze integratie mogelijk tussen GenStudio for Performance Marketing en uw betaalmedia netwerkaccounts. Door verbinding te maken met kanaalaccounts van derden, kunt u kritieke gegevens uitwisselen, zoals maatstaven voor campagneprestaties in [[!DNL Insights]](/help/user-guide/insights/overview.md) , en kunt u nieuwe ad-hoclocaties aanbieden met [[!DNL Activate]](/help/user-guide/activation/overview.md) . Dankzij deze integratie kan GenStudio for Performance Marketing uw media en advertenties beheren en tegelijkertijd waardevolle inzichten uit uw actieve campagnes krijgen, zoals afbeeldingen, klikken en conversies.

**om met een betaalde media rekening** te verbinden:

1. Klik op de ellips **[!UICONTROL ... More]** in de navigatie linksonder.

1. Selecteer **[!UICONTROL Settings]** met het cogopictogram.

1. Kies in _[!UICONTROL Settings]_&#x200B;een verbindingstype in de sectie&#x200B;_[!UICONTROL Data connectors]_ en klik op **[!UICONTROL Connect]** .

   Naar keuze, als er verbonden rekeningen zijn, kunt u op _verbonden rekeningen_ klikken om een lijst van rekeningsnamen, details, en status te bekijken.

1. Zie het [ schakelaartype ](#connector-types) u selecteerde, herzie de eerste vereisten, en ga met de verbindingsstappen verder.

## Betaalde media

GenStudio for Performance Marketing biedt ondersteuning voor verschillende connectortypen die u kunt integreren met uw favoriete marketingplatforms. Elk schakelaartype heeft specifieke eerste vereisten en opstellingsstappen om voor een succesvolle verbinding te voltooien.

### Google Campagne Manager 360 connect

>[!BEGINSHADEBOX]

**Eerste vereisten**:

- Google Campagne Manager 360-account
- Pop-upblokkeerprogramma&#39;s in uw browser verwijderen

>[!ENDSHADEBOX]

**om een Google Manager 360 van de Campagne te verbinden rekening**:

1. In de _schakelaars van Gegevens_ sectie, klik **[!UICONTROL Connect]** op _Google Manager 360_ kaart van de Campagne.

1. Meld u aan bij uw Google Campagne Manager 360-account.

   U moet mogelijk de pop-upblokkeerprogramma&#39;s verwijderen en vervolgens **[!UICONTROL Refresh]** gebruiken om het opnieuw te proberen.

1. Lees de voorwaarden en voorwaarden en klik op **[!UICONTROL Allow]** om toegang te verlenen.

1. Selecteer een of meer adverteerders in de weergave _[!UICONTROL Google Campaign Manager 360]_&#x200B;en klik op **[!UICONTROL Select]**.

In de weergave _[!UICONTROL Google Campaign Manager 360 accounts]_&#x200B;worden de `Account name` , `Added by` , `Date added` en `Status` weergegeven. Gebruik **[!UICONTROL Add account]**&#x200B;om meer accounts aan de lijst toe te voegen.

### Meta-advertenties verbinden

Wanneer u uw _Van Bedrijfs Meta_ profiel met GenStudio for Performance Marketing verbindt, verzekert het naadloze toegang tot reclamegegevens voor uw bedrijfspagina&#39;s, de rekeningen van Meta Adds, en andere activa van Meta.

>[!BEGINSHADEBOX]

**Eerste vereisten**:

- Facebook/Meta-aanmelding die toegang kan krijgen tot alle Meta-services, zoals het Meta Ads-account en het Facebook Business Profile
- Toegang tot een Meta-advertentiesaccount met `View performance` machtigingsniveau voor het openen van rapporten en het weergeven van advertenties, waaronder de volgende
   - Machtigingen vereist voor gebruik met [!DNL Insights] :

      - `pages_show_list`
      - `ads_read`
      - `ads_management`
      - `pages_read_engagement`

   - Machtigingen vereist voor gebruik met [!DNL Activate] :

      - `ads_management`
      - `ads_read`
      - `business_management`
      - `instagram_basic`
      - `instagram_content_publish`
      - `pages_manage_ads`
      - `pages_manage_posts`
      - `pages_show_list`

- Pop-upblokkeerprogramma&#39;s in uw browser verwijderen

>[!ENDSHADEBOX]

**om een Meta-advertentierekening** te verbinden:

1. In de _sectie van 0&rbrace; Verbindingen van Gegevens &lbrace;, klik **[!UICONTROL Connect]**&#x200B;op de_ Advertentiekaart van Meta _._

1. Log in bij je Facebook account.

   U moet mogelijk de pop-upblokkeerprogramma&#39;s verwijderen en vervolgens **[!UICONTROL Refresh]** gebruiken om het opnieuw te proberen.

1. Volg de Facebook-verificatieinstructies, controleer de accountgegevens en klik op **[!UICONTROL Continue as ...]**

1. Ga in _[!UICONTROL Facebook Login for Business]_(Symbool Meta t/m Adobe) door de volgende selecties om GenStudio for Performance Marketing toegang te verlenen:

   - Selecteer een of meer zakelijke profielen voor metagegevens en klik op **[!UICONTROL Continue]**
   - Selecteer een of meer metapagina&#39;s en klik op **[!UICONTROL Continue]**
   - Selecteer een of meer Instagram-accounts en klik op **[!UICONTROL Continue]**
   - Selecties bekijken en klikken **[!UICONTROL Save]**

1. Klik op **[!UICONTROL Got it]** wanneer u hebt gecontroleerd of uw account is verbonden.

   Deze stap zorgt ervoor dat GenStudio for Performance Marketing toegang krijgt tot alle advertenties, metagegevens en meetgegevens voor optimale prestaties.

1. Selecteer in _[!UICONTROL Meta Ads]_&#x200B;een of meer accounts die u wilt opnemen in [!DNL Insights] en klik op **[!UICONTROL Select]**.

1. Zodra u a _Platform verbonden_ bevestiging ontvangt, klik **[!UICONTROL View accounts]**.

   In de weergave _[!UICONTROL Meta Ads accounts]_&#x200B;worden de `Account name` , `Added by` , `Date added` en `Status` weergegeven.

Gebruik **[!UICONTROL Add account]** om meer accounts aan de lijst toe te voegen. De machtigingsstroom kan enigszins afwijken wanneer u accounts toevoegt die zijn gekoppeld aan hetzelfde Meta Business-profiel. Tijdens het verbindingsproces selecteert u alleen de nieuwe metagegevensaccounts.

## Gegevensinvoer

In eerste instantie importeert GenStudio for Performance Marketing de meest recente zes maanden van historische gegevens. Deze praktijk zorgt ervoor u directe toegang tot relevante inzichten voor het analyseren van tendensen, het evalueren van prestaties, en het nemen van geïnformeerde besluiten hebt. Het innameproces kan één tot vijf dagen duren, afhankelijk van het gegevensvolume in uw account.

>[!BEGINSHADEBOX]

**Beleid van de Ingestie en van het Behoud van Gegevens**

GenStudio for Performance Marketing bewaart kanaalgegevens gedurende 13 maanden. Dit bewaarbeleid omvat de zes maanden gegevens die tijdens de eerste verbinding worden ingevoerd, waardoor een uitgebreide historische gegevensanalyse en rapportage wordt gewaarborgd.

>[!ENDSHADEBOX]
