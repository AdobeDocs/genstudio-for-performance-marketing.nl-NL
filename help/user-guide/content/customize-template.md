---
title: Een sjabloon aanpassen
description: Leer hoe u uw sjabloon voor Adobe GenStudio for Performance Marketing kunt aanpassen en optimaliseren.
level: Intermediate
feature: Templates, Content
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 62ab3849296195ca4d9525cb5688f74ce8bede54
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 0%

---

# Een sjabloon aanpassen

U kunt een sjabloon aanpassen voor gebruik in GenStudio for Performance Marketing door plaatsaanduidingen voor inhoud of velden in te voegen die de generatieve AI gebruikt om inhoud in te voegen.

In de volgende secties wordt uitgelegd hoe u de sjablonen voor HTML voor GenStudio for Performance Marketing kunt aanpassen met de sjabloontaal _[!DNL Handlebars]_. In de syntaxis van [!DNL Handlebars] wordt gewone tekst met dubbele accolades gebruikt als plaatsaanduidingen voor inhoud. Zie [ wat  [!DNL Handlebars] ](https://handlebarsjs.com/guide/#what-is-handlebars) in de_ de taalgids van Handlebars _is om te leren hoe te om uw malplaatje voor te bereiden.


Zodra uw malplaatje klaar is, kunt u het [ uploaden aan GenStudio for Performance Marketing ](use-templates.md#upload-a-template) en beginnen gepersonaliseerde e-mails te produceren die op uw douanemalplaatje worden gebaseerd.

>[!TIP]
>
>Volg [ toegankelijkheidsrichtlijnen ](accessibility-for-templates.md) en [ beste praktijken ](/help/user-guide/content/best-practices-for-templates.md) zodat u meer van uw publiek kunt bereiken en een optimale ervaring verstrekken.

## Plaatsaanduidingen voor inhoud

GenStudio for Performance Marketing erkent bepaalde [ elementen ](use-templates.md#template-elements) binnen een malplaatje, maar slechts als u hen met een erkende gebiedsnaam identificeert.

In de kop of de hoofdtekst van een sjabloon kunt u de syntaxis van [!DNL Handlebars] gebruiken als plaatsaanduiding voor inhoud, waarbij u GenStudio for Performance Marketing nodig hebt om de sjabloon te vullen met werkelijke inhoud. GenStudio for Performance Marketing erkent en interpreteert de inhoudsplaceholders die op [ worden gebaseerd erkende _gebied_ naam ](#recognized-field-names).

U kunt `{{ headline }}` bijvoorbeeld met de syntaxis van [!DNL Handlebars] gebruiken om aan te geven waar de kop van de e-mail moet worden geplaatst:

```handlebars
<div>{{headline}}</div>
```

### Erkende veldnamen

De volgende tabel bevat een lijst met de veldnamen die door GenStudio for Performance Marketing worden herkend voor populatie in sjablonen. Voeg deze veldnamen met de syntaxis [!DNL Handlebars] toe aan uw sjabloon waar u GenStudio for Performance Marketing nodig hebt om inhoud te genereren.

| Veld | Rol | Kanaalsjabloon |
| ------------------ | ---------------------- | -------------------------------- |
| `{{pre_header}}` | Pre-header | email |
| `{{headline}}` | Titel | e-mail <br> Meta en <br> Vertoning |
| `{{body}}` | Platte kopie | e-mail <br> Meta en <br> Vertoning |
| `{{cta}}` | Oproep tot actie | e-mail <br> Meta en <br> Vertoning |
| `{{on_image_text}}` | Op afbeeldingstekst | Meta en |
| `{{image}}` | Afbeelding—Selecteren uit inhoud | e-mail <br> Meta en <br> Vertoning |
| `{{brand_logo}}` | Logo van geselecteerd merk <br> zie [ het merklogo gebiedsnaam ](#brand-logo-field-name) voor geadviseerd gebruik. | e-mail <br> Meta-advertentie |

GenStudio for Performance Marketing vult bepaalde velden automatisch in de volgende sjablonen in:

- **E-mailmalplaatje** vereist u niet om het `subject` gebied te identificeren
- **Meta voegt malplaatje** toe vereist u niet om `headline` te identificeren, `body`, en `CTA` gebieden
- **het malplaatje van Advertentie van de Vertoning** vereist u niet om het `CTA` gebied te identificeren

>[!WARNING]
>
>Voor Instagram-advertenties wordt de gegenereerde kop niet weergegeven in de uiteindelijke ervaring.

Er geldt een limiet van 20 velden wanneer u een sjabloon uploadt naar GenStudio for Performance Marketing. Aangezien het veld `subject` automatisch wordt gegenereerd in een e-mail, telt het als één veld. Dit betekent dat er 19 velden zijn toegestaan in een e-mailsjabloon.

>[!TIP]
>
>U kunt uw malplaatje verifiëren gebruikend de [ malplaatjevoorproef ](#template-preview) in GenStudio for Performance Marketing.

#### Naam merklogo

Op dit moment kunt u het merklogo voor het uploaden van de sjabloon niet selecteren. In de volgende voorbeelden worden twee methoden getoond die het merklogo voorwaardelijk weergeven. Elke methode verifieert de bron, biedt een standaard- of alternatieve afbeelding voor het geval het merklogo niet beschikbaar is en past een stijl toe:

**Voorbeeld 1**: Het gebruiken van [!DNL Handlebars] Ingebouwde voorwaarde van Helpers direct in het HTML `img src` attribuut:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Voorbeeld 2**: Het gebruiken van [!DNL Handlebars] Ingebouwde voorwaardelverklaring om de HTML `img` markering te verpakken:

```handlebars
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

#### Handmatige veldnamen

Alle andere veldnamen worden behandeld als handmatig gevulde velden.

Als u een bewerkbare sectie wilt maken, voegt u dubbele haakjes toe rond de sectienaam:

```handlebars
{{customVariable}}
```

### Secties of groepen

_Secties_ informeren GenStudio for Performance Marketing dat de gebieden in deze sectie een hoge graad van coherentie vereisen. Als u deze relatie instelt, kan de AI inhoud genereren die overeenkomt met de creatieve elementen in de sectie.

Gebruik een voorvoegsel van uw keuze in de veldnaam om aan te geven dat een veld deel uitmaakt van een sectie of groep. Gebruik een veldnaam (`headline`, `body`, `image` of `cta`) na het onderstrepingsteken (`_`). De volgende kop en tekst behoren bijvoorbeeld tot de sectie `pod1` :

- `pod1_headline`
- `pod1_body`

Elke sectie kan slechts één van elk gebiedstype gebruiken. In het bovenstaande voorbeeld kan de sectie `pod1` slechts één `pod1_headline` -veld gebruiken. Vanwege deze regel kunnen de secties niet worden genest.

Elk sjabloontype, zoals een e-mail- of Meta-advertentie, heeft kanaalspecifieke beperkingen voor het gebruik van secties. Zie [ kanaal-specifieke richtlijnen ](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates#follow-channel-specific-template-guidelines) in _Beste praktijken voor het gebruiken van malplaatjes_ onderwerp.

Een e-mailsjabloon kan bijvoorbeeld maximaal drie secties bevatten. Daarom kunt u drie kopregels en hoofdtekstsecties gebruiken:

- `pre-header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

GenStudio for Performance Marketing begrijpt dat `pod1_headline` nauwer verwant is aan `pod1_body` dan aan `pod2_body` .

Zie [ Gestructureerde herinneringen ](/help/user-guide/effective-prompts.md#structured-prompts) leren hoe te om een herinnering te amberen die variërende inhoud voor elke sectie in e-mail produceert.

### Oproepen tot actie

Een Oproep tot actie (CTA) omvat een uitdrukking en een verbinding. De CTA- _[!UICONTROL Rephrase]_en_[!UICONTROL Add link]_ -mogelijkheden werken alleen correct tijdens het genereren van varianten als u plaatsaanduidingen voor de koppeling en de woordgroep in uw sjabloon opneemt.

Gebruik de volgende richtlijnen voor het instellen van plaatsaanduidingen voor CTA:

- CTA herfrase is beschikbaar en de koppeling kan worden bewerkt

  ```html
  <a class="button" href="{{pod1_link}}" >{{cta}}</a>
  ```

- CTA herfragment is beschikbaar, maar de verbinding is **niet** editable omdat de daadwerkelijke verbinding in het malplaatje wordt verstrekt

  ```html
  <a align="center" href="https://link">{{cta}}</a>
  ```

- De verbinding van CTA is editable, maar het herformuleren is **niet** beschikbaar omdat de uitdrukking in het malplaatje wordt verstrekt

  ```html
  <a class="button" href="{{pod1_link}}" >Register now</a>
  ```

GenStudio for Performance Marketing kan variantvraag-aan-actie uitdrukkingen, ook verstrekken. Zie {de Vraag van 0} herzien aan actie ](/help/user-guide/create/manage-variants.md#revise-call-to-action).[

## Sjabloonvoorbeeld

Wanneer u [ een malplaatje ](use-templates.md#upload-a-template) uploadt, scant GenStudio for Performance Marketing het dossier van de HTML voor erkende gebieden. Gebruik de voorproef om uw [ malplaatjeelementen ](use-templates.md#template-elements) te herzien en te bevestigen dat u hen behoorlijk met [ erkende gebiedsnamen ](#recognized-field-names) identificeerde.

Voorbeeld van een e-mailsjabloon:

![ ontdekte gebieden van de Voorproef ](/help/assets/template-detected-fields.png){width="650"}

### Voorvertoning besturen

U kunt de zichtbaarheid van speciale inhoud bepalen met behulp van ingebouwde hulpmiddelen (speciale expressies in de sjabloontaal [!DNL Handlebars] die bepaalde handelingen uitvoeren). U kunt bijvoorbeeld een voorwaardelijke instructie toevoegen waarmee trackingparameters worden toegevoegd aan koppelingen in de geëxporteerde sjabloon terwijl de voorbeeldkoppelingen schoon blijven.

De waarde `_genStudio.browser` wordt ingesteld bij het renderen van een sjabloon en de waarde `genStudio.export` wordt ingesteld bij het exporteren van een sjabloon. U kunt besluiten om bepaalde inhoud bij de bovenkant van een e-mail te omvatten gebruikend een voorwaardelijke omslag, bijvoorbeeld wanneer het malplaatje voor de uitvoer wordt gebruikt:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Een ander voorbeeld kan zijn om het gebruik van volgcodes te verhinderen wanneer het previewing van een malplaatje in GenStudio for Performance Marketing. In het volgende voorbeeld ziet u hoe u volgparameters toevoegt aan koppelingen in de geëxporteerde sjabloon, terwijl de voorbeeldkoppelingen ongewijzigd blijven:

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Statische inhoud

E-mail- en metasjablonen zijn vaak gekoppeld aan afbeeldingen en CSS-bestanden die op andere domeinen worden gehost. Wanneer GenStudio for Performance Marketing miniaturen genereert voor sjabloonvoorvertoningen of de ervaringen die daaruit zijn afgeleid, wordt de inhoudsbron gevalideerd en wordt een kopie ingesloten voor voorvertoningen.

Externe bestanden worden alleen tijdelijk ingesloten om de voorvertoning van de sjabloon te maken, zodat de voorvertoning de inhoud correct weergeeft zoals deze wordt weergegeven op het moment dat u de sjabloon maakt. Deze externe dossiers worden **niet** permanent opgeslagen in GenStudio for Performance Marketing. Nadat de sjabloonvoorvertoning is gemaakt, gaat GenStudio for Performance Marketing door met het verwijzen naar de oorspronkelijke bronkoppeling in de sjabloon.

### Inhoud vernieuwen

Als de bron na het creëren van de aanvankelijke voorproef verandert, gebruik [ verfrist ](/help/user-guide/content/use-templates.md#refresh-template) functie om de malplaatjevoorproef met de meest recente versie van de inhoud van de externe bronnen bij te werken.

## Sjabloonvoorbeelden

+++Voorbeeld: E-mailsjabloon met één sectie

Hier volgt een eenvoudig voorbeeld van een HTML-sjabloon voor een e-mailbericht dat één sectie bevat. De kop bevat eenvoudige inline CSS voor opmaak. Het lichaam bevat a `pre-header`, `headline`, en `image` [ placeholder ](#content-placeholders) voor gebruik door GenStudio for Performance Marketing om inhoud tijdens het proces van de e-mailgeneratie te injecteren.

```handlebars {line-numbers="true" highlight="13"}
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
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

+++Voorbeeld: E-mailsjabloon met meerdere secties

In het bovenstaande voorbeeld ziet u dezelfde HTML-sjabloon, maar met nog twee secties. De kop bevat inline CSS voor het opmaken van een groep. Het lichaam gebruikt twee groepen met [ inhoudplaceholders ](#content-placeholders) gebruikend een prefix.

```handlebars {line-numbers="true" highlight="33"}
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
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    <!-- Pod1 -->
        <div class="pod">
            <h2>{{ pod1_header }}</h2>
            <p>{{ pod1_body }}</p>
        </div>
        <!-- End of Pod1 -->
    <!-- Pod2 -->
        <div class="pod">
            <h2>{{ pod2_header }}</h2>
            <p>{{ pod2_body }}</p>
        </div>
        <!-- End of Pod2 -->
    </div>
</body>
</html>
```

+++

+++Voorbeeld: Meta-advertentiesjabloon

Hier volgt een eenvoudig voorbeeld van een advertentiesjabloon van Meta. De kop bevat inline CSS voor opmaak. Het lichaam gebruikt [ inhoudplaceholders ](#content-placeholders) gebruikend een prefix.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">"{{ headline }}"</div>
    <div class="ad-body">"{{ body }}"</div>
    <a href="(https://example.com)" class="ad-cta">"{{ CTA }}"</a>
</div>
</body>
</html>
```

+++
