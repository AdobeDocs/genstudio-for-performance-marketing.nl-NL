---
title: Aanbevolen procedures voor sjablonen
description: Volg de beste praktijken wanneer het gebruiken van malplaatjes met Adobe GenStudio for Performance Marketing.
feature: Templates, Content
last-substantial-update: 2024-12-09T00:00:00Z
source-git-commit: 7ba2ecfbdd6853934be5210685bf447848715d28
workflow-type: tm+mt
source-wordcount: '0'
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

Bouw malplaatjes die de lay-out en visuele vereisten voor elk kanaal aanpassen. Houd rekening met de volgende tips en beperkingen wanneer u met elk sjabloontype werkt voor optimale prestaties en compatibiliteit:

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
- De maximale bestandsgrootte van HTML is 102 kB

**Erkende gebiedsnamen**:

Voor e-mail wordt het veld `subject` automatisch opgenomen. Gebruik plaatsaanduidingen voor inhoud voor de volgende velden:

- `pre_header`
- `headline`
- `body`
- `cta`
- `image` (geselecteerd uit inhoud)
- `brand_logo`

Zie [ placeholders van de Inhoud ](customize-template.md#content-placeholders) om meer over het gebruiken van gebiedsnamen in malplaatjes te begrijpen.

>[!TAB  Meta en ]

Volg deze aanbevolen werkwijzen bij het aanpassen van Meta-advertentiesjablonen voor GenStudio for Performance Marketing:

- De breedte van 360 pixels gebruiken voor kolomlay-outs
- Een minimale resolutie van 1080 x 1080 pixels gebruiken voor afbeeldingen
- Gebruik **niet** relatieve doopvontgrootte
- Bepaal **geen** viewports
- Gebruik **niet** JavaScript
- Overschrijf **** geen HTML element in CSS
- Gebruik de volgende instellingen voor achtergrondafbeeldingen:

  Voeg `object-fit: cover` value toe aan `background-image` CSS-klasse:

  ```css
  .background-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  ```

**Beperkingen**:

- Gebruik van [ secties ](customize-template.md#sections-or-groups):
   - Er kan slechts één sectie worden gebruikt, die één set sjabloonelementen genereert.

**Gesteunde aspectverhoudingen**:

- Vierkant 1:1 (1080 x 1080 pixels)
- Verticaal 4:5 (1080 x 1350 pixels)
- Artikel 9:16 (1080 x 1920 pixels)

**Erkende gebiedsnamen**:

Voor Meta-advertenties worden de velden `headline` , `body` en `CTA` automatisch gegenereerd. Gebruik plaatsaanduidingen voor inhoud voor de volgende velden:

- `image` (geselecteerd uit inhoud)
- `on-image-text`
- `brand_logo`

Zie [ placeholders van de Inhoud ](customize-template.md#content-placeholders) om meer over het gebruiken van gebiedsnamen in malplaatjes te begrijpen.

>[!TAB  Vertoning ]

Volg deze aanbevolen werkwijzen bij het aanpassen van weergave- en sjablonen voor GenStudio for Performance Marketing:

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

**Erkende gebiedsnamen**:

Gebruik plaatsaanduidingen voor inhoud voor de volgende velden:

- `headline`
- `body`
- `cta`
- `image` (geselecteerd uit inhoud)

Zie [ placeholders van de Inhoud ](customize-template.md#content-placeholders) om meer over het gebruiken van gebiedsnamen in malplaatjes te begrijpen.

>[!ENDTABS]
