---
title: Tekstkenmerken
description: Meer informatie over de tekstfunctie van kenmerkcategorieën die in GenStudio for Performance Marketing worden gebruikt.
feature: Reporting and Insights, Text Attributes, Generative AI
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
source-git-commit: 3448392bc3f1496dafdbed2995f40bdba9c91c31
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Tekstkenmerken

Tekstfuncties omvatten tellingen voor bepaalde tekstelementen, zoals woorden, zinnen, emojis en classificaties voor semantiek, emotie en toon die worden gebruikt voor analyse met [!DNL Insights] . De tekst kan ook een leesbaarheidsscore ontvangen.

GenStudio for Performance Marketing maakt gebruik van Adobe AI- en computerleermogelijkheden om tekst te bestuderen en [!UICONTROL Media attributes] toe te passen op basis van de bijbehorende teksttonen en marketingcommentaar. De invoertekst wordt gevalideerd om ervoor te zorgen dat deze alfanumerieke tekens bevat, extra witruimten en niet-afdrukbare tekens worden verwijderd en de tekst wordt afgekapt tot maximaal 1500 woorden. Voordat gedetecteerde kenmerkcodes worden toegepast, voorspelt de AI de prevalente toon.

## Tint van stem

Tint vertegenwoordigt een algemeen karakter, een houding, of een atmosfeer die door taal wordt tentoongesteld. Een eenvoudige keuze uit woorden en leestekens, de structuur van de zin en de stijl kunnen de toon van uw bericht wijzigen. Neem bijvoorbeeld de volgende dringende berichten met behulp van de drie basistoonniveaus:

- `Formal`

  ```
  Take advantage of this distinctive and exceptional opportunity!
  ```

- `Conversational`

  ```
  Don't miss out on this great opportunity!
  ```

- `Direct`

  ```
  Don't miss the chance!
  ```

De AI detecteert verder een genuanceerdere toon. Met dezelfde instructie met urgentie uit het vorige voorbeeld gebruikt de volgende versie een grappige `poetic` toon:

- `Poetic`

  ```
  Embrace the moment, without delay, for this occasion won't always stay.
  ```

Andere secundaire waarden voor de kleurtint zijn: `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal`

## Narratief

Met de commentaarkenmerken kunt u media identificeren die de waarden, het doel of de identiteit communiceren die op het doelpubliek reageren.

| Narratief | Beschrijving | Voorbeeld |
| ----------------- | ----------- | ------- |
| `Authenticity` |             |         |
| `Celebration` |             |         |
| `Community` |             |         |
| `Convenience` |             |         |
| `Empowerment` |             |         |
| `Exploration` |             |         |
| `Futuristic` |             |         |
| `Hype` |             |         |
| `Indulgence` |             |         |
| `Peace of mind` |             |         |
| `Personalization` |             |         |
| `Prestige` |             |         |
| `Timelessness` |             |         |
| `Versatility` |             |         |
| `Well-being` |             |         |

## Leesbaarheid scoren

Met lezen en lezen van lezen wordt beoordeeld hoe gemakkelijk een stuk tekst is om te lezen en te begrijpen. Zo weet u zeker dat de inhoud geschikt is voor uw doelgroep. De scores zijn gebaseerd op verschillende factoren, waaronder de lengte van zinnen en de complexiteit van woorden.

| Score | Schoolniveau | Notities |
| ----------- | ------------------ | ------------------------------------------------------------------------- |
| 100.00-90.00 uur | 5e rang | Heel gemakkelijk te lezen. Eenvoudig te begrijpen door een gemiddelde 11-jarige student. |
| 90,0-80,0 | 6e rang | Eenvoudig te lezen. Gesprek voor consumenten. |
| 80,0-70,0 | 7e graad | Gemakkelijk leesbaar. |
| 70,0-60,0 | 8e en 9e graad | Normaal gesproken Engels. Eenvoudig te begrijpen door 13- tot 15-jarige studenten. |
| 60,0-50,0 | 10e tot 12e graad | Fairly moeilijk te lezen. |
| 50,0-30,0 | College | Hartelijk om te lezen. |
| 30,0-0,0 | Afgestudeerd aan het college | Heel moeilijk te lezen. Dit wordt het best begrepen door afgestudeerden aan de universiteit. |

## Aantal woorden

TBD

In de volgende tabel worden de categorieën met afbeeldingsfuncties weergegeven die door de GenStudio for Performance Marketing AI worden herkend.

| Categorie | Beschrijving | Voorbeeld |
| -------------------- | ------------- | --------------------- |
| Emojis Count |             |        |
| Aantal HashTags |             |        |
| Trefwoorden |             |        |
| Marketingsbewegingen | Emoties zijn bedoeld in marketingberichten om specifieke gevoelens en reacties van het publiek te wekken, wat de betrokkenheid en de verbinding met het merk kan verbeteren. | `Aspiration`, `Challenge`, `Curiosity`, `Exclusivity`, `Fascination`, `Gratification`, `Recognition`, `Trust`, `Urgency` |
| Persusiestrategieën | Technieken die worden gebruikt om het consumentengedrag te beïnvloeden en gewenste acties te stimuleren. Deze strategieën zijn gericht op specifieke psychologische triggers en klantsegmenten om de doeltreffendheid van marketingberichten te verbeteren. | `Social identity`, `Social proof`, `Endorsement`, `Concreteness`, `Foot in the door`, `Overcoming reactance`, `Reciprocity`, `Comparison`, `Social impact`, `Scarcity`, `Anthropomorphism` |
| Tint van stem | Het algemene karakter, de houding, of de atmosfeer die in een marketing bericht door woordkeus, punctuatie, zinsstructuur, en stijl wordt overgebracht. | `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal` |
