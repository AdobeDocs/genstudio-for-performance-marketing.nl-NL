---
title: Richtlijnen voor advertentiesjablonen weergeven
description: Volg de aanbevolen procedures bij het gebruik van advertentiesjablonen en bannersjablonen met Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
source-git-commit: f4bc3442678e6366e185d0c7a91c784d43b8e455
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Richtlijnen voor advertentiesjablonen weergeven

Weergavesjablonen zijn vooraf ontworpen lay-outs waarmee visueel aantrekkelijke banner- en weergavesjablonen worden gemaakt. Ze bieden een flexibel kader voor het opnemen van afbeeldingen, tekst en call to action, zodat consistentie en efficiëntie worden gegarandeerd bij het produceren van meerdere en verschillende variaties. Wanneer u uw sjabloon voorbereidt voor gebruik in GenStudio for Performance Marketing, moet u ervoor zorgen dat alle elementen zijn geoptimaliseerd voor weergave op het web en voldoen aan de vereiste bestandsindelingen en -grootten.

Volg de onderstaande tips en trucs bij het aanpassen van banners en advertentiesjablonen om met GenStudio for Performance Marketing te werken:

- Adobe- of Google-lettertypen gebruiken
- Elementen voorbereiden die goed worden weergegeven in dunne afmetingen
- Er is precies één afbeeldingsveld vereist
- Gebruik **niet** ingebedde of gecodeerde achtergrondbeelden
- Gebruik achtergrondafbeeldingen (`image` -veld) die zijn geüpload naar de opslagplaats voor GenStudio for Performance Marketing-inhoud. Adhere aan de richtlijnen in [&#x200B; Uploading beelden voor vertoningsadvertenties &#x200B;](#uploading-images-for-display-ads) voor de beste resultaten
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

Zie [&#x200B; placeholders van de Inhoud &#x200B;](/help/user-guide/content/customize-template.md#content-placeholders) om meer over het gebruiken van gebiedsnamen in malplaatjes te begrijpen.

## Ondersteunde afmetingen

Breedte x Hoogte (pixels) moet zijn ingesteld.

| Afdrukstand | Afmetingen (pixels) | Notities |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| verticaal | 300 x 600 <br> 160 x 600 | Algemeen voor wolkenkrabber en halve pagina banners. |
| Horizontaal | 300 x 250 <br> 728 x 90 <br> 336 x 280 <br> 320 x 50 <br> 970 x 250 | Standaardleaderboard, normale rechthoek- en bannergrootten. |
| Aangepast | 50 x 50 tot 2000 x 2000 | Gebruik voor niet-standaard of unieke plaatsingen; controleer platformlimieten. |

## Afbeeldingen uploaden voor weergaveadvertenties

Afbeeldingen die in weergaveadvertenties worden gebruikt, moeten afkomstig zijn uit de opslagplaats voor inhoud en moeten correct worden geüpload om ervoor te zorgen dat de afbeelding correct in de sjabloon wordt weergegeven.

Wanneer een weergavesjabloon een afbeelding van rand tot rand (volledig afloopgebied) bevat, wordt de grootte van de geselecteerde afbeelding automatisch aangepast aan de volledige sjabloonafmetingen. Als de afbeelding echter niet overeenkomt met de hoogte-breedteverhouding van de sjabloon, wordt de afbeelding uitgesneden zodat deze binnen de sjabloonafmetingen past en wordt deze mogelijk niet naar behoren weergegeven.

Er is geen functie voor automatisch passend maken voor afbeeldingen in weergave- en sjablonen.

Om het uitsnijden van afbeeldingen te verhelpen, moeten gebruikers de hoogte-breedteverhouding van de afbeelding in de sjabloon definiëren wanneer deze naar de opslagplaats voor inhoud wordt geüpload. Bij het uploaden van een goedgekeurde weergave- en advertentiesjabloon:

1. [&#x200B; ga door het malplaatje te werk uploadt proces &#x200B;](/help/user-guide/content/use-templates.md#add-a-template) tot u de **[!UICONTROL Add details]** pagina bereikt.

1. Definieer de hoogte-breedteverhouding van de afbeelding die in de sjabloon in **[!UICONTROL Ad width (px)]** en **[!UICONTROL Ad height (px)]** moet worden gebruikt. Hiermee definieert u het afbeeldingsvenster voor het gedeelte van de sjabloon waarin de afbeelding wordt weergegeven.

1. In de **[!UICONTROL More details]** sectie, selecteer **[!UICONTROL Image size]** dropdown en kies _Gewas aan een vaste grootte_.
   ![&#x200B; Uitgesneden aan een vaste grootte &#x200B;](./crop-to-fixed-size.png " Uitgesneden aan een vaste grootte "){width="80%"}

De grootte en hoogte-breedteverhouding van een afbeelding bepalen in een browser:

1. Controleer de afbeelding.
   - Windows/Linux:
      - Druk op F12.
   - macOS:
      - Druk op Command + Option + I.

1. Houd de muisaanwijzer boven de afbeelding.

1. Noteer de hoogte-breedteverhouding. Hiermee definieert u de hoogte-breedteverhouding van de afbeelding in de sjabloon.

Wanneer deze details niet worden toegepast tijdens het uploaden, wordt aangenomen dat de afbeelding de volledige hoogte-breedteverhouding van de sjabloon is en worden afbeeldingen die niet overeenkomen met die hoogte-breedteverhouding uitgesneden.

![&#x200B; Beeld bijgesneden in een vertoning en &#x200B;](./cropped-display.png " Beeld uitsnijdend "){width="60%"}

**❌Uitgesneden afbeelding in een weergave- en sjabloonweergave**

![&#x200B; Beeld dat in een vertoning wordt getoond en &#x200B;](./full-fit.png " Beeld dat in vertoning wordt getoond en "){width="60%"}

**✅Afbeelding volledig weergegeven**
