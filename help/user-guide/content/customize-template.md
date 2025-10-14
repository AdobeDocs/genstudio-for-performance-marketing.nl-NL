---
title: Een sjabloon aanpassen
description: Leer hoe u uw HTML-sjabloon kunt aanpassen met plaatsaanduidingen voor inhoud die worden herkend door de generatieve AI van Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation, Generative AI
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 2c5a16f0767958d09cfe5bbaa7a5538ca1b4fe75
workflow-type: tm+mt
source-wordcount: '1610'
ht-degree: 0%

---

# Een sjabloon aanpassen

U kunt een sjabloon aanpassen voor gebruik in GenStudio for Performance Marketing door plaatsaanduidingen voor inhoud of velden in te voegen die de generatieve AI gebruikt om inhoud in te voegen.

In de volgende secties wordt uitgelegd hoe u uw HTML-sjablonen voor GenStudio for Performance Marketing kunt aanpassen met de sjabloontaal _[!DNL Handlebars]_. In de syntaxis van [!DNL Handlebars] wordt gewone tekst met dubbele accolades gebruikt als plaatsaanduidingen voor inhoud. Zie [&#x200B; wat  [!DNL Handlebars] &#x200B;](https://handlebarsjs.com/guide/#what-is-handlebars) in de_ de taalgids van Handlebars _is om te leren hoe te om uw malplaatje voor te bereiden.

Zodra uw malplaatje klaar is, kunt u het [&#x200B; uploaden aan GenStudio for Performance Marketing &#x200B;](use-templates.md#upload-a-template) en beginnen gepersonaliseerde e-mails te produceren die op uw douanemalplaatje worden gebaseerd.

>[!TIP]
>
>Volg [&#x200B; toegankelijkheidsrichtlijnen &#x200B;](accessibility-for-templates.md) en [&#x200B; beste praktijken &#x200B;](/help/user-guide/content/best-practices-for-templates.md) zodat u meer van uw publiek kunt bereiken en een optimale ervaring verstrekken.

## Plaatsaanduidingen voor inhoud

GenStudio for Performance Marketing erkent bepaalde soorten inhoud of [&#x200B; elementen &#x200B;](use-templates.md#template-elements) binnen een malplaatje, maar slechts als u hen met a [&#x200B; erkende gebiedsnaam &#x200B;](#recognized-field-names) identificeert.

In de kop of de hoofdtekst van een HTML-sjabloon kunt u de syntaxis van [!DNL Handlebars] gebruiken om een tijdelijke aanduiding voor inhoud in te voegen op de plaats waar u GenStudio for Performance Marketing nodig hebt om de sjabloon te vullen met werkelijke inhoud. GenStudio for Performance Marketing erkent en interpreteert deze placeholders die op de [&#x200B; worden gebaseerd erkende _gebied_ naam &#x200B;](#recognized-field-names). Elke veldnaam is gekoppeld aan specifieke regels en gedragingen die bepalen hoe inhoud wordt gegenereerd en in de sjabloon wordt ingevoegd.

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
| `{{cta}}` | Vraag aan actie <br> Zie [&#x200B; Vraag aan actie &#x200B;](#calls-to-action) | E-mail <br> Meta en <br> Banner en de Beeld van de Vertoning <br> LinkedIn ad |
| `{{image}}` | Afbeelding—selecteren vanuit [!DNL Content] | E-mail <br> Meta en <br> Banner en de Beeld van de Vertoning <br> LinkedIn ad |
| `{{on_image_text}}` | Op beeldtekst <br> zie [&#x200B; op beeldtekst &#x200B;](#on-image-text). | Meta en <br> LinkedIn ad |
| `{{link}}` | Call to action op beeld <br> zie [&#x200B; Verbinding op beeld &#x200B;](#link-on-image). | email |

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
>U kunt uw malplaatje verifiëren gebruikend de [&#x200B; malplaatjevoorproef &#x200B;](#template-preview) in GenStudio for Performance Marketing.

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

GenStudio for Performance Marketing kan variantvraag-aan-actie uitdrukkingen, ook verstrekken. Zie [&#x200B; herzien Call to action &#x200B;](/help/user-guide/create/manage-variants.md#revise-call-to-action).

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

### Toegankelijkheidslabel

Het kenmerk `aria-label` wordt gebruikt om een toegankelijke naam te definiëren voor elementen die geen zichtbare labels hebben. Dit kenmerk is vooral handig in sjablonen waarin het belangrijk is context te bieden voor interactieve elementen, zoals een CTA-knop.

```html
<a class="button" href="{{link}}" aria-label="{{CTAAriaLabel}}">{{cta}}</a>
```

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

### RTF-bewerking

Verbeter uw creatieve inhoud tijdens het [!DNL Create] -proces met RTF-bewerkingen. Het canvas bepaalt de mogelijkheid voor tekstopmaak op basis van de locatie van de tijdelijke aanduiding voor inhoud. RTF-functionaliteit is alleen beschikbaar wanneer u plaatsaanduidingen voor inhoud gebruikt als zelfstandige elementen of binnen HTML-tags op blokniveau, zoals `<p>` , `<div>` of `<span>` .

RTF-tekstbewerking is beschikbaar voor zelfstandige inhoud in een alinea:

```html
<p>{{body}}</p>
```

Als u een tijdelijke aanduiding voor inhoud binnen een HTML-kenmerk gebruikt (zoals `alt` , `href` of `src` ), wordt RTF-bewerking niet ondersteund voor dat veld.

De rijke tekst geeft uit is **&#x200B;**&#x200B;niet beschikbaar voor `alt` inhoud uit:

```html
<img src="image.jpg" alt="{{image_description}}">
```

Als een veld meerdere keren wordt weergegeven, wordt de mogelijkheid van RTF-opmaak bepaald op basis van het feit of het veld in een van de instanties wordt gebruikt als een HTML-kenmerk. Wanneer de kop bijvoorbeeld wordt gebruikt als een kop en als alternatieve tekst voor een afbeelding, heeft de tag `alt` voorrang.

De rijke tekst geeft uit is **niet** beschikbaar voor `headline` aangezien het als `alt` inhoud wordt gebruikt:

```html
<h1>{{headline}}</h1>
<img src="image.jpg" alt="{{headline}}">
```

Rijke tekstbewerking kan beschikbaar zijn voor bepaalde velden binnen specifieke kanalen, zoals `on_image_text` in sociale kanalen (Meta, LinkedIn).

## Secties of groepen

Als uw e-mailsjabloon meerdere inhoudsgebieden nodig heeft, zoals meerdere aanbiedingen of artikelen, kunt u deze indelen met secties of groepen. _Secties_ informeren GenStudio for Performance Marketing dat de gebieden in deze sectie een hoge graad van coherentie vereisen. Als u deze relatie instelt, kan de AI inhoud genereren die overeenkomt met de creatieve elementen in de sectie.

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

Elk sjabloontype, zoals een e-mail- of Meta-advertentie, heeft kanaalspecifieke beperkingen voor het gebruik van secties. Zie [&#x200B; kanaal-specifieke richtlijnen &#x200B;](/help/user-guide/content/best-practices-for-templates.md) in _Beste praktijken voor het gebruiken van malplaatjes_ onderwerp.

Een e-mailsjabloon kan bijvoorbeeld maximaal drie secties bevatten. Daarom kunt u drie kopregels en hoofdtekstsecties gebruiken:

- `pre_header`
- `pod1_headline`, `pod1_body`
- `pod2_headline`, `pod2_body`
- `pod3_headline`, `pod3_body`
- `cta`

GenStudio for Performance Marketing begrijpt dat `pod1_headline` nauwer verwant is aan `pod1_body` dan aan `pod2_body` .

>[!TIP]
>
>Zie [&#x200B; Gestructureerde herinneringen &#x200B;](/help/user-guide/effective-prompts.md#structured-prompts) leren hoe te om een herinnering te amberen die variërende inhoud voor elke sectie in een multi-sectiee-mail produceert.

## Sjabloonvoorbeeld

Wanneer u [&#x200B; een malplaatje &#x200B;](use-templates.md#upload-a-template) uploadt, scant GenStudio for Performance Marketing het dossier van HTML voor erkende gebieden. Gebruik de voorproef om uw [&#x200B; malplaatjeelementen &#x200B;](use-templates.md#template-elements) te herzien en te bevestigen dat u hen behoorlijk met [&#x200B; erkende gebiedsnamen &#x200B;](#recognized-field-names) identificeerde.

Voorbeeld van een e-mailsjabloon:

&lbrace;de gebieden van de Voorproef ontdekte ![&#128279;](/help/assets/template-detected-fields.png " Controle ontdekte gebieden "){zoomable="yes"}

Zie [&#x200B; de coderedacteur van het Malplaatje &#x200B;](/help/user-guide/content/code-editor.md).

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

Als de bron na het creëren van de aanvankelijke voorproef verandert, gebruik [&#x200B; verfrist &#x200B;](/help/user-guide/content/use-templates.md#refresh-template) functie om de malplaatjevoorproef met de meest recente versie van de inhoud van de externe bronnen bij te werken.
