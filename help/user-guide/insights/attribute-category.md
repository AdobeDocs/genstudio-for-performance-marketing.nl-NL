---
title: Kenmerkcategorieën
description: Meer informatie over kenmerkcategorieën die in GenStudio for Performance Marketing worden gebruikt.
feature: Insights, Attributes, Generative AI
recommendations: noDisplay
source-git-commit: 3b5fc55595f766db0327b6aefb0e29c3896e00c0
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# Kenmerkcategorieën

Een kenmerkcategorie is een classificatiegroep die gerelateerde kenmerken organiseert die een gemeenschappelijk kenmerk delen. Deze categorieën helpen de ontdekking, identificatie, en begrip van specifieke attributen te stroomlijnen door grotere context te verstrekken en hun toepassing en gebruik te vergemakkelijken.

GenStudio for Performance Marketing gebruikt de AI- en computerleermogelijkheden van Adobe om afbeeldingen, video&#39;s en tekst te bestuderen en [!UICONTROL Asset attributes] toe te passen op basis van het betrouwbaarheidsniveau. _Vertrouwen_ verwijst naar de waarschijnlijkheid dat AI aan een voorspelling of een classificatie toewijst. In de context van machinaal leren is het een soort scoring die meet hoe &quot;zelfverzekerd&quot; de AI is dat de classificatie correct is. Hoe hoger de betrouwbaarheidsscore, hoe groter de zekerheid. Wanneer een afbeelding wordt geanalyseerd, kan de AI bijvoorbeeld verschillende functies identificeren en een score toewijzen aan elke afbeelding om aan te geven hoe zeker het is dat de functie correct is. De lijst met kenmerken van een element is niet uitputtend. Assets met een uitgebreide reeks kenmerken kan worden beperkt tot een betrouwbaarheidsdrempel, zoals de drie belangrijkste geïdentificeerde kenmerken.

## Afbeeldingsfuncties

Afbeeldingsfuncties vertegenwoordigen duidelijke en informatieve elementen of patronen in een afbeelding die worden gebruikt voor analyse met [!DNL Insights] . In de volgende tabel worden de categorieën met afbeeldingsfuncties weergegeven die door de GenStudio for Performance Marketing AI worden herkend.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Categorie | Beschrijving | Voorbeeld |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Camerahoek | De locatie en hoek van de camera ten opzichte van het onderwerp. |                                                                                                                                                                                |
| Onderwerpafstand | De afstand tussen de camera en het onderwerp van een afbeelding. | `close up`, `mid shot`, `long shot` |
| Camera instellen | De configuratie van de besturingselementen van de camera om de afbeelding te produceren. |                                                                                                                                                                                |
| Kleur en toon | Evalueert de kleuren die worden gebruikt in afbeeldingselementen. Identificeert één tot drie kleuren van een reeks van 40 vooraf bepaalde kleuren in de volgende beeldlagen:<br>**[!UICONTROL Foreground colors]**- elementen in de voorlaag van beeld<br>**[!UICONTROL Background colors]** - elementen in de achterlaag van een beeld<p>In **[!UICONTROL Color temperature]** wordt de algemene warmte of koude van kleuren in de afbeelding beschreven.<br> Kleur- of temperatuurwaarden: `warm`, `cool`, `neutral` | ![ kleuren en koele tonen ](../../assets/category/image-color-temp.png){width="200" zoomable="yes"} |
| Afbeeldingsstijl | De visuele behandeling van een afbeelding. |                                                                                                                                                                                |
| Belichtingsvoorwaarde | Het type licht in een afbeelding. |                                                                                                                                                                                |
| Objecten | Identificeert een of meer items, entiteiten en elementen waaruit de afbeelding bestaat. | ![ zonnebloem, vliegtuig, bloemvoorwerp ](../../assets/category/image-objects.png){width="200" zoomable="yes"} |
| Afdrukstand | De positie van de afbeelding ten opzichte van de verhouding. | `landscape`, `portrait`, `square` |
| Mensen | Wanneer ten minste één persoon aanwezig is, kunnen een of meer kenmerken de persoon of personen in de afbeelding beschrijven. | ![ vrouwelijke persoon dansend ](../../assets/category/image-people.png){width="200" zoomable="yes"} |
| Fotografie | Detecteert het onderwerp en de techniek die worden gebruikt om een afbeelding vast te leggen, zoals `abstract` of `landscape` (niet hetzelfde als de stand Liggend). |           |
| Scènes | Detecteert de instelling of omgeving die in een afbeelding wordt weergegeven. |                                             |
| Tags | Hiermee worden objecten, elementen en andere afbeeldingskenmerken gedetecteerd die niet onder een specifieke classificatie vallen. |                                      |

