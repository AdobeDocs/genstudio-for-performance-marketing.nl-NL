---
title: Richtlijnen voor advertentiesjablonen weergeven
description: Volg de aanbevolen procedures bij het gebruik van advertentiesjablonen en bannersjablonen met Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
source-git-commit: 3251d81a6bfb0c1f7d2bf3c5bd319ad4e2237699
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Richtlijnen voor advertentiesjablonen weergeven

Weergavesjablonen zijn vooraf ontworpen lay-outs waarmee visueel aantrekkelijke banner- en weergavesjablonen worden gemaakt. Ze bieden een flexibel kader voor het opnemen van afbeeldingen, tekst en call to action, zodat consistentie en efficiëntie worden gegarandeerd bij het produceren van meerdere en verschillende variaties. Wanneer u uw sjabloon voorbereidt voor gebruik in GenStudio for Performance Marketing, moet u ervoor zorgen dat alle elementen zijn geoptimaliseerd voor weergave op het web en voldoen aan de vereiste bestandsindelingen en -grootten.

Volg de onderstaande tips en trucs bij het aanpassen van banners en advertentiesjablonen om met GenStudio for Performance Marketing te werken:

- Adobe- of Google-lettertypen gebruiken
- Elementen voorbereiden die goed worden weergegeven in dunne afmetingen
- Er is precies één afbeeldingsveld vereist
- Gebruik **niet** ingebedde of gecodeerde achtergrondbeelden
- Gebruik achtergrondafbeeldingen (`image` -veld) die zijn geüpload naar de opslagplaats voor GenStudio for Performance Marketing-inhoud. Adhere aan de richtlijnen in [ Uploading beelden voor vertoningsadvertenties ](#uploading-images-for-display-ads) voor de beste resultaten
- Gebruik **niet** JavaScript
- Er kan slechts één sectie worden gebruikt, die één set sjabloonelementen genereert

## Erkende veldnamen

Wanneer u uw banner of advertentiesjabloon aanpast, gebruikt u tijdelijke aanduidingen voor inhoud voor de volgende vereiste velden:

- `headline`
- `sub_headline`
- `body`
- `image` (vereist, geselecteerd in Content JPEG, PNG of GIF)

GenStudio for Performance Marketing genereert automatisch de volgende velden. U hoeft geen plaatsaanduidingen voor inhoud toe te passen voor:

- `cta`

Zie [ placeholders van de Inhoud ](/help/user-guide/templates/customize-template.md#content-placeholders) om meer over het gebruiken van gebiedsnamen in malplaatjes te begrijpen.

## Ondersteunde afmetingen

Breedte x Hoogte (pixels) moet zijn ingesteld.

| Afdrukstand | Afmetingen (pixels) | Notities |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| verticaal | 300 x 600 <br> 160 x 600 | Algemeen voor wolkenkrabber en halve pagina banners. |
| Horizontaal | 300 x 250 <br> 728 x 90 <br> 336 x 280 <br> 320 x 50 <br> 970 x 250 | Standaardleaderboard, normale rechthoek- en bannergrootten. |
| Aangepast | 50 x 50 tot 2000 x 2000 | Gebruik voor niet-standaard of unieke plaatsingen; controleer platformlimieten. |

