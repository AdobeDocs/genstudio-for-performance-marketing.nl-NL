---
title: Aanbevolen procedures voor sjablonen
description: Volg de beste praktijken wanneer het gebruiken van malplaatjes met Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: 0f296fe6ec92178498e2e0eeb3e190a194e46aa0
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# Aanbevolen procedures voor het gebruik van sjablonen

De malplaatjes verminderen beduidend de tijd en de inspanning die wordt vereist om nieuwe inhoud te produceren door een uitgangspunt te verstrekken dat pre-gevormde lay-outs en ontwerpelementen omvat.

Gebruik de volgende aanbevelingen wanneer u sjablonen gebruikt met GenStudio for Performance Marketing:

1. Kennis over [ malplaatjeelementen ](#know-about-template-elements)
1. Vorm [ kanaalrichtlijnen ](#configure-channel-guidelines) voor efficiënte verpersoonlijking van inhoud
1. Ontwerp met [ toegankelijkheidsnormen ](accessibility-for-templates.md) voor een optimale ervaring
1. Volg [ kanaal-specifieke malplaatjerichtlijnen ](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Leer meer over basismalplaatjeelementen en procedures in [ Werk met Malplaatjes ](use-templates.md). En diep-duik in [ het aanpassen van een malplaatje ](customize-template.md) voor gebruik in uw volgende campagne.

## Informatie over sjabloonelementen

U kunt het beste vertrouwd maken met de delen van een sjabloon. Elk sjabloontype gebruikt verschillende elementen om een structuur te maken voor het maken van kanaalspecifieke inhoud. Als u uw sjabloon wilt aanpassen, gebruikt u de veldnamen in plaats van deze elementen waar u GenStudio for Performance Marketing nodig hebt om inhoud te genereren.

Zie [ elementen van het Malplaatje ](use-templates.md#template-elements).

## Kanaalrichtlijnen configureren

Configureer kanaalrichtlijnen voor elk merk voordat u sjablonen gebruikt in GenStudio for Performance Marketing. De kanaalrichtlijnen beïnvloeden rechtstreeks het type inhoud dat wordt gegenereerd wanneer de sjabloon wordt gebruikt. U kunt bijvoorbeeld tekenlimieten instellen voor de hoofdtekst van een e-mail.

![ de specificaties van het Lichaam ](/help/assets/channel-email-body.png)

Zie [ kanaalrichtlijnen ](/help/user-guide/guidelines/brands.md#channel-guidelines).

## Volg kanaalspecifieke sjabloonrichtlijnen

Wanneer het creëren van malplaatjes, zorg ervoor zij aan de specifieke vereisten van het voorgenomen kanaal voldoen. Bouw malplaatjes die de lay-out en visuele vereisten voor elk kanaal aanpassen. Er zijn algemene richtlijnen die op om het even welk malplaatje van toepassing zijn, zoals:

- Onbewerkte en responsieve HTML en inline CSS gebruiken
- Adobe- of Google-lettertypen gebruiken
- Gebruik **niet** JavaScript

Houd rekening met de volgende tips en beperkingen wanneer u met elk sjabloontype werkt voor optimale prestaties en compatibiliteit:

>[!BEGINTABS]

>[!TAB  E-mail ]

Volg deze tips en trucs bij het aanpassen van e-mailsjablonen om met GenStudio for Performance Marketing te werken:

- Adobe- of Google-lettertypen gebruiken
- Onbewerkte en responsieve HTML en inline CSS gebruiken
- Gebruik **niet** JavaScript
- Gebruik **niet** vaste breedte in lichaam of container
- Gebruik **niet** base64 het coderen voor beelden omdat het de malplaatjegrootte kan beduidend verhogen

**Beperkingen**:

- Gebruik van [ secties ](customize-template.md#sections-or-groups):
   - Een basissjabloon (slechts één sectie) kan één set sjabloonelementen genereren.
   - Een complexe sjabloon (meerdere secties) kan maximaal drie sets sjabloonelementen genereren.
- Een sjabloon mag maximaal 20 velden bevatten
- De maximale HTML-bestandsgrootte is 102 kB

**Erkende gebiedsnamen**:

Voor e-mail wordt het veld `subject` automatisch opgenomen. Gebruik plaatsaanduidingen voor inhoud voor de volgende velden:

- `pre_header`
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (geselecteerd in Content JPEG, PNG of GIF)

Zie [ placeholders van de Inhoud ](customize-template.md#content-placeholders) om meer over het gebruiken van gebiedsnamen in malplaatjes te begrijpen.

>[!TAB  Meta en ]

Volg deze aanbevolen werkwijzen bij het aanpassen van Meta-advertentiesjablonen voor GenStudio for Performance Marketing:

- De breedte van 360 pixels gebruiken voor kolomlay-outs
- Een minimale resolutie van 1080 x 1080 pixels gebruiken voor afbeeldingen
- Gebruik **niet** relatieve doopvontgrootte
- Bepaal **geen** viewport
- Gebruik **niet** JavaScript
- Overschrijf **** geen element van HTML in CSS
- De tag `<img>` gebruiken in plaats van `background-image`
- Maskeren gebruiken om de leesbaarheid van tekst op achtergrondafbeeldingen te verbeteren

**Beperkingen**:

- Gebruik van [ secties ](customize-template.md#sections-or-groups):
   - Er kan slechts één sectie worden gebruikt, die één set sjabloonelementen genereert.

**Gesteunde aspectverhoudingen**:

- Vierkant 1:1 (1080 x 1080 pixels)
- Verticaal 4:5 (1080 x 1350 pixels)
- Artikel 9:16 (1080 x 1920 pixels)
- Aangepaste afbeeldingsgrootte: (minimale afbeeldingsbreedte van 50 x 50 pixels)

**Erkende gebiedsnamen**:

Voor Meta-advertenties worden de velden `headline` , `body` en `CTA` automatisch gegenereerd. Gebruik plaatsaanduidingen voor inhoud voor de volgende velden:

- `image` (geselecteerd in Content JPEG, PNG of GIF)
- `on_image_text`

Zie [ placeholders van de Inhoud ](customize-template.md#content-placeholders) om meer over het gebruiken van gebiedsnamen in malplaatjes te begrijpen.

>[!TAB  Banner &amp; de advertentie van de Vertoning ]

Volg de onderstaande tips en trucs bij het aanpassen van banners en advertentiesjablonen om met GenStudio for Performance Marketing te werken:

- Adobe- of Google-lettertypen gebruiken
- Elementen voorbereiden die goed worden weergegeven in dunne afmetingen
- Gebruik **niet** ingebedde of gecodeerde achtergrondbeelden
- Gebruik achtergrondafbeeldingen (`image` veld) die zijn geüpload naar de GenStudio for Performance Marketing-opslagplaats voor inhoud
- Gebruik **niet** JavaScript

**Beperkingen**:

- Gebruik van [ secties ](customize-template.md#sections-or-groups):
   - Er kan slechts één sectie worden gebruikt, die één set sjabloonelementen genereert.

**Gesteunde afmetingen**:

- Verticaal: (pixels)
   - 300 x 600
   - 160 x 600 &#x200B;
- Horizontaal: (pixels)
   - 300 x 250
   - 728 x 90
   - 336 x 280
   - 320 x 50
   - 970 x 250 &#x200B;
- Aangepast: (pixels)
   - 50 x 50 tot 2000 x 2000

**Erkende gebiedsnamen**:

Voor banner- en weergaveadvertenties wordt het veld `CTA` automatisch gegenereerd. Gebruik plaatsaanduidingen voor inhoud voor de volgende velden:

- `headline`
- `sub_headline`
- `body`
- `image` (geselecteerd in Content JPEG, PNG of GIF)

Zie [ placeholders van de Inhoud ](customize-template.md#content-placeholders) om meer over het gebruiken van gebiedsnamen in malplaatjes te begrijpen.

>[!TAB  LinkedIn en ]

[!BADGE  Beta ]{type=Informative tooltip="Deze functie is momenteel in Beta, waardoor bepaalde functionaliteit mogelijk beperkt is of kan worden gewijzigd."}

Volg deze tips en trucs bij het aanpassen van LinkedIn-advertentiesjablonen om met GenStudio for Performance Marketing te werken:

**Beperkingen**:

- Gebruik van [ secties ](customize-template.md#sections-or-groups):
   - Er kan slechts één sectie worden gebruikt, die één set sjabloonelementen genereert.
- Maximale afbeeldingsgrootte van 5 MB
- Maximale kop 70 tekens
- Maximaal, inleidende tekst, 150 tekens

**Gesteunde aspectverhoudingen**:

- Vierkant 1:1
   - desktop of mobiel
   - Min.: 360 x 360 pixels
   - Max.: 4320 x 4320 pixels
- Horizontaal 1,91:1
   - desktop
   - Min.: 640 x 360 pixels
   - Max.: 7.680 x 4.320 pixels
- Verticaal 1:1,91
   - mobiel
   - Min.: 360 x 640 pixels
   - Max.: 2430 x 4320 pixels
- Verticaal 2,3
   - mobiel
   - Min.: 360 x 640 pixels
   - Max.: 2430 x 4320 pixels
- Verticaal 4.5 (aanbevolen)
   - mobiel
   - Min.: 360 x 640 pixels
   - Max.: 2430 x 4320 pixels

**Erkende gebiedsnamen**:

Voor LinkedIn-advertenties worden de velden `headline` , `introductory_text` en `CTA` automatisch gegenereerd. Gebruik plaatsaanduidingen voor inhoud voor de volgende velden:

- `image` (geselecteerd in Content JPEG, PNG of GIF)
- `on_image_text`

Zie [ placeholders van de Inhoud ](customize-template.md#content-placeholders) om meer over het gebruiken van gebiedsnamen in malplaatjes te begrijpen.

>[!ENDTABS]
