---
title: Afbeeldingen genereren
description: Creeer een beeld, dat de stijl van een verwijzingsbeeld aanpast, in Adobe  [!DNL GenStudio]  voor de Marketing van Prestaties.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="Deze functie is momenteel in Beta, waardoor bepaalde functionaliteit mogelijk beperkt is of kan worden gewijzigd."
role: User
level: Beginner
recommendations: noDisplay
exl-id: c1118ada-7fee-43cd-aff4-eab69539afb4
source-git-commit: 3251d81a6bfb0c1f7d2bf3c5bd319ad4e2237699
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 0%

---

# Afbeeldingen genereren

Met het gebruiken van GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (het pictogram van het schilderpenseel), kunt u _[!DNL On-brand images]_&#x200B;produceren - geproduceerde activa die inspiratie uit een gekozen beeld trekken, die zijn visuele invloed en algemene esthetie vangen.<!-- [two types of images](#image-types) using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon)—_[!DNL On-brand images]_ and _[!DNL Similar images]_. -->

Om een oog-vangend en efficiënt beeld te ontwerpen, adviseert men dat u [&#x200B; richtsnoeren aan GenStudio for Performance Marketing &#x200B;](/help/user-guide/guidelines/add-guidelines.md) toevoegt en de [&#x200B; grondbeginselen van het schrijven herinneringen &#x200B;](/help/user-guide/effective-prompts.md) herziet.

## Afbeeldingstypen

_[!DNL On-brand images]_&#x200B;zijn gegenereerde elementen die inspiratie putten uit een gekozen afbeelding en die de visuele impact en algehele esthetische effecten vastleggen. Deze afbeeldingen worden gemaakt met behulp van afbeeldingen die al beschikbaar zijn in [!DNL Content] en een zorgvuldig gemaakte aanwijzing die het ontwerp begeleidt. Zij houden zich strikt aan zowel de merkrichtlijnen als de parameters die tijdens het productieproces worden gekozen.

_[!DNL On-brand images]_<!-- and _[!DNL Similar images]_ --> neem vastgestelde richtlijnen, parameters, en a [&#x200B; bewust-gemaakte herinnering &#x200B;](/help/user-guide/effective-prompts.md) op om oog-vangstbeeldactiva te leveren.

<!-- * _[!DNL Similar images]_—Image assets created with strong similarity to an existing selected image available in [!DNL Content]. When generating similar images, GenStudio for Performance Marketing redesigns the selected image, giving slight variations on the content to provide variety and nuance. -->

## On-brand-afbeeldingen genereren

U kunt [!DNL On-brand images] genereren aan de hand van gedefinieerde richtlijnen, parameters en een geselecteerde referentieafbeelding. Deze elementen helpen samen met uw vraag het genereren van consistente [!DNL On-brand image] variaties.

### Een referentieafbeelding kiezen

Als u een _[!DNL On-brand images]_-bestand wilt maken, selecteert u een bestaande afbeelding die is opgeslagen in [!DNL Content] . Zie [&#x200B; Beste praktijken voor malplaatjes &#x200B;](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines) voor informatie over gesteunde [!DNL on-brand image] dimensies.

**om een verwijzingsbeeld** te kiezen:

1. Klik in _[!DNL Create]_&#x200B;op **[!UICONTROL On-brand image]**.
1. Gebruik de onderzoeksoptie, naast _Filter_, om een specifiek beeld te vinden.

   ![&#x200B; Uitgezochte verwijzingsbeeld &#x200B;](/help/assets/select-img.png){width="400" zoomable="yes"}

   Om activa van een verbonden [!DNL AEM Assets Content Hub] bewaarplaats te gebruiken, verkies een bewaarplaats van het _drop-down menu van de Plaats_. Filter en selecteer één afbeelding.

1. In de _Uitgezochte beeld_ mening, klik op een beeld.

   De geselecteerde afbeelding kan maximaal 10 MB groot zijn.

1. Klik op **[!UICONTROL Use]**.

   Het canvas, dat fungeert als het centrale knooppunt voor het maken van inhoud, wordt weergegeven.

### Parameters toevoegen

Het opnemen van [&#x200B; richtlijnen &#x200B;](/help/user-guide/guidelines/overview.md) en parameters verbetert het proces van de inhoudgeneratie en is een cruciale voorbereidende stap voor het produceren van [!DNL on-brand image].

**om richtlijnen en parameters** toe te voegen:

1. In het _Basis_ lusje, selecteer a [!DNL Brand] om inhoudsverwezenlijking te informeren.

   Als er geen merken beschikbaar van dit menu zijn, [&#x200B; voeg richtlijnen aan uw GenStudio for Performance Marketing &#x200B;](/help/user-guide/guidelines/add-guidelines.md) toe.

1. Selecteer in _[!UICONTROL Image category]_&#x200B;een afbeeldingscategorie die het beste bij het gewenste resultaat past.

   Afbeeldingscategorieën zijn beschikbaar als er een [!DNL Brand] is geselecteerd. De opties worden bepaald door de geselecteerde [!DNL Brand].

<!-- 1. _(Optional)_ Select a custom model from _[!UICONTROL Model]_.

   Models are available if you access to [custom models in Firefly](https://adobedx.slack.com/archives/CMF1JGMLY/p1743534402774569). The _Models_ list will be blank if you do not have access. -->

1. Selecteer de gewenste hoogte-breedteverhouding in _[!UICONTROL Aspect ratio]_.
1. Klik op **[!UICONTROL Select from Content]** in _[!UICONTROL Style reference]_&#x200B;om een referentieafbeelding toe te voegen. De afbeelding die u selecteert, beïnvloedt de visuele esthesie en diepte van de afbeeldingen die u genereert.

   Om activa van een verbonden [!DNL AEM Assets Content Hub] bewaarplaats te gebruiken, verkies een bewaarplaats van het _drop-down menu van de Plaats_. Filter en selecteer één afbeelding.

1. In het _Geavanceerde_ lusje, selecteer het _type van Inhoud_.

   Dit wordt pre-geselecteerd gebaseerd op de beeldcategorie huidig voor geselecteerde [!DNL Brand] - _Kunst_ of _Foto_ - en is niet editable.

1. Pas de algemene intensiteit van de bestaande visuele kenmerken van de afbeelding aan in _[!UICONTROL Visual intensity]_.

### Een vraag invoeren

Nadat u de parameters hebt geselecteerd, vraagt u met behulp van natuurlijke taal om merkafbeeldingen te genereren.

Zie [&#x200B; efficiënte herinneringen &#x200B;](/help/user-guide/effective-prompts.md) schrijven.

**om een herinnering** in te gaan:

1. Ga een herinnering in de snelle doos in.
1. Klik op **[!UICONTROL Generate]**.

Standaard worden vier variaties gegenereerd, die worden gevoed door de vraag, parameters en inhoud die u hebt toegevoegd, en weergegeven op het canvas.

### Bewerken in Adobe Express

Nadat u afbeeldingsvarianten hebt gegenereerd, kunt u deze rechtstreeks in Adobe GenStudio for Performance Marketing bewerken met behulp van Adobe Express.

**om een individueel beeld uit te geven gebruikend Adobe Express**:

1. Houd de muisaanwijzer boven een gegenereerde afbeeldingsvariant en klik op _[!UICONTROL Edit in Adobe Express]_.

   A _Aangedreven door Adobe Express_ venster verschijnt.

1. Voer beeld uit het uitgeven, zoals [&#x200B; uitsnijdend een beeld &#x200B;](https://helpx.adobe.com/nl/express/create-and-edit-images/edit-images/crop-images.html), [&#x200B; verwijderend een voorwerp &#x200B;](https://helpx.adobe.com/nl/express/create-and-edit-images/create-and-modify-with-generative-ai/remove-objects-generative-fill.html), en het toepassen van gevolgen.

   Zie {de documentatie van 0} Adobe Express [&#x200B; leren hoe te herzien beelden in GenStudio for Performance Marketing met Adobe Express.](https://helpx.adobe.com/nl/express/user-guide.html)

1. Klik op _[!UICONTROL Apply changes]_&#x200B;om uw bewerkingen op te slaan.
1. Bewerk de afzonderlijke afbeeldingsvarianten naar wens en pas de wijzigingen toe om de voortgang op te slaan.

### Uitlijning van inhoud controleren

Om de geproduceerde varianten te optimaliseren en strikte naleving van merkidentiteit, platformrichtlijnen, en toegankelijkheidsnormen te verzekeren, hefboomwerking de macht van het [_paneel van de controle van de Inhoud 1&rbrace;_. &#x200B;](/help/user-guide/guidelines/brand-validation.md#content-check-panel) In dit deelvenster worden uitgebreide details van inhoudscontroles weergegeven en worden verbeteringsgebieden belicht.

**om inhoudcontroles uit te voeren**:

1. Klik het _paneelpictogram van de controle van de Inhoud 1&rbrace; in de juiste actiebar om het_ controle van de Inhoud [_paneel_ te openen. &#x200B;](/help/user-guide/guidelines/brand-validation.md#content-check-panel) Bekijk een samenvatting van het *overzicht van Behoeften* en *overgegaan* controles om te zien welke secties en richtlijnen verbetering vergen.

   ![_de controle van de Inhoud_ paneel &#x200B;](/help/assets/content-check-img.png){width="500" zoomable="yes"}

1. Wijzig de afbeeldingsvarianten om ervoor te zorgen dat de varianten nauw overeenkomen met de uitgevoerde inhoudscontroles.

Zie [&#x200B; Bevestiging van de Merk &#x200B;](/help/user-guide/guidelines/brand-validation.md).

<!-- ## Generate Similar images

You can quickly generate images similar to a selected image within [!DNL Content] from the [!DNL Create] home.

**To create _[!DNL Similar images]_**:

1. In _[!DNL Create]_, click **[!UICONTROL Similar images]**.
1. Use the search option, adjacent to _Filter_, to find a specific image.

   To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ drop-down menu. Filter and select one image.

1. In the _Select image_ view, click on an image.
1. Click **[!UICONTROL Use]**.

   The Canvas, which serves as the central hub for content creation, is displayed. Four image variations similar to the original selected image appear.

   ![Generate similar images](/help/assets/generate-similar.png){width="400" zoomable="yes"} -->

## Afbeeldingen publiceren en exporteren

De geproduceerde beeldontwerpen worden getoond in de _sectie van Recenten_ van het [!DNL Create] huis.

Als u de gegenereerde afbeeldingen beschikbaar wilt maken voor gebruik in de huidige en toekomstige versie, publiceert u ze naar [!UICONTROL Content] en exporteert u deze voor gebruik in uw marketingcampagnes.

1. **om uw nieuwe beelden** te publiceren, klik **[!UICONTROL Publish]** in de hoogste toolbar.
   1. _[!UICONTROL Add details]_, zoals&#x200B;_[!UICONTROL Campaigns]_ of _[!UICONTROL Channels]_, indien gewenst.
   1. Klik op **[!UICONTROL Publish]**.

1. **om uw nieuwe beelden** uit te voeren, klik **[!UICONTROL Export]** in de hoogste toolbar.
   1. Selecteer de indeling JPG of PNG en klik op **[!UICONTROL Export]** .

Zie [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) .
