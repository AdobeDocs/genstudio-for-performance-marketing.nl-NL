---
title: Afbeeldingsfuncties
description: Meer informatie over de afbeeldingsfunctie van kenmerkcategorieën die in GenStudio for Performance Marketing worden gebruikt.
level: Intermediate
feature: Reporting and Insights, Image Attributes, Generative AI
exl-id: b7e3d202-4085-48a4-a6ba-c950dfd52233
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# Afbeeldingsfuncties

Afbeeldingsfuncties vertegenwoordigen duidelijke en informatieve elementen of patronen in een afbeelding die worden gebruikt voor analyse met [!DNL Insights] . Deze functies helpen u bij het indelen en begrijpen van de visuele inhoud, waardoor nauwkeurigere en gedetailleerdere inzichten mogelijk worden. Door verschillende kenmerken, zoals stijl, kleur en objecten, te identificeren, kan de AI een uitgebreide analyse van het beeld leveren, die helpt bij betere besluitvorming en strategieformulering.

## Stijldetectie

Het bepalen van de _beeldstijl_ dient als stichting voor het identificeren van andere beeldkenmerken. De AI kan de juiste analysetechnieken toepassen en relevante kenmerken herkennen, waardoor het beeld beter wordt begrepen. Elke stijl heeft duidelijke visuele kenmerken die van invloed zijn op de manier waarop de afbeelding wordt waargenomen en geanalyseerd.

Als de afbeeldingsstijl wordt geïdentificeerd als een `photograph` , analyseert de AI extra kenmerken voor `camera settings` , `camera proximity` en `Photography genres` . Deze eigenschappen zijn specifiek voor foto&#39;s en bieden dieper inzicht in de samenstelling en kwaliteit van de afbeelding. Zie [ 28 types van fotografiestijlen ](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html) in Adobe _fotografie_ leren en over populaire types van fotografie en stichtende terminologie leren.

Als de afbeeldingsstijl wordt geïdentificeerd als een `sketch` of een `digital cartoon` , kan een andere reeks kenmerken relevant zijn. Deze hiërarchische aanpak zorgt ervoor dat de analyse contextafhankelijk nauwkeurig is en is afgestemd op het specifieke type afbeelding dat wordt onderzocht.

## Afbeeldingsfuncties zoeken

**om beelden in een specifieke attributencategorie** te bekijken:

1. Selecteer de weergave _[!DNL Insights]_in **[!UICONTROL Attributes]**.

1. Wijzig de tabelweergave door **[!UICONTROL Images]** te selecteren.

1. Selecteer een afbeeldingsfunctie in de lijst **[!UICONTROL Attribute category]** , bijvoorbeeld `Scenes` .

1. Selecteer een kenmerk voor een gedetailleerde weergave van afbeeldingen die dezelfde categorie hebben.

   De categorie `Scenes` kan bijvoorbeeld `restaurant` als attribuut hebben.

1. De _details van Attributen_ pagina maakt een lijst van alle beelden met dit attribuut.

