---
title: Een e-mailervaring maken
description: Leer hoe u e-mailervaringen kunt maken in Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
source-git-commit: 6c2a8ca1fd981bc4f6eb15f1487b304c0c8f67b4
workflow-type: tm+mt
source-wordcount: '1053'
ht-degree: 0%

---

# Een e-mailervaring maken

Dit leerprogramma toont aan hoe te om gemerkte [ e-mailervaringen ](/help/user-guide/create/email-experiences.md) te produceren gebruikend GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (het pictogram van het schildpenseel in het linkernavigatiegebied).

Om een efficiënte e-mailervaring tot stand te brengen, adviseert men dat u [ richtlijnen aan GenStudio for Performance Marketing ](/help/user-guide/guidelines/add-guidelines.md) toevoegt en omhoog op de [ grondbeginselen van het creëren van een herinnering ](/help/user-guide/effective-prompts.md) alvorens u begint.

## Een sjabloon kiezen

Als u een nieuwe e-mailervaring wilt maken, gebruikt u een beschikbare sjabloon om het framework voor uw inhoud te bieden.

**om een e-mailmalplaatje** te kiezen:

1. Klik in _[!DNL Create]_op **[!UICONTROL Email]**.
1. Gebruik de onderzoeksoptie, naast _Filter_, om een specifiek e-mailmalplaatje te vinden.
1. Klik om een e-mailsjabloon te selecteren en klik op **[!UICONTROL Use]** .

   Het canvas, het epicentrum van het maken van inhoud, wordt weergegeven.

## Parameters toevoegen

Het toevoegen van [ richtlijnen ](/help/user-guide/guidelines/overview.md) en activa in _Parameters_ in de snelle lade vult het proces van de inhoudgeneratie op en is een integrale voorbereidende stap voor het produceren van een e-mailervaring.

Als u een sjabloon gebruikt met vooraf gedefinieerde hulplijnen (zoals [!DNL Brands] , [!DNL Personas] of [!DNL Products] ), gelden deze richtlijnen voor de varianten. U kunt deze desgewenst wijzigen.

**om parameters en activa** toe te voegen:

1. Klik het _pictogram van Parameters_ om de herinnering lade uit te breiden.
1. In de _sectie van Parameters_, uitgezochte richtlijnen - [!DNL Brands], [!DNL Personas], en [!DNL Products] - om inhoudsverwezenlijking te informeren.

   ![ kies persona ](/help/assets/persona-select.png){width="600" zoomable="yes"}

   Als er geen merken, persona&#39;s, of producten beschikbaar van deze menu&#39;s zijn, [ voeg richtlijnen aan uw GenStudio for Performance Marketing ](/help/user-guide/guidelines/add-guidelines.md) toe.

