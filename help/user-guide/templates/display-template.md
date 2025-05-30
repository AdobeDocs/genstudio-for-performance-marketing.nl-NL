---
title: Richtlijnen voor advertentiesjablonen weergeven
description: Volg de aanbevolen procedures bij het gebruik van advertentiesjablonen en bannersjablonen met Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
source-git-commit: 78313c2a2177a2ccb39e37a87ca3c657e7906d0a
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Richtlijnen voor advertentiesjablonen weergeven

Weergavesjablonen zijn vooraf ontworpen lay-outs waarmee visueel aantrekkelijke banner- en weergavesjablonen worden gemaakt. Ze bieden een flexibel kader voor het opnemen van afbeeldingen, tekst en call to action, zodat consistentie en efficiëntie worden gegarandeerd bij het produceren van meerdere en verschillende variaties. Wanneer u uw sjabloon voorbereidt voor gebruik in GenStudio for Performance Marketing, moet u ervoor zorgen dat alle elementen zijn geoptimaliseerd voor weergave op het web en voldoen aan de vereiste bestandsindelingen en -grootten.

Volg de onderstaande tips en trucs bij het aanpassen van banners en advertentiesjablonen om met GenStudio for Performance Marketing te werken:

- Adobe- of Google-lettertypen gebruiken
- Elementen voorbereiden die goed worden weergegeven in dunne afmetingen
- Er is precies één afbeeldingsveld vereist
- Gebruik **niet** ingebedde of gecodeerde achtergrondbeelden
- Gebruik achtergrondafbeeldingen (`image` veld) die zijn geüpload naar de GenStudio for Performance Marketing-opslagplaats voor inhoud
- Gebruik **niet** JavaScript
- Er kan slechts één sectie worden gebruikt, die één set sjabloonelementen genereert

## Erkende veldnamen

Voor banner- en weergaveadvertenties genereert GenStudio for Performance Marketing automatisch het veld `cta` . Gebruik bij het aanpassen van de sjabloon plaatsaanduidingen voor inhoud voor de volgende vereiste velden:

- `headline`
- `sub_headline`
- `body`
- `image` (vereist, geselecteerd in Content JPEG, PNG of GIF)

Zie [ placeholders van de Inhoud ](/help/user-guide/content/customize-template.md#content-placeholders) om meer over het gebruiken van gebiedsnamen in malplaatjes te begrijpen.

## Ondersteunde afmetingen

Breedte x Hoogte (pixels) moet zijn ingesteld.

| Afdrukstand | Afmetingen (pixels) | Notities |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| verticaal | 300 x 600 <br> 160 x 600 | Algemeen voor wolkenkrabber en halve pagina banners |
| Horizontaal | 300 x 250 <br> 728 x 90 <br> 336 x 280 <br> 320 x 50 <br> 970 x 250 | Standaardleaderboard, gemiddelde rechthoek en bannergrootte |
| Aangepast | 50 x 50 tot 2000 x 2000 | Gebruik voor niet-standaard of unieke plaatsingen; controle platformgrenzen |

<!-- Potentially add an example

## Template example

+++Example: Display ad template

+++

-->
