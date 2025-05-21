---
title: Een sjabloon aanpassen
description: Leer hoe u uw HTML-sjabloon kunt aanpassen met plaatsaanduidingen voor inhoud die worden herkend door de generatieve AI van Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation, Generative AI
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: f6c00f473d561cae123997ab3e310867fbdf60d1
workflow-type: tm+mt
source-wordcount: '1527'
ht-degree: 0%

---

# Een sjabloon aanpassen

U kunt een sjabloon aanpassen voor gebruik in GenStudio for Performance Marketing door plaatsaanduidingen voor inhoud of velden in te voegen die de generatieve AI gebruikt om inhoud in te voegen.

In de volgende secties wordt uitgelegd hoe u uw HTML-sjablonen voor GenStudio for Performance Marketing kunt aanpassen met de sjabloontaal _[!DNL Handlebars]_. In de syntaxis van [!DNL Handlebars] wordt gewone tekst met dubbele accolades gebruikt als plaatsaanduidingen voor inhoud. Zie [ wat  [!DNL Handlebars] ](https://handlebarsjs.com/guide/#what-is-handlebars) in de_ de taalgids van Handlebars _is om te leren hoe te om uw malplaatje voor te bereiden.

Zodra uw malplaatje klaar is, kunt u het [ uploaden aan GenStudio for Performance Marketing ](use-templates.md#upload-a-template) en beginnen gepersonaliseerde e-mails te produceren die op uw douanemalplaatje worden gebaseerd.

>[!TIP]
>
>Volg [ toegankelijkheidsrichtlijnen ](accessibility-for-templates.md) en [ beste praktijken ](/help/user-guide/content/best-practices-for-templates.md) zodat u meer van uw publiek kunt bereiken en een optimale ervaring verstrekken.

## Plaatsaanduidingen voor inhoud

GenStudio for Performance Marketing erkent bepaalde [ elementen ](use-templates.md#template-elements) binnen een malplaatje, maar slechts als u hen met a [ erkende gebiedsnaam ](#recognized-field-names) identificeert.

In de kop of de hoofdtekst van een HTML-sjabloon kunt u de syntaxis van [!DNL Handlebars] gebruiken om een tijdelijke aanduiding voor inhoud in te voegen op de plaats waar u GenStudio for Performance Marketing nodig hebt om de sjabloon te vullen met werkelijke inhoud. GenStudio for Performance Marketing erkent en interpreteert deze placeholders die op de [ worden gebaseerd erkende _gebied_ naam ](#recognized-field-names). Elke veldnaam is gekoppeld aan specifieke regels en gedragingen die bepalen hoe inhoud wordt gegenereerd en in de sjabloon wordt ingevoegd.

U kunt `{{headline}}` bijvoorbeeld gebruiken met de syntaxis van [!DNL Handlebars] om aan te geven waar de kop van de e-mail moet worden geplaatst. GenStudio herkent dit veld, genereert een relevante kop op basis van uw richtlijnen en criteria en voegt de kop op deze locatie in:

```handlebars
<div>{{headline}}</div>
```

### Erkende veldnamen

In de volgende tabel staan de veldnamen die door GenStudio for Performance Marketing worden herkend voor het toevoegen van een tijdelijke aanduiding aan een sjabloon. Elk gebied volgt specifieke kanaalrichtlijnen, instructies LLM, en rol-basis regels. Voeg deze veldnamen met de syntaxis [!DNL Handlebars] toe aan uw sjabloon waar u GenStudio for Performance Marketing nodig hebt om een bepaald type inhoud te genereren.

| Veld | Rol | Kanaalsjabloon |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}` | Preheader | email |
| `{{headline}}` | Titel | E-mail <br> Meta en <br> Banner en de Beeld van de Vertoning <br> LinkedIn ad |
| `{{sub_headline}}` | Subkop | E-mail <br> Banner en de advertentie van de Vertoning |
| `{{introductory_text}}` | Inleidende tekst | LinkedIn en |
| `{{body}}` | Platte kopie | E-mail <br> Meta en <br> Banner en de advertentie van de Vertoning |
| `{{cta}}` | Vraag aan actie <br> Zie [ Vraag aan actie ](#calls-to-action) | E-mail <br> Meta en <br> Banner en de Beeld van de Vertoning <br> LinkedIn ad |
| `{{image}}` | Afbeelding—selecteren vanuit [!DNL Content] | E-mail <br> Meta en <br> Banner en de Beeld van de Vertoning <br> LinkedIn ad |
| `{{on_image_text}}` | Op beeldtekst <br> zie [ op beeldtekst ](#on-image-text). | Meta en <br> LinkedIn ad |
| `{{link}}` | Call to action op beeld <br> zie [ Verbinding op beeld ](#link-on-image). | email |

<!-- | `{{brand_logo}}`        | Logo of selected brand<br>See [Brand logo field name](#brand-logo-field-name). | email<br>Meta ad <br>LinkedIn ad | -->

GenStudio for Performance Marketing genereert automatisch bepaalde velden in de volgende sjablonen:

- **E-mailmalplaatje** vereist u niet om het `subject` gebied te identificeren
- **Meta en malplaatje** vereist u niet om `headline` te identificeren, `body`, en `CTA` gebieden
- **Banner en de advertentiesjabloon van de Vertoning** vereist u niet om het `CTA` gebied te identificeren
- **LinkedIn en malplaatje** vereist u niet om `headline` te identificeren, `introductory_text`, en `CTA` gebieden

>[!WARNING]
>
>Voor Instagram-advertenties wordt de gegenereerde kop niet weergegeven in de uiteindelijke ervaring.

Er geldt een limiet van 20 velden wanneer u een sjabloon uploadt naar GenStudio for Performance Marketing. Aangezien het veld `subject` automatisch wordt gegenereerd in een e-mail, telt het als één veld. Dit betekent dat er 19 velden zijn toegestaan in een e-mailsjabloon.

>[!TIP]
>
>U kunt uw malplaatje verifiëren gebruikend de [ malplaatjevoorproef ](#template-preview) in GenStudio for Performance Marketing.

### Oproepen tot actie

Een Oproep tot actie (CTA) omvat een uitdrukking en een verbinding. De functies _[!UICONTROL Rephrase]_&#x200B;en&#x200B;_[!UICONTROL Add link]_ werken alleen correct tijdens het genereren van varianten als u plaatsaanduidingen voor de koppeling en de woordgroep in de sjabloon opneemt.

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

GenStudio for Performance Marketing kan variantvraag-aan-actie uitdrukkingen, ook verstrekken. Zie [ herzien Call to action ](/help/user-guide/create/manage-variants.md#revise-call-to-action).

### Koppeling op afbeelding

U kunt uw e-mailsjabloon aanpassen, zodat ontwerpers een koppeling naar een afbeelding kunnen toevoegen. Net als bij de CTA-koppeling kunt u de volgende richtlijnen gebruiken om een tijdelijke aanduiding `link` toe te passen op een afbeeldingstag:

```html
<a href="{{link}}"><img src="image-source.jpg" alt="{{imageDescription}}"></a>
```

In dit voorbeeld:

- `{{link}}` is een plaatsaanduiding voor de werkelijke URL.
- `src="image-source.jpg"` moet worden vervangen door de URL van de eigenlijke afbeeldingsbron.
- `{{imageDescription}}` is een door de gebruiker gedefinieerde veldnaam die een tijdelijke aanduiding voor de alternatieve tekst van de afbeelding biedt. Dit is handig voor toegankelijkheid en SEO.

### Alternatieve tekst

Gebruik een door de gebruiker gedefinieerde veldnaam als plaatsaanduiding om een alternatieve tekstbeschrijving (HTML `alt="text"` -kenmerk) voor een afbeelding te genereren. De volgende tijdelijke aanduiding voor `{{imageDescription}}` wordt gebruikt met het `{{image}}` veld binnen dezelfde tag `<img>` , zodat de relatie tussen de afbeelding en de beschrijving behouden blijft.

```html
<img src="{{image}}" alt="{{imageDescription}}">
```

In dit voorbeeld:

- `{{image}}` is de plaatsaanduiding voor de URL van de afbeeldingsbron.
- `{{imageDescription}}` is de plaatsaanduiding voor de alt-tekst. Deze bevat een beschrijving van de afbeelding voor toegankelijkheids- en SEO-doeleinden.

### Op afbeeldingstekst

De tijdelijke aanduiding `{{on_image_text}}` wordt gebruikt om een tekstbedekking op te geven met korte, onzichtbare berichten die rechtstreeks in een ervaring op de afbeelding worden geplaatst.

```html
<div class="image-text">{{on_image_text}}</div>
```

<!-- this field does not work in Create canvas 2025/03

### Brand logo field name

At this time, you cannot select the brand logo for the template upload. The following examples demonstrate two methods that conditionally render the brand logo. Each method verifies the source, provides a default or alternative image in case the brand logo is not available, and applies a style:

**Example 1**: Using [!DNL Handlebars] Built-in Helpers condition directly in the HTML `img src` attribute:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Example 2**: Using [!DNL Handlebars] Built-in condition statement to wrap the HTML `img` tag:

```html
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

-->

### Handmatige veldnamen

Alle andere veldnamen worden door de gebruiker gedefinieerd en worden behandeld als handmatig gevulde velden. U wilt bijvoorbeeld een sectie reserveren voor voettekstinhoud.

Als u een bewerkbare sectie wilt maken, voegt u dubbele haakjes toe rond de sectienaam:

```html
<tbody>
    <tr>
        <td>
            <p><span class="footer-text">{{footerLegal}}</span></p>
        </td>
    </tr>
</tbody>
```

## Secties of groepen

U kunt secties in een marketing e-mailmalplaatje gebruiken wanneer u twee of drie groepen gebieden hebt. _Secties_ informeren GenStudio for Performance Marketing dat de gebieden in deze sectie een hoge graad van coherentie vereisen. Als u deze relatie instelt, kan de AI inhoud genereren die overeenkomt met de creatieve elementen in de sectie.


Gebruik een groepsnaam van uw keuze als voorvoegsel om aan te geven dat een veld deel uitmaakt van een sectie of groep. Gebruik een veldnaam (zoals `headline` , `body` , `image` of `cta` ) na het onderstrepingsteken ( `_` ).

Syntaxis: `groupname_fieldname`

- _Correct_ (👍): `pod1_body`
- _Onjuist_ (❌): `pod1body`

Elke sectie kan slechts één van elk gebiedstype gebruiken. De volgende velden behoren bijvoorbeeld tot de sectie `pod1` :

- `pod1_headline`
- `pod1_body`
- `pod1_image`
- `pod1_cta`

Vanwege deze regel kunnen de secties niet worden genest.

Elk sjabloontype, zoals een e-mail- of Meta-advertentie, heeft kanaalspecifieke beperkingen voor het gebruik van secties. Zie [ kanaal-specifieke richtlijnen ](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates#follow-channel-specific-template-guidelines) in _Beste praktijken voor het gebruiken van malplaatjes_ onderwerp.

Een e-mailsjabloon kan bijvoorbeeld maximaal drie secties bevatten. Daarom kunt u drie kopregels en hoofdtekstsecties gebruiken:

- `pre_header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

GenStudio for Performance Marketing begrijpt dat `pod1_headline` nauwer verwant is aan `pod1_body` dan aan `pod2_body` .

>[!TIP]
>
>Zie [ Gestructureerde herinneringen ](/help/user-guide/effective-prompts.md#structured-prompts) leren hoe te om een herinnering te amberen die variërende inhoud voor elke sectie in een multi-sectiee-mail produceert.

## Sjabloonvoorbeeld

Wanneer u [ een malplaatje ](use-templates.md#upload-a-template) uploadt, scant GenStudio for Performance Marketing het dossier van HTML voor erkende gebieden. Gebruik de voorproef om uw [ malplaatjeelementen ](use-templates.md#template-elements) te herzien en te bevestigen dat u hen behoorlijk met [ erkende gebiedsnamen ](#recognized-field-names) identificeerde.

Voorbeeld van een e-mailsjabloon:

&lbrace;de gebieden van de Voorproef ontdekte ![&#128279;](/help/assets/template-detected-fields.png " Controle ontdekte gebieden "){zoomable="yes"}

Zie [ de coderedacteur van het Malplaatje ](/help/user-guide/content/code-editor.md).

### Voorvertoning besturen

U kunt de zichtbaarheid van speciale inhoud bepalen met behulp van ingebouwde hulpmiddelen (speciale expressies in de sjabloontaal [!DNL Handlebars] die bepaalde handelingen uitvoeren). U kunt bijvoorbeeld een voorwaardelijke instructie toevoegen waarmee trackingparameters worden toegevoegd aan koppelingen in de geëxporteerde sjabloon terwijl de voorbeeldkoppelingen schoon blijven.

De waarde `_genStudio.browser` wordt ingesteld bij het renderen van een sjabloon en de waarde `genStudio.export` wordt ingesteld bij het exporteren van een sjabloon. U kunt besluiten om bepaalde inhoud bij de bovenkant van een e-mail te omvatten gebruikend een voorwaardelijke omslag, bijvoorbeeld wanneer het malplaatje voor de uitvoer wordt gebruikt:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Een ander voorbeeld kan zijn om het gebruik van volgcodes te verhinderen wanneer het previewing van een malplaatje in GenStudio for Performance Marketing. In het volgende voorbeeld ziet u hoe u volgparameters toevoegt aan koppelingen in de geëxporteerde sjabloon, terwijl de voorbeeldkoppelingen ongewijzigd blijven:

```html
<a class="button" {{#if _genStudio.browser }}
   href="{{link}}"{{/if}}{{#if _genStudio.export }}
   href="{{link}}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{cta}}</a>
```

## Statische inhoud

E-mail- en metasjablonen zijn vaak gekoppeld aan afbeeldingen en CSS-bestanden die op andere domeinen worden gehost. Wanneer GenStudio for Performance Marketing miniaturen genereert voor sjabloonvoorvertoningen of de ervaringen die daaruit zijn afgeleid, wordt de inhoudsbron gevalideerd en wordt een kopie ingesloten voor voorvertoningen.

Externe bestanden worden alleen tijdelijk ingesloten om de voorvertoning van de sjabloon te maken, zodat de voorvertoning de inhoud correct weergeeft zoals deze wordt weergegeven op het moment dat u de sjabloon maakt. Deze externe dossiers worden **niet** permanent opgeslagen in GenStudio for Performance Marketing. Nadat de sjabloonvoorvertoning is gemaakt, gaat GenStudio for Performance Marketing door met het verwijzen naar de oorspronkelijke bronkoppeling in de sjabloon.

### Inhoud vernieuwen

Als de bron na het creëren van de aanvankelijke voorproef verandert, gebruik [ verfrist ](/help/user-guide/content/use-templates.md#refresh-template) functie om de malplaatjevoorproef met de meest recente versie van de inhoud van de externe bronnen bij te werken.

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

+++Voorbeeld: Meta-advertentiesjabloon

Hier volgt een eenvoudig voorbeeld van een advertentiesjabloon van Meta. De kop bevat inline CSS voor opmaak. Het lichaam gebruikt [ inhoudplaceholders ](#content-placeholders), zoals `image` en `on_image_text`, om erop te wijzen waar GenStudio for Performance Marketing inhoud kan produceren.

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
