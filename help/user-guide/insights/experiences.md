---
title: Overzicht van ervaringen
description: Bekijk een overzicht van de betrokkenheid van klanten, het budget en de uitgaven voor ervaringen en plaatsingsprestaties in Adobe GenStudio for Performance Marketing.
feature: Insights, Experiences, Attributes
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: c027d5fa15b05feb95c976805d06d8fe3204c5d1
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 0%

---

# Overzicht van ervaringen

In de weergave [!DNL Insights] _[!UICONTROL Experiences]_ziet u een lijst met ervaringen voor het aangesloten kanaal en account. Voor Facebook zijn de ervaringen Meta-advertenties.

De tabel _[!UICONTROL Experiences]_wordt ingedeeld met [!UICONTROL Ad names] . Klik op het instellingenpictogram (cog) boven de rechterkant van de tabel om de weer te geven kolommen in en uit te schakelen. Het filterpictogram (trechter) boven de linkerkant van de tabel opent het menu **[!UICONTROL Filter]**, waarin u uit de lijsten [!UICONTROL Account] en [!UICONTROL Campaign] kunt selecteren om de namen van de advertenties in de tabel te filteren.

![ de filter en lijst van Ervaringen ](/help/assets/insights-experiences-filter.png){zoomable="yes"}

## Ervaar details

Een _ervaring_ is een promotieactiva die visuele en interactieve inhoud voorgenomen voor distributie aan een specifiek publiek als deel van een marketing campagne omvat.

Selecteer een ervaring (advertentienaam) en bekijk de prestatiesmetriek, tekstattributen, en plaatsingen verbonden aan elke advertentie. In de detailweergave kunt u de maatstaven van een ervaring analyseren op basis van de advertentie-plaatsing en marketinginspanningen binnen een opgegeven datumbereik.

De gedetailleerde weergave bevat een algemene advertentie `click-through rate` , `cost per action` en `spend` waarmee u kunt aangeven hoeveel van het budget op de advertentie is geplaatst. Omdat advertenties meerdere plaatsingen kunnen hebben, zoals een feed of een banner, ziet u een uitsplitsing van dezelfde meetwaarden voor elke advertentie-plaatsing. Met de pijl-links en pijl-rechts onder **[!UICONTROL Performance by ad placement]** doorloopt u de plaatsingswaarden.

![ voeg details met metriek en advertentiepunten toe ](/help/assets/insights-experience-details.png){zoomable="yes"}

### Tekstkenmerken

