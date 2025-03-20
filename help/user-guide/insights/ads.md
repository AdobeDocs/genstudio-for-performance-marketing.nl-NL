---
title: Overzicht van advertenties en advertentieplaatsen
description: Bekijk een overzicht van de betrokkenheid van klanten, het budget en de uitgaven voor advertenties en plaatsingsprestaties in Adobe GenStudio for Performance Marketing.
feature: Ad Performance, Text Attributes, Reporting and Insights
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: 3448392bc3f1496dafdbed2995f40bdba9c91c31
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 0%

---

# Overzicht van advertenties en advertentieplaatsen

In de weergave [!DNL Insights] _[!UICONTROL Ads]_ziet u een lijst met advertenties voor het aangesloten kanaal en account. Een_ advertentie _is een promotieactiva die visuele en interactieve inhoud voorgenomen voor distributie aan een specifiek publiek als deel van een marketing campagne omvat. Voor Facebook zijn de advertenties namen van Meta-advertenties.

{{connect-insights}}

De tabel _[!UICONTROL Ads]_wordt ingedeeld met [!UICONTROL Ad names] . Klik op het instellingenpictogram (cog) boven de rechterkant van de tabel om de weer te geven kolommen in en uit te schakelen. Met het filterpictogram (trechter) boven de linkerzijde van de tabel wordt het menu **[!UICONTROL Filter]**geopend waarin u uit meerdere lijsten kunt kiezen. Selecteer **[!UICONTROL Clear all]**boven de tabel om alle filters te verwijderen.

