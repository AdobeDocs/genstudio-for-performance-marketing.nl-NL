---
title: Richtlijnen voor e-mailsjablonen
description: Volg de aanbevolen procedures bij het gebruik van e-mailsjablonen met Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: d9d774f727b69b18af6114965fdb8ffb450f797b
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Richtlijnen voor e-mailsjablonen

Een e-mailsjabloon voor marketing fungeert als basis voor visueel aantrekkelijke en responsieve e-mailcampagnes. Over het algemeen kunt u met HTML-sjablonen de lay-out, typografie, kleuren en afbeeldingen aanpassen aan de richtlijnen van uw merk. Wanneer u uw sjabloon voorbereidt voor gebruik in GenStudio for Performance Marketing, gebruikt u semantische HTML en inline CSS voor opmaak en vermijdt u scripts of externe afhankelijkheden. Goed gestructureerde HTML-sjablonen kunnen de ervaring van de ontvanger verbeteren en de leverings- en betrokkenheidspercentages verbeteren.

Volg deze tips en trucs bij het aanpassen van e-mailsjablonen om met GenStudio for Performance Marketing te werken:

- Adobe- of Google-lettertypen gebruiken
- Onbewerkte en responsieve HTML en inline CSS gebruiken
- Gebruik **niet** JavaScript
- Gebruik **niet** vaste breedte in lichaam of container
- Gebruik **niet** base64 het coderen voor beelden omdat het de malplaatjegrootte kan beduidend verhogen
- De maximale HTML-bestandsgrootte is 102 kB

## Erkende veldnamen

GenStudio for Performance Marketing genereert automatisch het veld `subject` voor e-mailberichten. Wanneer u uw sjabloon aanpast, gebruikt u plaatsaanduidingen voor inhoud voor de volgende vereiste velden:

- `pre_header` (RTF-bestand is niet ingeschakeld)
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (geselecteerd in Content JPEG, PNG of GIF)

De maximaal toegestane velden in een sjabloon zijn 20. Zie [ placeholders van de Inhoud ](/help/user-guide/content/customize-template.md#content-placeholders) om meer over het gebruiken van gebiedsnamen in malplaatjes te begrijpen.

## E-mail met meerdere secties

_Secties_ staan u toe om inhoud in verschillende groepen te organiseren, die complexere lay-outs steunt. In Genstudio for Performance Marketing kunt u elke sectie definiëren met behulp van een groepsnaamconventie. Zie [ malplaatjesecties ](/help/user-guide/content/customize-template.md#sections-or-groups) aanpassen.

Meerdere sectiesjablonen kunnen uit 0, 2 of 3 secties bestaan:

- Een basissjabloon (nulsecties) kan één set sjabloonelementen genereren, waarvoor de naamgevingsconventie voor groepen niet nodig is.
- Een complexe sjabloon (meerdere secties) kan maximaal drie sets sjabloonelementen genereren, waarvoor u de naamgevingsconventie voor groepen moet naleven: (`groupname_fieldname`)

Voorbeeld van veldnamen voor twee secties:

- `pod1_headline`, `pod1_body`, `pod1_cta`
- `pod2_headline`, `pod2_body`, `pod2_cta`

## Sjabloonvoorbeelden

+++Voorbeeld: E-mailsjabloon met één sectie

Hieronder ziet u een eenvoudig voorbeeld van een HTML-sjabloon voor een e-mailbericht dat één sectie bevat. De kop bevat eenvoudige inline CSS voor opmaak. Het lichaam bevat a `pre_header`, `headline`, en `image` [ placeholder ](#content-placeholders) voor gebruik door GenStudio for Performance Marketing om inhoud tijdens het proces van de e-mailgeneratie te injecteren.

```html {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
    <head>
        <title>Adobe</title>
        <style>
            .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
            }
        </style>
    </head>
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p><a href="{{link}}">
            <img alt="{{headline}}"
                    src="{{image}}"
                    width="600" height="600"
                    border="0"/></a></p>
            <p>{{body}}</p>
        </div>
    </body>
</html>
```

+++

+++Voorbeeld: E-mailsjabloon met meerdere secties

In het bovenstaande voorbeeld ziet u dezelfde HTML-sjabloon, maar met nog twee secties. De kop bevat inline CSS voor het opmaken van een groep. Het lichaam gebruikt twee groepen met [ inhoudplaceholders ](#content-placeholders) gebruikend een prefix.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Adobe</title>
        <style>
            .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
            }
            .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
            }
            .pod h2 {
            color: #333;
            }
            .pod p {
                color: #666;
            }
        </style>
    </head>
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p>{{body}}</p>
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="{{ headline }}" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="{{headline}}" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
        </div>
    </body>
</html>
```

+++