In de volgende tabel worden de categorieën met afbeeldingsfuncties weergegeven die door de GenStudio for Performance Marketing AI worden herkend. De lijst met gedetecteerde kenmerken voor media-inhoud is niet limitatief. Media die een uitgebreide reeks kenmerken bevatten, kunnen worden beperkt tot de drie belangrijkste kenmerken die door de AI worden geïdentificeerd.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Categorie | Beschrijving | Voorbeeld |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Let op verspreiding | Het niveau van de kijkeraandacht spreidt zich over een beeld, die erop wijst hoeveel nadruk verschillende gebieden van het beeld kunnen ontvangen. Een hogere distributie betekent dat geen enkel gebied de focus van de kijker domineert, terwijl een lagere distributie betekent dat een of twee brandpunten de aandacht van de kijker vastleggen. | `high`, `medium`, `low`<p>Voorbeeld van `low` distributie links en `high` distributie rechts:<p>![ laag en high-distribution bal spel ](/help/assets/category/image-attn-lowhigh.png " Verschil in lage en hoge distributie "){width="200" zoomable="yes"} |
| Camerahoek | Het perspectief van waaruit de camera het onderwerp vastlegt. Dit beïnvloedt de perceptie en interpretatie van de kijker van het beeld. Als de afbeeldingsstijl `photograph` is, wordt dit kenmerk geïdentificeerd. | `Low angle`, `High angle`, `Eye level`, `Neutral angle`, `Overhead view`, `Bird's eye view`<p>Voorbeeld van `Overhead view` :<p>![ Overheadmening ](/help/assets/category/image-camera-angle.png " Paar van korte broeken van overheadkosten "){width="200" zoomable="yes"} |
| Camera instellen | De specifieke aanpassingen en configuraties van de besturingselementen van de camera die van invloed zijn op de uiteindelijke weergave en kwaliteit van de afbeelding. Als de afbeeldingsstijl `photograph` is, wordt dit kenmerk geïdentificeerd. | `Fast shutter speed`, `Long exposure`, `Bokeh blur`, `Motion blur`, `Tilt-shift blur`, `Flash`, `Wide-angle`, `Black and white`, `Double-exposure`, `Macro`, `Normal mode`<p>Voorbeeld van een instelling `Fast shutter speed` :<p>![ Snelle sluitersnelheid ](/help/assets/category/image-camera-setting.png " die op een golf overstroomt "){width="200" zoomable="yes"} |
| Kleur en toon | De kleuren en toonkwaliteiten in een afbeelding. Hiermee worden maximaal drie kleuren geïdentificeerd uit een vooraf gedefinieerde set van 40 kleuren in verschillende afbeeldingslagen:<p>**[!UICONTROL Foreground colors]** - kleuren in de voorlaag van beeld <br>**[!UICONTROL Background colors]**- kleuren in de achterlaag van het beeld | Kleurwaarden: `Red`, `Dark Red`, `Green`, `Bright Green`, `Dark Green`, `Light Green`, `Mud Green`, `Blue`, `Dark Blue`, `Light Blue`, `Royal Blue`, `Black`, `White`, `Off White`, `Gray`, `Dark Gray`, `Silver`, `Cream`, `Magenta` 9}, `Cyan`, `Yellow`, `Mustard`, `Khaki`, `Brown`, `Dark Brown`, `Violet`, `Pink`, `Dark Pink`, `Maroon`, `Tan`, `Purple`, `Lavender`, `Turquoise`, `Plum`, `Gold`, 36}, `Emerald`, `Orange`, `Beige``Lilac``Olive` |
| Kleurtemperatuur | Beschrijft de algemene warmte of koude van kleuren in het beeld. | Toon of temperatuurwaarden: `warm`, `cool`, `neutral`<br>![ kleuren en koele tonen ](/help/assets/category/image-color-temp.png " de temperatuur van de Kleur met koele achtergrond en veelvoudige gekleurde voorwerpen "){width="200" zoomable="yes"} |
| Inhoudsdichtheid | De concentratie van visuele elementen en details in een afbeelding die aangeeft hoeveel informatie in de visuele ruimte wordt ingepakt.<p>In tegenstelling tot de verdeling van de aandacht, die meet hoe de kijker zich over verschillende gebieden van een beeld verspreidt, concentreert de inhoudsdichtheid zich op de hoeveelheid aanwezige visuele informatie. Een hogere inhoudsdichtheid betekent dat er meer elementen aanwezig zijn. | `high`, `medium`, `low`<p>Voorbeeld van `low` dichtheid aan de linkerkant en `high` dichtheid aan de rechterkant:<p>![ laag en high-density bal spel ](/help/assets/category/image-attn-lowhigh.png " Verschil in lage en hoge inhoudsdichtheid "){width="200" zoomable="yes"} |
| Afbeeldingsstijl | De visuele behandeling van een afbeelding, zoals een foto of schets. Wanneer de AI de afbeeldingsstijl heeft bepaald, kunnen andere kenmerken worden geïdentificeerd. Als de afbeelding bijvoorbeeld een foto is, kunnen de camera-instellingen, de nabijheid van de camera en de belichtingsomstandigheden van toepassing zijn. | `Photograph`, `Photograph with text overlay`, `Sketch`, `Painting`, `Digital cartoon`, `Infographics`, `Graphic design`, `Collage`, `Software screenshot`<p>Voorbeeld van a `digital cartoon` beeldstijl ![ de stijl van het beeldbeeld van de 1} cartoon van het beeldstijl ](/help/assets/category/image-style.png " van het Beeld van een kat "){width="200" zoomable="yes"} |
| Belichtingsvoorwaarde | Beschrijft de kwaliteit en de kenmerken van het licht in een afbeelding, die van invloed zijn op de stemming, toon en zichtbaarheid. | `Golden hour`, `Blue hour`, `Midday`, `Overcast`, `Night`, `Daylighting`, `Incandescent`, `Fluorescent`, `Colorful`, `Studio`<p>Voorbeeld van de voorwaarde `daylighting` :<p>![ Persoon en hond op sidewalk in dagverlichtingsvoorwaarde ](/help/assets/category/image-lighting.png " Daylighting voorwaarde "){width="200" zoomable="yes"} |
| Objecten | Identificeert een of meer items, entiteiten en elementen waaruit de afbeelding bestaat. | De waarden zijn te talrijk, maar enkele voorbeelden zijn: `backpack`, `book`, `hawk`, `glasses`, `fish`, `pencil`, `mountain bike`, `soap`<p>Voorbeeld van `toucan` - en `bird` -objecten:<p>![ vogel, toucan voorwerp ](/help/assets/category/image-objects-bird.png " Grafisch ontwerp van Toucan vogelvoorwerp "){width="200" zoomable="yes"} |
| Afdrukstand | De uitlijning van de afbeelding ten opzichte van de breedte en hoogte. Geeft aan of de breedte breder is dan de lengte (liggend), groter dan de breedte (staand) of gelijk aan de hoogte (vierkant). | `landscape`, `portrait`, `square`<p>Voorbeeld van een oriëntatie `square` :<p>![ vierkante schets ](/help/assets/category/image-orientation-square.png " Vierkante schets van de richtingbloem "){width="200" zoomable="yes"} |
| Mensen | Wanneer ten minste één persoon aanwezig is, kunnen een of meer kenmerken de persoon of personen in de afbeelding beschrijven. | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people`<p>Voorbeeld van personencategorieën `woman` en `person` :<p>![ persoonvrouw met camera ](/help/assets/category/image-people.png " Persoon die een camera "){width="200" zoomable="yes"} beheert |
| Fotografie | Detecteert het onderwerp en de techniek die worden gebruikt om een afbeelding vast te leggen, zoals `Abstract` of `Landscape` (niet hetzelfde als de stand Liggend). | `Architecture`, `Astro`, `Landscape`, `Pet`, `Interior`, `Wildlife`, `Night`, `Cityscape`, `Seascape`, `Underwater`, `Storm`, `Adventure sports`, `Fashion`, `Portrait`, `Sports`, `Food`, `Street`, `Event`, `Lifestyle`, `Commercial` `Group` , `Abstract` , `Minimalist` , `Composite` , `Surreal` <p>Zie [ Types van fotografie ](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html).<p>Voorbeeld van `Adventure sports` :<p>![ persoon die met kano ](/help/assets/category/image-photography-genres.png " Persoon met een oor die door een kano "){width="200" zoomable="yes"} staat |
| Scènes | Hiermee wordt de instelling of omgeving in een afbeelding aangegeven, waarbij context wordt verschaft over de plaats waar de afbeelding is vastgelegd of het type locatie dat wordt weergegeven. | De waarden zijn te talrijk, maar enkele voorbeelden zijn: `lake`, `underwater`, `highway`, `hill`, `log cabin`, `island`, `beach`, `lounge`<p>Voorbeeld `snow` -, `sky` -, `winter` - en `mountain` scènes die worden gereflecteerd op een helm:<p>![ wintersneeuwscène ](/help/assets/category/image-scenes.png " Winter, sneeuw, lucht, en de bezinning van de bergscène "){width="200" zoomable="yes"} |
| Onderwerpafstand | De afstand tussen de camera en het onderwerp van een afbeelding. | `close up`, `mid shot`, `long shot`<p>Voorbeeld van een `Long shot` :<p>![ Lange ontsproten bergtop ](/help/assets/category/image-subject-distance.png " Man op een verre bergtop "){width="200" zoomable="yes"} |
| Stijlen | Geeft aan of er visuele bewerkingen worden toegepast op afbeeldingselementen, zoals de bewerkingen die worden gebruikt in Lightroom of Photoshop. | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `circle`, `circular`<p>Voorbeeld van `circular` -stijl:<p>![ circulaire gateway in koraalrif ](/help/assets/category/image-styles-circular.png " Cirkelportaal in een koraalrif "){width="200" zoomable="yes"} |
| Tags | Hiermee worden andere afbeeldingskenmerken gedetecteerd die niet onder een specifieke classificatie vallen. Tags bieden extra context en metagegevens over de afbeelding. De AI kan bijvoorbeeld `helmet` - en `motorobike` -objecten in een afbeelding detecteren en `riding` als tag opnemen. | De waarden zijn te talrijk, maar enkele voorbeelden zijn: `construction`, `gothic`, `healing`, `military`, `selfie`, `football`, `typing`, `dancer`, `dancing`<p>Voorbeeld van tags `dancer` en `dancing` :<p>![ markeringen voor danser en het dansen ](/help/assets/category/image-tags.png " Dansende persoon "){width="200" zoomable="yes"} |