Onder de ervaringsvoorvertoning bevindt zich een lijst met [!UICONTROL Text attributes] die aan de advertentie is gekoppeld. Wanneer elementen en ervaringen in [!DNL Content] worden goedgekeurd en opgeslagen, genereert GenStudio for Performance Marketing tags op basis van de inherente functies. Zie [ details van Activa ](../content/asset-details.md#system-metadata) voor details over systeemmeta-gegevens.

### Plaatsen toevoegen

Op het tijdstip dat u een campagne met de advertenties van Meta creeerde, kunt u hebben geselecteerd waar te om uw advertenties in werking te stellen die op de campagne [ worden gebaseerd doelstelling ](channels.md#objectives). Met plaatsingen vergroot u het bereik van het publiek voor uw advertentie.

GenStudio for Performance Marketing biedt ondersteuning voor advertentievormen, zoals elementenfeeds, koppelingsadvertenties en één afbeelding of video. Hieronder volgt een lijst met advertentievormen per platform:

| Instagram | Facebook/Meta | Messenger | Poortnetwerk |
| ------------ | ---------------- | ------------ | ---------------- |
| Verken <br> het huis van het 1} ontdekken van het roosterhuis <br> Gegeven <br> Reels <br> het voer van het Profiel <br> Onderzoek <br> Shop <br> Artikelen<br> | De zaken onderzoeken <br> In-stroom video <br> Van de Marketplace <br> Reels <br> Reels bedekking <br> Rechterkolom <br> de resultaten van het Onderzoek <br> van de Verhalen <br> Videofeed <br> Adds op Facebook reels<br> | Inbox <br> Artikelen | Inheemse, banner, en interstitiële <br> Verkochte video |

#### Niet-ondersteunde plaatsingen

GenStudio for Performance Marketing biedt geen ondersteuning voor de volgende advertentieplaatsen:

- Samenwerken
- Catalog/Advantage+-catalogus
- Instantieervaring
- Carousel

## Ervaar prestaties

Metrische gegevens over inzichten kunnen u helpen evalueren welke ervaringen bijdragen aan het succes van een campagne en welke plaatsen het meest effectief zijn.

In de volgende tabel vindt u definities en inzichten voor de belangrijkste maatstaven voor digitale marketing in de tabelweergave van [!UICONTROL Experiences] . Elke metrisch omvat een korte definitie aangezien het op ad namen betrekking heeft, hoe metrisch wordt berekend, en één of meerdere inzichten helpen zijn betekenis en effect op een ervaring begrijpen.

| Metrisch | Definitie | Inzicht |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Experience name]** | Een lijst met ervaringen voor de verbonden kanaalaccount. Filter advertenties door een campagne te selecteren. | U kunt de lijst met ervaringen sorteren door op een van de belangrijkste meetgegevens te klikken. |
| **[!UICONTROL Campaign]** | Een campagne is een reeks ervaringen om een specifieke doelstelling te bereiken. | Wanneer u de lijst van Ervaringen door campagne filtreert, kunnen de summiere metriek van alle ervaringen voor de campagne verschillend zijn dan de summiere rij van de campagne in de [!UICONTROL Channels] mening. Deze discrepantie kan optreden als de kanaalbron, zoals Meta, en GenStudio lichtjes verschillende samenvattingsberekeningen gebruiken. |
| **[!UICONTROL Placements]** | Een telling van ad [ plaatsen ](#ad-placements), plaatsen waar een ervaring in de campagne verscheen. | Plaatsen vergroten het bereik van het publiek.<p>Adds die nul plaatsen en nul activa tonen kunnen op een [ niet gestaafd advertentietype ](#unsupported-placements) wijzen.</p> |
| **[!UICONTROL Assets]** | Het aantal elementen dat in de advertentie of ervaring wordt gebruikt. | De telling in de lijst van Ervaring kan verschillend zijn dan de telling in de mening van de Details van de Ervaring. Deze discrepantie kan optreden als de kanaalbron, zoals Meta, en GenStudio lichtjes verschillende samenvattingsberekeningen gebruiken. |
| **[!UICONTROL Impressions]** | Een telling van elke keer dat de plaatsing van de advertentie of ervaring in het kanaal laadt, ongeacht interactie of het bekijken. | Een hoog aantal impressies kan wijzen op brede zichtbaarheid, maar voor echt prestatieinzicht kunt u dit in verhouding tot andere betrokkenheidsmetriek overwegen. |
| **[!UICONTROL Clicks]** | Het aantal tijden de gebruikers met een klikbaar element, zoals een verbinding of een vraag-aan-actie knoop, in een ervaringsplaatsing in wisselwerking staan. | Een hoge kliktelling wijst op sterke interesse en betrokkenheid met de inhoud, die efficiënt kan zijn en het juiste publiek bereikt. |
| **[!UICONTROL CTR]**<br>_klik-door tarief _ | Percentage (%) van de indrukkingen dat heeft geresulteerd in klikken op de ervaringsplaatsing binnen een campagne.<br>**Berekening**: `clicks` verdeeld door `impressions` | Een hoog klikthrough tarief wijst erop dat de inhoud hoogst relevant en motiverend voor het publiek in het overseinen en ontwerp is, en effectief gericht op de belangen van het publiek. |
| **[!UICONTROL CPM]**<br>_Kosten per duizend _ | Kosten voor elke duizend beelden voor de ervaringsplaatsing.<br>**Berekening**: totaal bedrag `spent` verdeeld door bereik, dan vermenigvuldigd door 1000 | Een lage waarde kan op rendabele zichtbaarheid wijzen, vooral wanneer gecombineerd met een hoge doorkliksnelheid. |
| **[!UICONTROL CPA]**<br>_Kosten per Actie _ | Gemiddelde kosten die worden uitgegeven om een specifieke klantenactie, zoals een aankoop of een abonnement te bereiken.<br>**Berekening**: totaal bedrag `spent` gedeeld door het aantal voltooide klantenacties | Gebruik om uitgaven aan ervaringen te controleren die in waardevolle klantenacties resulteren. |
| **[!UICONTROL CPC]**<br>_Kosten per klik _ | Gemiddelde kosten voor elke klik in een ervaringsplaatsing.<br>**Berekening**: totaal bedrag `spent` gedeeld door `clicks` | Lagere gemiddelde kosten kunnen duiden op kostenefficiënte en bestedingen, vooral in vergelijking met een stijging van de omzettingen. |
| **[!UICONTROL Spend]** | Het bedrag dat gedurende een bepaalde periode uit de begroting is besteed. | Een hoog bestedingsbedrag in een korte periode kan wijzen op snel gebruik, wat tot een vroegtijdige uitputting van de middelen zou kunnen leiden. Houd het uitgavenbedrag bij de belangrijkste prestatiemetriek om het algemene rendement op investering te helpen controleren. |

## Plaatsingsprestaties

In de _mening van de Details van de Ervaring_, wijzen de hoogste drie metriek op de algemene prestaties van de geselecteerde ervaring. Nochtans, toont de _Prestaties door plaats_ sectie de gedetailleerde metriek voor elke advertentisplaatsing. De volgende tabel bevat definities voor de maatstaven voor plaatsingsprestaties:

| Metrisch | Definitie | Berekening |
| ---------------------- | ----------------------------- | ----------- |
| **[!UICONTROL CTR]**<br>_klik-door tarief _ | Percentage (%) van de indrukkingen die hebben geresulteerd in het klikken in de advertentie-plaatsing van de ervaring. | `clicks` gedeeld door `impressions` |
| **[!UICONTROL CPA]**<br>_Kosten per Actie _ | Gemiddelde kosten die aan deze advertentie worden besteed om een specifieke klantenactie, zoals een aankoop of een abonnement te bereiken. | totaal bedrag `spent` gedeeld door het aantal voltooide klantenacties |
| **[!UICONTROL CPC]**<br>_Kosten per klik _ | Gemiddelde kosten voor elke klik in een ervaringsplaatsing. | totaal bedrag `spent` gedeeld door `clicks` |
| **[!UICONTROL Spend]** | Het bedrag dat gedurende een bepaalde periode uit de begroting is besteed. | |
