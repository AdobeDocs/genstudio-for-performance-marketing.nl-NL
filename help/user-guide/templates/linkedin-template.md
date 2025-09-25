---
title: Richtlijnen voor LinkedIn-sjablonen
description: Volg de aanbevolen procedures bij het gebruik van LinkedIn-sjablonen met Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 85432185-8311-411b-b57b-f482c3d45854
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Richtlijnen voor LinkedIn-sjablonen

LinkedIn malplaatjes verstrekken een gestructureerde manier om ad creatieve voor campagnes te creëren en aan te passen LinkedIn. Deze richtlijnen zorgen ervoor dat uw advertenties voldoen aan de specificaties van LinkedIn en stroomlijnen het creatieve proces in GenStudio for Performance Marketing. Deze handleiding helpt u zich voor te bereiden op consistente branding en effectieve prestaties op verschillende LinkedIn&#39;s desktops en mobiele platforms.

Volg deze tips en trucs bij het aanpassen van LinkedIn-advertentiesjablonen om met GenStudio for Performance Marketing te werken:

- Er is precies één afbeeldingsveld vereist
- Maximale afbeeldingsgrootte van 5 MB
- Maximale kop 70 tekens
- Maximaal, inleidende tekst, 150 tekens
- Er kan slechts één sectie worden gebruikt, die één set sjabloonelementen genereert

## Erkende veldnamen

Pas tijdens het aanpassen van uw LinkedIn-sjabloon plaatsaanduidingen voor inhoud toe voor de volgende vereiste velden:

- `image` (vereist, geselecteerd in Content JPEG, PNG of GIF)
- `on_image_text` (tekst die boven de afbeelding wordt weergegeven)

GenStudio for Performance Marketing genereert automatisch de volgende velden. U hoeft geen plaatsaanduidingen voor inhoud toe te passen voor:

- `headline`
- `introductory_text`
- `cta` (Call to action)

Zie [ placeholders van de Inhoud ](/help/user-guide/content/customize-template.md#content-placeholders) om meer over het gebruiken van gebiedsnamen in malplaatjes te begrijpen.

## Ondersteunde hoogte-breedteverhoudingen

| Hoogte-breedteverhouding | Platform | Minimale grootte (px) | Max. grootte (px) | Notities |
|-------------------|-----------------|---------------|----------------|-------------------------------------------------------------------------------------|
| Vierkant 1 :1 | Desktop, mobiel | 360 x 360 | 4320 x 4320 | Het meest veelzijdig. Ideaal voor een consistente weergave op verschillende apparaten en plaatsen. |
| Horizontaal 1.91 :1 | Desktop | 640 x 360 | 7680 x 4320 | Standaardindeling liggend. Meestal gebruikt voor gesponsorde inhoud en nieuwsberichten. |
| Verticaal 1:1.91 | Mobiel | 360 x 640 | 2430 x 4320 | Groot verticaal formaat. Geoptimaliseerd voor mobiele weergave, met meer schermaanwezigheid. |
| Verticaal 2 :3 | Mobiel | 360 x 640 | 2430 x 4320 | Iets minder hoog dan 1:1.91. Goed voor campagnes op mobiele basis. |
| Verticaal 4 :5 | Mobiel | 360 x 640 | 2430 x 4320 | Aanbevolen voor mobiele apparaten. Hiermee worden de zichtbaarheid en de inhoud in evenwicht gebracht, wat vaak een hogere impact heeft. |

<!-- Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
