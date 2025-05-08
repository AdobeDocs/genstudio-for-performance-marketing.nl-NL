---
title: Weergaven met inzichten filteren
description: Leer hoe u de verbeterde filtermogelijkheden met Inzichten kunt gebruiken.
level: Intermediate
feature: Reporting and Insights
exl-id: fbc53c2a-388c-4b51-94e2-626cd1e18e63
source-git-commit: 04bc6f911394d0f4c324abc347ce125203011960
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# Filter voor inzichten

Het dashboard van [!DNL Insights] verstrekt een uitvoerige reeks filters voor een efficiënte ervaring van de gegevensexploratie. Wanneer u kanalen, advertenties, media of specifieke kenmerken analyseert, kunt u met de filteropties de weergave aanpassen en de workflow stroomlijnen. Gebruik trefwoordfilters voor het nauwkeurig zoeken naar of verkennen van vooraf gedefinieerde lijsten om uw zoekopdracht te verfijnen en de focus te richten op de gegevens die het belangrijkst zijn.

## Basisbegrippen voor filters

Elke weergave in [!DNL Insights] biedt een lijst met filteropties. Met de filtertrechter aan de linkerkant wordt het menu **[!UICONTROL Filter]** geopend. Of u nu de tabel of de galerie weergeeft, de toegepaste filters worden weergegeven in de lijst **[!UICONTROL Filter by]** boven de tabel of galerie. Standaard zijn een kanaal en een account geselecteerd.

![ Filter door ](/help/assets/insights-filter-by.png " Filter door "){width=600 zoomable="yes"}

Toegepaste filters blijven in alle weergaven aanwezig. Selecteer **[!UICONTROL Clear all]** boven de tabel of galerie om alle geselecteerde filters te verwijderen.

### Zoekveld

Klik op het pictogram Zoeken (vergrootglas) om een zoekterm te typen om specifieke items in de tabel of galerie te zoeken. Als u bijvoorbeeld de term `Gear` opgeeft in de [!UICONTROL Ads] -tabel, worden de resultaten gefilterd zodat alleen advertenties worden weergegeven met de term `Gear` in de naam.