<!-- Not yet approved by legal
| Attention distribution  | The level of viewer attention spread across an image.                                                 | `high`, `medium`, `low`                                                                                                                                                                                                    |
| Content density         | The amount of information or detail in an image.                                                      | `high`, `medium`, `low`                                                                                                                                                                                                    |
-->

## Videofuncties

Afbeeldingsfuncties vertegenwoordigen duidelijke en informatieve elementen, geluiden of patronen in een video voor analyse met [!DNL Insights] . In de volgende tabel worden de categorieën met videofuncties weergegeven die door de GenStudio for Performance Marketing AI worden herkend.

| Categorie | Beschrijving | Voorbeeld |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| Genre audio | Wanneer muziek aanwezig is, kan de video één classificatie van muziekstijl, zoals `electronic` of `classical` ontvangen. |          |
| Categorie Audiovereenstemming | Wanneer muziek aanwezig is, kan de video één brede classificatie van muziekgenre, zoals `acoustic` of `traditional` ontvangen. |          |
| Audiovisuele stemming | Beschrijft de algemene atmosfeer of toon van de audio, zoals `relaxing` of `energetic` . |          |
| Audiotypen | Wanneer audio aanwezig is, kan de video een markering voor één of meerdere audiotypes, zoals `music` of `speech` ontvangen. |          |
| Objecten | Identificeert een of meer items, entiteiten en elementen die in de video worden weergegeven. | ![ voorwerpen in video ](../../assets/category/video-objects.png){width="200" zoomable="yes"} |
| Afdrukstand | De positie van de video ten opzichte van de hoogte-breedteverhouding van het frame. | `landscape`, `portrait`, `square` |
| Mensen | Wanneer ten minste één persoon aanwezig is, kunnen een of meer kenmerken de persoon of personen in de video beschrijven. |        |
| Scènes | De instelling of omgeving die in de video wordt weergegeven. |        |
| Stijlen | Detecteert visuele bewerkingen die worden toegepast op elementen in de video, zoals `matte` of `neon` . |        |
| Tags | Hiermee worden objecten, elementen en andere videokenmerken gedetecteerd die niet onder een specifieke classificatie vallen. |        |

## Tekstkenmerken

Tekstfuncties omvatten tellingen voor bepaalde tekstelementen, zoals woorden, zinnen, emojis en classificaties voor semantiek, emotie en toon die worden gebruikt voor analyse met [!DNL Insights] . De tekst kan ook een leesbaarheidsscore ontvangen. Binnenkort beschikbaar.

<!-- Not yet approved by legal

The following table lists the image feature categories recognized by the GenStudio for Performance Marketing AI.

| Category             | Description | Example |
|----------------------|-------------|--------|
| Emojis Count         |             |        |
| HashTags Count       |             |        |
| Keywords             |             |        |
| Marketing Emotions   |             |        |
| Narratives           | Text that represents an overarching situation, theme, or a story. Narratives can communicate values, purpose, or identity that resonates with consumers on many levels.   |        |
| Persuasion Strategies|             |        |
| Readability          |             |        |
| Tone of voice        | | |
-->
