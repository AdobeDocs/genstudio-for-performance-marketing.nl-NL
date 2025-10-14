---
title: Richtlijnen voor e-mailsjablonen
description: Volg de aanbevolen procedures bij het gebruik van e-mailsjablonen met Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 49d8d5daa2f3c93c18cd9132dab5207871b51237
workflow-type: tm+mt
source-wordcount: '441'
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

Wanneer u uw e-mailsjabloon aanpast, gebruikt u plaatsaanduidingen voor inhoud voor de volgende vereiste velden:

- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (geselecteerd in Content JPEG, PNG of GIF)

GenStudio for Performance Marketing genereert automatisch de volgende velden. RTF-tekst is niet ingeschakeld. U hoeft geen plaatsaanduidingen voor inhoud toe te passen voor:

- `pre_header`
- `subject`

De maximaal toegestane velden in een sjabloon zijn 20. Zie [&#x200B; placeholders van de Inhoud &#x200B;](/help/user-guide/content/customize-template.md#content-placeholders) om meer over het gebruiken van gebiedsnamen in malplaatjes te begrijpen.

## E-mail met meerdere secties

_Secties_ staan u toe om inhoud in verschillende groepen te organiseren, ondersteunend complexere lay-outs. In GenStudio for Performance Marketing kunt u elke sectie definiëren met een naamgevingsconventie voor groepen. Zie [&#x200B; malplaatjesecties &#x200B;](/help/user-guide/content/customize-template.md#sections-or-groups) aanpassen.

Meerdere sectiesjablonen kunnen uit 0, 2 of 3 secties bestaan:

- Een basissjabloon (nulsecties) kan één set sjabloonelementen genereren, waarvoor de naamgevingsconventie voor groepen niet nodig is.
- Een complexe sjabloon (meerdere secties) kan maximaal drie sets sjabloonelementen genereren, waarvoor u de naamgevingsconventie voor groepen moet volgen: `<groupname_fieldname>` .
- Wanneer u meerdere secties gebruikt, worden elementen die zelfstandig, buiten een sectie, staan, niet gevuld.

Hier volgen voorbeelden van veldnamen, waarbij de naamconventie voor groepen wordt gebruikt voor twee secties:

- In sectie 1:`pod1_headline`, `pod1_body`, `pod1_cta`
- In sectie 2:`pod2_headline`, `pod2_body`, `pod2_cta`

## Sjabloonvoorbeelden

+++Voorbeeld: E-mailsjabloon met één sectie

Hier volgt een eenvoudig voorbeeld van een HTML-e-mailsjabloon met één sectie. `<head>` bevat eenvoudige inline CSS voor opmaak en in `<body>` worden tijdelijke aanduidingen voor inhoud gebruikt, zoals `pre_header` , `headline` , `sub_headline` , `body` , `cta` en `image` met koppeling en. Met deze plaatsaanduidingen kan GenStudio for Performance Marketing dynamische inhoud injecteren tijdens het genereren van e-mail.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Marketing Email</title>
        <style>
            .container {
                width: 100%;
                padding: 20px;
                font-family: Arial, sans-serif;
            }
            .cta-button {
                display: inline-block;
                background-color: #fff;
                color: #000;
                border: 2px solid #000;
                padding: 10px 20px;
                text-decoration: none;
                font-family: 'Source Sans Pro', Arial, sans-serif;
                font-weight: 600;
                font-size: 14px;
                margin-top: 20px;
                text-align: center;
            }
        </style>
    </head>
    <body>
        <div class="container">
            {{pre_header}}
            <h1>{{headline}}</h1>
            <p>
                <a href="{{link}}">
                    <img alt="banner headline" src="{{image}}" width="600" height="600">
                </a>
            </p>
            <h2>{{sub_headline}}</h2>
            <p>{{body}}</p>
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++

+++Voorbeeld: E-mailsjabloon met meerdere secties

Hier is dezelfde HTML-sjabloon in het bovenstaande voorbeeld, maar met nog twee secties. De kop bevat inline CSS voor het opmaken van een groep. Het lichaam gebruikt twee groepen met [&#x200B; inhoudplaceholders &#x200B;](#content-placeholders) gebruikend een prefix.

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
            .cta-button {
            display: inline-block;
            background-color: #fff; /* Background color to white */
            color: #000; /* Text color to black */
            border: 2px solid #000; /* Border color to black */
            padding: 10px 20px;
            text-decoration: none;            
            font-family: 'Source Sans Pro', Arial, sans-serif;
            font-weight: 600; /* Semibold */
            font-size: 14px;
            margin-top: 20px;
            text-align: center;
            }
        </style>
    </head>
    <body>{{pre_header}}
        <div class="container">
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="pic1" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="pic2" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++