![&#128279;](/help/assets/insights-search.png " Onderzoek van het het gebiedsvoorbeeld van het 0&rbrace; Onderzoek naar advertenties met Gear in de naam "){width=600 zoomable="yes"}

### Datumbereik

De datumbereikkiezer is een krachtig hulpmiddel om de weergegeven gegevens af te stemmen op de analysedoelstellingen. Gebruik de kiezer voor het datumbereik om het tijdkader aan te passen voor de gegevens die worden weergegeven in de tabel- of galerieweergave. Standaard wordt het datumbereik ingesteld op de laatste 30 dagen. Vouw het datumbereik uit als u meer gegevens wilt opnemen of de focus op een bepaalde periode wilt plaatsen.

![ de bereikselecteur van de Datum ](/help/assets/insights-date-range.png " Uitgezocht een datumwaaier "){width=400}

Als er geen items worden weergegeven in de tabel- of galerieweergave, is dit mogelijk het gevolg van het geselecteerde datumbereik, exclusief relevante gegevens. In dergelijke gevallen vergroot u het datumbereik om ervoor te zorgen dat de gewenste gegevens worden opgenomen.

### Pagina&#39;s

Sommige tabellen kunnen meerdere pagina&#39;s beslaan, zoals aangegeven onder de tabel aan de rechterkant. Gebruik de veelzijdige zoek- en filteropties om de resultaten te verfijnen. Als u tussen pagina&#39;s wilt navigeren, gebruikt u de besturingselementen voor paginering rechts (vooruit) en links (achteruit). Zorg ervoor dat u filters correct toepast om alle relevante gegevens over pagina&#39;s te omvatten.

### Diabesturingselement

Sommige filteropties bevatten een diabesturingselement waarmee u een waarde binnen een gedefinieerd bereik kunt selecteren. Met de schuifregelaar **[!UICONTROL Media count]** in _[!UICONTROL Attributes]_&#x200B;kunt u bijvoorbeeld kenmerken filteren op basis van het aantal gekoppelde afbeeldingen of video&#39;s. Sleep de schuifregelaar om een bereik op te geven, beginnend bij een minimum van 0 tot een maximum van 100.

## Geavanceerde filtering

Met _[!UICONTROL Campaigns]_- en&#x200B;_[!UICONTROL Ads]_ -filters kunt u exacte trefwoorden gebruiken om de lijst te verfijnen. Trefwoordfilters zijn vooral handig voor het filteren van campagnes of advertenties die een complexe naamgevingsconventie gebruiken met meerdere unieke id&#39;s. Een campagnenaam kan bijvoorbeeld het volgende bevatten:

- Naam of code van specifiek gebied: `NA`, `EMEA`
- Inhoudstype acroniemen: `EB`, `CHT` of `DSP`
- Aanbiedingscodes of acroniemen: `OFFER2023`, `PROMO`

In de loop der tijd kan uw lijst met campagnes en advertenties exponentieel groeien. Houd rekening met het volgende scenario als u het filter _[!UICONTROL Campaigns]_&#x200B;wilt gebruiken om de tabel [!UICONTROL Ads] te verfijnen.

**om de lijst van Advertenties te verfijnen gebruikend de filter van Campagnes**:

1. Selecteer de weergave **[!UICONTROL Ads]** in _[!DNL Insights]_.

   ![ Adds filter en lijst ](/help/assets/insights-ads-filter.png " Advertentie mening met filtermenu "){zoomable="yes"}

1. Klik op het filter (trechter) boven de linkerkant van de tabel om het menu **[!UICONTROL Filter]** te openen.

1. Controleer of het juiste `Filter by` -kanaal en -account is geselecteerd.

1. Vouw het filter **[!UICONTROL Campaigns]** uit en klik op **[!UICONTROL Select]** .

   ![ campagnes van de Filter ](/help/assets/insights-filter-campaigns-expand.png " breid campagnecilter "){width=200} uit

1. Voer in het zoekveld van _[!UICONTROL Select campaigns]_&#x200B;trefwoorden in, gescheiden door komma&#39;s.

   Gebruik trefwoorden om uw zoekopdracht te verfijnen met logische en nauwkeurige filtering.

   - Om campagnemenamen te vinden die zowel `adventure` **EN** `ready` bevatten, ga beide sleutelwoorden in die door een komma worden gescheiden:

     ![ Onderzoek alle sleutelwoorden ](/help/assets/insights-select-campaigns-and.png " Onderzoek naar campagnemenamen die beide sleutelwoorden "){width=500} bevatten

   - Om campagnemenamen te vinden die of `adventure` **OF** `ready` bevatten, ga elk sleutelwoord afzonderlijk in:

     ![ Onderzoek of sleutelwoorden ](/help/assets/insights-select-campaigns-or.png " Onderzoek naar campagnemenamen die minstens één sleutelwoord "){width=500} bevatten

   - Als u geavanceerde zoekopdrachten wilt uitvoeren, combineert u meerdere sets trefwoorden. Bijvoorbeeld, onderzoek campagnemenamen met `adventure` en `apparel` **OF** `sun` en `gear`:

     ![ Onderzoek met veelvoudige reeksen van sleutelwoorden ](/help/assets/insights-advanced-or.png " campagnemenamen van het Onderzoek gebruikend veelvoudige reeksen sleutelwoorden "){width=500}

1. Selecteer een of meer campagnes in de resulterende zoekopdracht en klik op **[!UICONTROL Apply]** .

   ![ Lijst van campagnes ](/help/assets/insights-select-campaigns-list.png " Uitgezochte campagnes om te omvatten ")

De geselecteerde campagnes staan nu in de lijst _[!UICONTROL Filter by]_&#x200B;boven de tabel of galerie met advertenties. U kunt zich uitsluitend richten op de advertenties die gekoppeld zijn aan de gekozen campagnes. In dit voorbeeld bevatten de gefilterde resultaten zes advertenties, waarmee u een meer doelgerichte weergave voor analyse kunt maken.

![ Lijst die door campagnes ](/help/assets/insights-filter-by-campaigns.png " Lijst met campagnefilter "){zoomable="yes"} wordt gefiltreerd

U kunt de tabel van [!UICONTROL Media] verder filteren op een vergelijkbare manier voor advertentienamen. Vouw het filter **[!UICONTROL Ads]** uit en klik op **[!UICONTROL Select]** en u kunt een vergelijkbaar trefwoordfilter uitvoeren om de weergave van de mediatabel of galerie te verfijnen.

## Tabelresultaten downloaden

U kunt de gefilterde resultaten downloaden uit de tabelweergave voor verdere analyse of delen. Klik op het pictogram Downloaden (pijl die omlaag wijst) boven de rechterkant van de tabel om een CSV-bestand te downloaden op basis van de zichtbare tabel. Het downloaden begint automatisch en plaatst het CSV-bestand op de standaarddownloadlocatie.

Sommige tabellen hebben meerdere pagina&#39;s, die u onder de rechterkant van de tabel kunt zien. Het CSV- dossier omvat gegevens van _alle_ pagina&#39;s van de lijst.
