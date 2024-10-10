---
title: Toegankelijke sjablonen maken
description: Sjablonen maken in Adobe GenStudio for Performance Marketing waarmee u meer van uw publiek kunt bereiken en een optimale ervaring kunt bieden.
feature: Templates, Content
exl-id: eaaa5d9f-ad45-4fd0-826d-c250deb6d238
source-git-commit: fee67ba0d9781cf16ac909eddf385bd3d60ac97b
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Toegankelijke sjablonen maken

Adobe streeft ernaar een optimale ervaring voor alle doelgroepen te bieden. Zie [ Initiatieven van de Toegankelijkheid bij Adobe ](https://www.adobe.com/trust/accessibility/initiatives.html) voor verdere lezing.

In GenStudio for Performance Marketing kunt u elementen en sjablonen uploaden waarmee u inhoud kunt maken voor verschillende ervaringen. Door de toegankelijkheidsstandaarden te respecteren, bereikt u uw inhoud het maximale doelpubliek.

Gebruik de volgende aanbevelingen om uw sjablonen voor te bereiden met behulp van optimale toegankelijkheidsstandaarden.

## Alternatieve tekst

Maak tekstalternatieven voor niet-tekstuele inhoud, zoals afbeeldingen.

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![ Collage van ideeën, boeken, man die reuzenpotlood, computer ](../../assets/card-create-assets.png){width="400"} houden

## Lettertypen

Gebruik lettertypen die u gemakkelijk kunt lezen. Sans Serif-lettertypen hebben bijvoorbeeld een duidelijke, blokachtige vormgeving, die bijdraagt tot een hogere leesbaarheid.

Zorg voor een passend contrast tussen tekst en achtergrond. Vermijd het gebruik van lettertypekleuren die donkere tekst produceren op een donkere achtergrond en lichte tekst op een lichte achtergrond. Houd rekening met de contrastrichtlijnen voor een optimale verhouding:

- Tekst en afbeeldingen van tekst: contrastverhouding van ten minste 4,5:1
- Grote tekst en afbeeldingen van grootschalige tekst: contrastverhouding van ten minste 3:1

## Koppelingsdoel (alleen koppeling)

Maak duidelijke koppelingstekst die het doel en de locatie van de koppeling beschrijft.

Als u bijvoorbeeld koppelingstekst gebruikt zoals &quot;Klik hier&quot; of &quot;Meer lezen&quot;, wordt het doel van de koppeling niet duidelijk beschreven:

```html
<a href="product-site.html">Click here</a>
```

Als beste praktijken, zou u tekst moeten gebruiken die duidelijk beschrijft waar de verbinding gaat. Een beter voorbeeld zou de titel van de verbindingsbron en het doel kunnen gebruiken:

```html
<a href="product-site.html">Explore Product Site</a>
```

## Taal

Veel producten en services gebruiken taal op een creatieve of unieke manier. Vermijd jargon, lange zinnen en complexe zinnen. Gebruik een heldere, beknopte en goed leesbare taal die compatibel is met het doelpubliek.

- Gebruik waar mogelijk duidelijke beschrijvingen, inlinedefinities of verwante voorbeelden. Het kan moeilijk zijn om een uniek verticaal te vertalen.

- Spel uit of verbind met een definitie voor de eerste instanties van een acroniem of een afkorting. Het kan moeilijk zijn om afkortingen te vertalen.

- Gebruik waar mogelijk visuele elementen als aanvulling op tekst of complexe ideeën.
