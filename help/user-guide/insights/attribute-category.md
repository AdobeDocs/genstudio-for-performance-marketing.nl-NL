---
title: Kenmerkcategorieën
description: Meer informatie over kenmerkcategorieën die in GenStudio for Performance Marketing worden gebruikt.
feature: Insights, Attributes, Generative AI
recommendations: noDisplay
last-substantial-update: 2024-11-11T00:00:00Z
exl-id: c3b51ef2-56ac-4dd8-98b7-79185b5998d0
source-git-commit: 976358742e598b55b1f0c4ca4664d2bcd8f1e9b9
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Kenmerkcategorieën

Een kenmerkcategorie is een classificatiegroep die gerelateerde kenmerken organiseert die een gemeenschappelijk kenmerk delen. Deze categorieën helpen de ontdekking, identificatie, en begrip van specifieke attributen te stroomlijnen door grotere context te verstrekken en hun toepassing en gebruik te vergemakkelijken.

GenStudio for Performance Marketing maakt gebruik van Adobe AI en mogelijkheden voor machinaal leren om afbeeldingen, video&#39;s en tekst te bestuderen en [!UICONTROL Asset attributes] toe te passen op basis van de waarschijnlijkheid van juistheid. De lijst met kenmerken van een element is niet uitputtend. Assets met een uitgebreide reeks kenmerken kan worden beperkt tot de drie belangrijkste kenmerken die door de AI zijn geïdentificeerd.

## Afbeeldingsfuncties

Afbeeldingsfuncties vertegenwoordigen duidelijke en informatieve elementen of patronen in een afbeelding die worden gebruikt voor analyse met [!DNL Insights] . In de volgende tabel worden de categorieën met afbeeldingsfuncties weergegeven die door de GenStudio for Performance Marketing AI worden herkend.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Categorie | Beschrijving | Voorbeeld |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Camerahoek | De locatie en hoek van de camera ten opzichte van het onderwerp. |                                                                                                                                                                                |
| Onderwerpafstand | De afstand tussen de camera en het onderwerp van een afbeelding. | `close up`, `mid shot`, `long shot` |
| Camera instellen | De configuratie van de besturingselementen van de camera om de afbeelding te produceren. |                                                                                                                                                                                |
| Kleur en toon | Evalueert de kleuren die worden gebruikt in afbeeldingselementen. Identificeert één tot drie kleuren van een reeks van 40 vooraf bepaalde kleuren in de volgende beeldlagen:<br>**[!UICONTROL Foreground colors]**- elementen in de voorlaag van beeld<br>**[!UICONTROL Background colors]** - elementen in de achterlaag van een beeld | Kleurwaarden: `Red`, `Dark_Red`, `Green`, `Bright_Green`, `Dark_Green`, `Light_Green`, `Mud_Green`, `Blue`, `Dark_Blue`, `Light_Blue`, `Royal_Blue`, `Black`, `White`, `Off_White`, `Gray`, `Dark_Gray`, `Silver`, `Cream`, `Magenta` 9}, `Yellow`, `Mustard`, `Cyan`, `Brown`, `Dark_Brown`, `Violet`, `Pink`, `Dark_Pink`, `Maroon`, `Tan`, `Purple`, `Lavender`, `Turquoise`, `Plum`, `Gold`, `Emerald`, 36}, `Beige`, `Lilac`, `Olive``Khaki``Orange` |
| Kleurtemperatuur | Beschrijft de algemene warmte of koude van kleuren in het beeld. | Toon of temperatuurwaarden: `warm`, `cool`, `neutral`<br>![ kleuren en koele tonen ](../../assets/category/image-color-temp.png){width="200" zoomable="yes"} |
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
