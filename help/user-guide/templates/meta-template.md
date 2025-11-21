---
title: Richtlijnen voor Meta Adtemplate
description: Volg de beste praktijken wanneer het gebruiken van Meta en malplaatjes met Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
source-git-commit: 3251d81a6bfb0c1f7d2bf3c5bd319ad4e2237699
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---

# Richtlijnen voor Meta en sjablonen

Met Meta en sjablonen kunt u op Meta-platforms visueel consistente en effectieve advertenties maken. Door de aanbevolen ontwerpprocedures te volgen en ondersteunde velden te gebruiken, kunt u ervoor zorgen dat uw sjablonen zijn geoptimaliseerd voor GenStudio for Performance Marketing. In deze handleiding wordt uitgelegd hoe u Meta en sjablonen kunt structureren, aanpassen en voorbereiden op naadloze integratie en resultaten met veel impact.

Volg de onderstaande tips en trucs bij het aanpassen van Meta en sjablonen voor GenStudio for Performance Marketing:

- De breedte van 360 pixels gebruiken voor kolomlay-outs
- Een minimale resolutie van 1080 x 1080 pixels gebruiken voor afbeeldingen
- Er is precies één afbeeldingsveld vereist
- Gebruik **niet** relatieve doopvontgrootte
- Bepaal **geen** viewport
- Gebruik **niet** JavaScript
- Overschrijf **&#x200B;**&#x200B;geen element van HTML in CSS
- De tag `<img>` gebruiken in plaats van `background-image`
- Maskeren gebruiken om de leesbaarheid van tekst op achtergrondafbeeldingen te verbeteren
- Er kan slechts één sectie worden gebruikt, die één set sjabloonelementen genereert

## Erkende veldnamen

Wanneer u de sjabloon voor Meta-advertenties aanpast, past u plaatsaanduidingen voor inhoud toe voor de volgende vereiste velden:

- `image` (vereist, geselecteerd in Content JPEG, PNG of GIF)
- `on_image_text` (tekst die boven de afbeelding wordt weergegeven)

GenStudio for Performance Marketing genereert automatisch de volgende velden. U hoeft geen plaatsaanduidingen voor inhoud toe te passen voor:

- `headline`
- `body`
- `cta`

Zie [&#x200B; placeholders van de Inhoud &#x200B;](/help/user-guide/templates/customize-template.md#content-placeholders) om meer over het gebruiken van gebiedsnamen in malplaatjes te begrijpen.

## Ondersteunde hoogte-breedteverhoudingen

| Hoogte-breedteverhouding | Afmetingen (pixels) | Notities |
|------------------|----------------------------|-----------------------------------------------------------------------|
| Vierkant 1 :1 | 1080 x 1080 | Standaard voor de meeste Meta-plaatsingen; aanbevolen voor brede compatibiliteit. |
| Staand 4 :5 | 1080 x 1350 | Geoptimaliseerd voor mobiele feeds; biedt meer verticale ruimte. |
| Artikel 9 :16 | 1080 x 1920 | Ideaal voor artikelen en rollen; vult het volledige mobiele scherm. |
| Liggend 1.91 :1 | 1080 x 566 | Meest geschikt voor koppelingsadvertenties en News Feed-plaatsingen; breed formaat. |
| Aangepast | Minimaal 50 x 50 (breedte) | Alleen gebruiken als dat nodig is. Dit kan resulteren in uitsnijden of schalen. |

Als de advertentie niet in één van deze aspectverhoudingen wordt ontworpen, snijdt GenStudio for Performance Marketing automatisch het beeld in de aangewezen grootte uit.

## Sjabloonvoorbeeld

+++Voorbeeld: Meta en sjabloon

<!-- Does this need to be a precise size? -->

Hier volgt een eenvoudig voorbeeld van een Meta-advertentiesjabloon. De kop bevat inline CSS voor opmaak. Het lichaam gebruikt [&#x200B; inhoudplaceholders &#x200B;](#content-placeholders), zoals `image` en `on_image_text`, om erop te wijzen waar GenStudio for Performance Marketing inhoud kan produceren.

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Adobe</title>
        <style>
            .ad-container {
            font-family: Helvetica, sans-serif;
            position: relative;
            text-align: center;
            height: 100%;
            }
            .ad-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
            .ad-text {
            position: absolute;
            top: 0;
            left: 0;
            margin: 1em;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 1em;
            font-size: 75px;
            }
        </style>
    </head>
    <body>
        <div class="ad-container">
            <img src="{{image}}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{on_image_text}}</div>
        </div>
    </body>
</html>
```

+++