1. Voeg inhoud voor gebruik in de ervaring *en* toe om inhoudsgeneratie te beïnvloeden:
   * Klik op **[!UICONTROL Select from Content]** om elementen (afbeeldingen) te selecteren in de [!DNL Content] -opslagplaats, filter een of meer afbeeldingen en selecteer deze.

     ![ kies visuele inhoud ](/help/assets/content-select-email.png){width="500" zoomable="yes"}

     Om activa van een verbonden [!DNL AEM Assets Content Hub] bewaarplaats te gebruiken, verkies een bewaarplaats van het _2} dropdown menu van de Plaats {._ Filter een of meer afbeeldingen en selecteer deze.

   * Of sleep elementen naar de sectie **[!UICONTROL Select from Content]** om een of meer nieuwe elementen te uploaden.
1. Klik op **[!UICONTROL Use]**.

   >[!NOTE]
   >Als uw e-mailmalplaatje veelvoudige secties heeft, selecteer [!DNL Products] en inhoud (visuele activa) voor elke e-mailsectie in _multi-sectiemails_. E-mailberichten met meerdere secties ondersteunen één visueel middel per sectie. U kunt vanuit [!DNL Content] alleen visuele elementen toevoegen aan e-mailberichten met meerdere secties. U kunt vanuit uw lokale bron geen elementen slepen en neerzetten of uploaden.
   >![ voegt inhoud en parameters voor elke e-mailsectie ](/help/assets/parameters-multisection-email.png){width="450" zoomable="yes"} toe

Wanneer u wordt gebeëindigd toevoegend parameters, kunt u de snelle lade doen ineenstorten door het _pictogram van Parameters_ opnieuw te klikken.

## Een vraag invoeren

Nadat u richtlijnen hebt geselecteerd, kunt u vragen in een natuurlijke taal te schrijven om inhoud te genereren voor uw nieuwe e-mailervaring. Gedetailleerde aanwijzingen leveren een hogere kwaliteit op dan vage of dubbelzinnige aanwijzingen.

Zie [ efficiënte herinneringen ](/help/user-guide/effective-prompts.md) schrijven om meer over het schrijven van herinneringen te leren.

**om een herinnering** in te gaan:

1. Ga een herinnering in _&quot;beschrijf de ervaringen in u &quot;_ snelle doos wilt produceren.
1. Klik op **[!UICONTROL Generate]**.

Standaard worden vier variaties gegenereerd, die allemaal worden geactiveerd door de vraag, de hulplijnen en de inhoud die u hebt toegevoegd, en weergegeven in het canvas.

Gegenereerde inhoud wordt progressief geladen. Elke sectie van de e-mailervaring wordt gegenereerd en wordt weergegeven op het canvas. Zie [ E-mailervaringen ](/help/user-guide/create/meta-experiences.md#progressive-loading) leren hoe die veranderingen in het Canvas worden geladen.

## Door revisie gegenereerde varianten

Voordat u selecteert wat u wilt verzenden voor goedkeuring of publicatie naar [!DNL Content] , kunt u e-mailsecties bewerken of een variant uit de set gegenereerde e-mailberichten verwijderen.

**om geproduceerde varianten** te herzien:

* **[ om de naam van het e-mailontwerp](/help/user-guide/create/manage-variants.md#change-draft-name)** uit te geven, klik in de _Naamloze 4} titel van het Ontwerp bij de bovenkant van het Canvas en ga een nieuwe titel in._
* **om [ een e-mail](/help/user-guide/create/manage-variants.md#manually-edit-text)** manueel uit te geven, klik in om het even welke editable tekstgebieden (zoals de onderwerpregel, kopbal, of lichaamskopie) en geef uit zoals nodig
* **[ om Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)** te veranderen of te selecteren, klik de knoop van call-to-action en selecteer _[!UICONTROL Rephrase]_of_[!UICONTROL Add link]_.
* **om [ tekst toe te passen formatterend](/help/user-guide/create/manage-variants.md#manually-edit-text)** in een variant, klik de tekst op beeld voor een variant en klik **[!UICONTROL Format text]**.
* **[ regenerate een sectie van een variant](/help/user-guide/create/manage-variants.md#re-generate-sections)**, klik een editable tekstgebied en gebruik de _[!UICONTROL Suggested edits]_opties of ga een nieuwe herinnering in en klik **[!UICONTROL Generate]**.
* **om [ beelden in een variant](/help/user-guide/create/manage-variants.md#swap-image)** toe te voegen of te ruilen, klik een beeldactiva (of het gebied van beeldactiva als een beeld momenteel niet bestaat) en klik het **[!UICONTROL Swap from content]** pictogram.
* **[ om een verbinding aan een beeld in een variant](/help/user-guide/create/manage-variants.md#add-image-link)** toe te voegen, klik een beeldactiva (of het gebied van de beeldactiva als een beeld momenteel niet bestaat) en klik het verbindingspictogram.
* **[ om alt tekst voor beelden in een variant](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)** toe te voegen, klik een beeldactiva en gebruik de _alt tekst_ optie om alt tekst per beeld manueel toe te voegen of te produceren.
* **[ om toegankelijkheidsetiketten ](/help/user-guide/create/manage-variants.md#add-accessibility-labels) aan uw varianten** toe te voegen klik op een beeld of verbinding van call-to-action, dan een korte beschrijving verstrekken die verklaart wat de verbinding of de knoop doet.
* **[ om een e-mail](/help/user-guide/create/manage-variants.md#delete-variant)** te schrappen, om de e-mailtitel (bijvoorbeeld, &quot;E-mail 1/4&quot;) te selecteren en **[!UICONTROL Delete variant]** te klikken.

## Feedback op generatie verzenden

Om [ voor te leggen terugkoppelt ](/help/user-guide/create/manage-variants.md#generation-feedback) over de kwaliteit van de generatieoutput, klik het optiepictogram (drie punten) en selecteer **[!UICONTROL Good output]** of **[!UICONTROL Poor output]**.

## Voorvertoning voor apparaat

Wanneer het herzien van en het voorbereiden van e-mailervaringen, kunt u [ schakelen tussen voorproeven voor Desktop en mobiele meningen ](/help/user-guide/create/manage-variants.md#preview-for-device) om coherentie en visuele aantrekkingskracht van ontwerp varianten te verzekeren.

## Uitlijning van inhoud controleren

Om de geproduceerde varianten te optimaliseren en strikte naleving van merkidentiteit, platformrichtlijnen, en toegankelijkheidsnormen te verzekeren, hefboomwerking de macht van het [_paneel van de controle van de Inhoud 1}_. ](/help/user-guide/guidelines/brand-validation.md#content-check-panel) In dit deelvenster worden uitgebreide details van inhoudscontroles weergegeven en worden verbeteringsgebieden belicht.

**om inhoudcontroles op een variant** uit te voeren:

1. Klik het _paneelpictogram van de controle van de Inhoud 1} in de juiste actiebar om het_ controle van de Inhoud [_paneel_ te openen. ](/help/user-guide/guidelines/brand-validation.md#content-check-panel) Bekijk een samenvatting van het *overzicht van Behoeften* en *overgegaan* controles om te zien welke secties en richtlijnen verbetering vergen.

   ![_de controle van de Inhoud_ paneel ](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [ herziet manueel varianten ](#revise-generated-variants) om uw varianten te verzekeren dicht met de uitgevoerde inhoudscontroles worden gericht.

Zie [ Bevestiging van de Merk ](/help/user-guide/guidelines/brand-validation.md).

## Revisies en goedkeuringen ophalen

Gebruik het deelvenster Goedkeuringen, dat als een pictogram op de rechteractiebalk van het canvas kan worden weergegeven, om revisies op te vragen, revisieopmerkingen bij te houden en om goedkeuring te krijgen van belanghebbenden.

**om overzichten en goedkeuringen** te verkrijgen:

1. [ Lanceer een goedkeuringsverzoek ](/help/user-guide/approvals/request-review.md) om een [ goedkeuring van geschreven e-mailervaringen ](/help/user-guide/approvals/approve-content.md) te vragen.
1. [ verwijdert of voegt recensenten ](/help/user-guide/approvals/review-and-edit.md#manage-approvals) tijdens het overzichtsproces toe.
1. [ heb toegang tot de inhoud voor overzicht ](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) en bekijk de verzoeken om herziening.
1. Bewerk de concepten per overzichtscommentaren en [ publiceer uw e-mailervaringen ](#publish-and-export-experience).

Zie [ Revisies en goedkeuringen ](/help/user-guide/approvals/overview.md) voor meer informatie.

## Publiceren en exporteren

Als u de gegenereerde e-mails beschikbaar wilt maken voor huidige en toekomstige gebruik, publiceert u deze naar [!UICONTROL Content] en exporteert u deze voor gebruik in uw marketingcampagnes.

1. **om uw nieuwe e-mailervaring(en)** te publiceren, klik **[!UICONTROL Publish]** in de hoogste toolbar, of binnen de goedkeuringsstroom.
1. **om uw nieuwe e-mailervaring(en) uit te voeren**, klik **[!UICONTROL Export]** in de hoogste toolbar.
   1. Selecteer de indeling (alleen CSV en afbeeldingen of HTML) en klik op **[!UICONTROL Export]** .

Zie [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) voor meer informatie.