![ filter en lijst van Adverten ](/help/assets/insights-ads-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Details advertentie

Selecteer een advertentie en bekijk de prestatiesmetriek, tekstattributen, en plaatsingen verbonden aan elke advertentie. _[!UICONTROL Ad details page]_bevat meetgegevens voor de advertentie `click-through rate` , `cost per action` en `spend` - hoeveel van het budget is besteed aan de advertentie. Omdat advertenties meerdere plaatsingen kunnen hebben, zoals een feed of een banner, ziet u een uitsplitsing van dezelfde meetwaarden voor elke advertentie-plaatsing. Met de pijl-links en pijl-rechts onder **[!UICONTROL Performance by ad placement]**doorloopt u de plaatsingswaarden.

![ voeg details met metriek en advertentiepunten toe ](/help/assets/insights-ad-details.png){zoomable="yes"}

### Tekstkenmerken

Onder de voorvertoning van de advertentie bevindt zich een lijst met [!UICONTROL Text attributes] die aan de advertentie is gekoppeld. Wanneer elementen en advertenties worden goedgekeurd en opgeslagen in [!DNL Content] , genereert GenStudio for Performance Marketing tags op basis van de inherente functies ervan. Zie [ details van Media ](/help/user-guide/content/asset-details.md#system-metadata) voor details over systeemmeta-gegevens.

### Plaatsen toevoegen

Op het tijdstip dat u een campagne met de advertenties van Meta creeerde, kunt u hebben geselecteerd waar te om uw advertenties in werking te stellen die op de campagne [ worden gebaseerd doelstelling ](channels.md#objectives). Met plaatsingen vergroot u het bereik van het publiek voor uw advertentie.

GenStudio for Performance Marketing biedt ondersteuning voor advertentievormen, zoals elementenfeeds, koppelingsadvertenties en één afbeelding of video. Hieronder volgt een lijst met advertentievormen per platform:

| Instagram | Facebook/Meta | Messenger | Poortnetwerk |
| ------------ | ---------------- | ------------ | ---------------- |
| Verken <br> het huis van het 1} ontdekken van het roosterhuis <br> Gegeven <br> Reels <br> het voer van het Profiel <br> Onderzoek <br> Shop <br> Artikelen<br> | De zaken onderzoeken <br> In-stroom video <br> Van de Marktplaats {<br> Reels <br> Reels bedekking <br> Juiste kolom <br> de resultaten van het Onderzoek <br> de Videoframes van de Verhalen <br> <br> Adds op de realen van Facebook<br> | Inbox <br> Artikelen | Inheemse, banner, en interstitiële <br> Verkochte video |

#### Niet-ondersteunde plaatsingen

GenStudio for Performance Marketing biedt geen ondersteuning voor de volgende advertentieplaatsen:

- Samenwerken
- Catalog/Advantage+-catalogus
- Instantieervaring
- Carousel

## Prestaties verhogen

Metrische gegevens over inzichten kunnen u helpen evalueren welke advertenties bijdragen aan het succes van een campagne en welke plaatsingen het meest effectief zijn.

In de volgende tabel vindt u definities en inzichten voor de belangrijkste maatstaven voor digitale marketing in de tabelweergave van [!UICONTROL Ads] . Elke metrisch omvat een korte definitie aangezien het op ad namen betrekking heeft, hoe metrisch wordt berekend, en één of meerdere inzichten helpen zijn betekenis en effect op een advertentie begrijpen.

| Metrisch | Definitie | Inzicht |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Ad name]** | Een lijst met advertenties voor de account van het aangesloten kanaal. Filter advertenties door een campagne te selecteren. | Sorteer de advertentielijst door op een van de belangrijkste meetgegevens te klikken. |
| **[!UICONTROL Campaign]** | Een campagne is een reeks advertenties die zijn ontworpen om een specifiek doel te bereiken. | Wanneer u de Advertentietabel door campagne filtreert, kunnen de summiere metriek van alle advertenties voor de campagne verschillend zijn dan de samenvattingsrij van de campagne in de [!UICONTROL Channels] mening. Deze discrepantie kan optreden als de kanaalbron, zoals Meta, en GenStudio lichtjes verschillende samenvattingsberekeningen gebruiken. |
| **[!UICONTROL Placements]** | Een telling van ad [ plaatsen ](#ad-placements), plaatsen waar een advertentie in de campagne verscheen. | Plaatsen vergroten het bereik van het publiek.<p>Adds die nul plaatsen en nul media tonen kunnen op een [ niet gestaafd advertentietype ](#unsupported-placements) wijzen.</p> |
| **[!UICONTROL Media]** | Het aantal elementen dat in de advertentie of advertentie wordt gebruikt. | Het aantal in de tabel Advertenties kan verschillen van het aantal in de weergave Advertentiedetails. Deze discrepantie kan optreden als de kanaalbron, zoals Meta, en GenStudio lichtjes verschillende samenvattingsberekeningen gebruiken. |
| **[!UICONTROL Impressions]** | Een telling van elke keer dat de advertentie of advertentie in het kanaal wordt geladen, ongeacht interactie of weergave. | Een hoog aantal impressies kan wijzen op brede zichtbaarheid, maar voor echt prestatieinzicht kunt u dit in verhouding tot andere betrokkenheidsmetriek overwegen. |
| **[!UICONTROL Clicks]** | Het aantal tijden de gebruikers met een klikbaar element, zoals een verbinding of een vraag-aan-actie knoop, in een advertentieplaatsing in wisselwerking staan. | Een hoge kliktelling wijst op sterke interesse en betrokkenheid met de inhoud, die efficiënt kan zijn en het juiste publiek bereikt. |
| **[!UICONTROL CTR]**<br>_klik-door tarief _ | Percentage (%) van de indrukkingen dat heeft geresulteerd in klikken op de advertentie binnen een campagne.<br>**Berekening**: `clicks` verdeeld door `impressions` | Een hoog klikthrough tarief wijst erop dat de inhoud hoogst relevant en motiverend voor het publiek in het overseinen en ontwerp is, en effectief gericht op de belangen van het publiek. |
| **[!UICONTROL CPM]**<br>_Kosten per duizend _ | Kosten voor elke duizend beelden.<br>**Berekening**: totaal bedrag `spent` verdeeld door bereik, dan vermenigvuldigd door 1000 | Een lage waarde kan op rendabele zichtbaarheid wijzen, vooral wanneer gecombineerd met een hoge doorkliksnelheid. |
| **[!UICONTROL CPA]**<br>_Kosten per Actie _ | Gemiddelde kosten die worden uitgegeven om een specifieke klantenactie, zoals een aankoop of een abonnement te bereiken.<br>**Berekening**: totaal bedrag `spent` gedeeld door het aantal voltooide klantenacties | Gebruik deze optie om de uitgaven voor advertenties te controleren die waardevolle acties van klanten tot gevolg hebben. |
| **[!UICONTROL CPC]**<br>_Kosten per klik _ | Gemiddelde kosten voor elke klik in een advertentie.<br>**Berekening**: totaal bedrag `spent` gedeeld door `clicks` | Lagere gemiddelde kosten kunnen duiden op kostenefficiënte en bestedingen, vooral in vergelijking met een stijging van de omzettingen. |
| **[!UICONTROL Spend]** | Het bedrag dat gedurende een bepaalde periode uit de campagnebegroting wordt besteed om deze advertentie te plaatsen. | Een hoog bestedingsbedrag in een korte periode kan wijzen op snel gebruik, wat tot een vroegtijdige uitputting van de middelen zou kunnen leiden. Houd het uitgegeven bedrag tegen zeer belangrijke prestatiesmetriek bij helpen het algemene rendement op investering controleren. |

## Plaatsingsprestaties

In de weergave _[!UICONTROL Ad details page]_weerspiegelen de bovenste drie cijfers de algemene prestaties van de geselecteerde advertentie. Nochtans, toont de_ Prestaties door plaats _sectie de gedetailleerde metriek voor elke advertentisplaatsing. Gebruik de rechter- en linkerpijlen om door de verschillende advertentiepunten te navigeren.

De volgende tabel bevat definities voor maatstaven voor plaatsingsprestaties:

| Metrisch | Definitie | Inzicht |
| ---------------------- | ----------------------------- | ----------- |
| **[!UICONTROL CTR]**<br>_klik-door tarief _ | Het percentage (%) van de afbeeldingen voor één advertentie-plaatsing dat heeft geresulteerd in klikken.<p>**Berekening**:`clicks` verdeeld door `impressions`<p>Deze metrische hulp bepaalt de doeltreffendheid van de advertentie in het in dienst nemen van het publiek. | Een hoge CTR geeft aan dat de advertentie relevant en aantrekkelijk is voor het publiek, wat leidt tot meer interacties. |
| **[!UICONTROL CPA]**<br>_Kosten per Actie _ | De gemiddelde kosten die aan één enkele advertentie worden besteed om een gewenste klantenactie, zoals een aankoop of een abonnement te bereiken.<p>**Berekening**: totaal bedrag `spent` gedeeld door het aantal voltooide klantenacties<p>Deze maatstaf helpt de kosteneffectiviteit van de advertentie evalueren bij het aansturen van waardevolle acties. | Een lagere CPA suggereert dat de advertentie efficiënt in het omzetten van publieksinteractie in gewenste acties tegen lagere kosten is. |
| **[!UICONTROL CPC]**<br>_Kosten per klik _ | De gemiddelde kosten verbonden aan elke klik in één enkele advertentie plaatsing.<p>**Berekening**: totaal bedrag `spent` gedeeld door `clicks`<p>Deze metrische hulp beoordeelt de kosten-efficiency van de advertentie plaatsing in het produceren van kliks. | Een lagere CPC wijst erop dat de advertentie klikt tegen lagere kosten produceert, die voor het maximaliseren van het rendement van investering kunnen nuttig zijn. |
| **[!UICONTROL Spend]** | Het bedrag dat wordt uitgegeven aan één advertentie-plaatsing, die een fractie van het totale bedrag vertegenwoordigt dat aan de volledige advertentie wordt uitgegeven. Deze maatstaf helpt de begrotingstoewijzing en de bestedingsefficiency voor elke advertentie-plaatsing te volgen. | Toezicht op de uitgaven kan helpen ervoor te zorgen dat de middelen effectief worden gebruikt over verschillende plaatsen. |
