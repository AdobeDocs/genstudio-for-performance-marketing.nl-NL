---
title: Figma-insteekmodule voor Adobe GenStudio for Performance Marketing
description: Leer hoe u de Figma-plug-in voor GenStudio for Performance Marketing configureert en gebruikt.
feature: Generative AI
role: User
exl-id: 232fbbc6-c523-4525-8d26-a8ac8d62c035
source-git-commit: 4ab7e82336bfa6907331b0684253e48066e7d021
workflow-type: tm+mt
source-wordcount: '1140'
ht-degree: 0%

---

# Figma-insteekmodule voor GenStudio for Performance Marketing

Met de insteekmodule GenStudio for Performance Marketing Figma voegt u een nieuw deelvenster toe aan de toepassing Figma waarmee u inhoud van het merk kunt genereren.
[&#x200B; vind en installeer de stop van de communautaire markt van Figma &#x200B;](https://www.figma.com/community/plugin/1604251370122180013/firefly-enterprise-and-genstudio).

Op deze pagina wordt beschreven hoe u de plug-in configureert en gebruikt.

Functies van deze plug-in:

* Tekstelementen van Figma toewijzen aan GenStudio for Performance Marketing-velden, zoals `headline` , `body` , `on_image_text` en meer.
* Genereer nieuwe on-brand Meta, LinkedIn of Display advertentie [!DNL Experiences] op basis van een merk, persona, product en tekstprompt.
* Maak [!DNL Experiences] rechtstreeks in het figuurdocument door de tekst in de figuuukelementen die zijn toegewezen te vervangen door waarden die door GenStudio for Performance Marketing zijn gegenereerd.
* Bestaande inhoud die is gebaseerd op een vraag, hernoemen, verkorten, verlengen of vertalen.
* Vertaal gegenereerde [!DNL Experiences] naar meerdere talen.
* Exporteer gegenereerde [!DNL Experiences] naar een lokale bron als samengevoegde afbeeldingen.
* Gegenereerde exportbewerking [!DNL Experiences] naar GenStudio for Performance Marketing.
* Gebruik plug-inopties die zich aanpassen aan de geselecteerde elementen in het figuurcanvas.

>[!VIDEO](https://video.tv.adobe.com/v/3478815?captions=dut&learn=on)

## Een sjabloon maken

Voor de insteekmodule zijn de eerste twee niveaus van het Figma-document vereist, zodat deze instelling wordt gebruikt:

* **Sectie** - dit vertegenwoordigt het ouderproject, dat veelvoudige malplaatjes kan bevatten.
* **Kader** - dit vertegenwoordigt een malplaatje binnen een project. De sjabloon kan worden gevuld met tekst, afbeeldingen, componenten en andere elementen.

### Meta-sjablonen

Deze sjabloongrootten worden ondersteund:

Voor Instagram- of Facebook-berichten:

* Breedte: 1080 px (vast)
* Hoogte: 1080 px of 1350 px

Voor Instagram- of Facebook-artikelen:

* Breedte: 1080 px (vast)
* Hoogte: 1920 px

De insteekmodule bepaalt de chroom van de gegenereerde ervaring op basis van de hoogte van de sjabloon.

### Sjablonen weergeven

Er is geen vaste grootte vereist. Weergavesjablonen ondersteunen elke gewenste grootte.

### LinkedIn-sjablonen

* Breedte: 1200 px (vast)
* Hoogte: 1200 px, 628 px, 2292 px, 1800 px of 1500 px

### Veldroltoewijzing

De plug-in moet inzicht hebben in de verschillende elementen van de sjabloon, zoals een kop, platte tekst of afbeelding.

Elementrollen toewijzen:

1. Selecteer een element in de sjabloon (tekst, afbeelding, enzovoort).
1. Gebruik het vervolgkeuzemenu om een rol toe te wijzen.

De plug-in onthoudt deze toewijzingen voor gegenereerde inhoud. Een veldrol kan worden toegewezen aan meerdere sjabloonelementen.

![&#x200B; roltoewijzing van het Gebied &#x200B;](./field-role-mapping.png){width="600"}

### Uitzonderingen voor veldtoewijzing

{{$include /help/_includes/field-mapping-exceptions.md}}

## Nieuwe inhoud genereren

Met GenStudio for Performance Marketing AI kunt u elementen in figuursjablonen genereren of variëren.

1. Als u de GenStudio Plugin Playground of reeds voorbereide malplaatjes gebruikt, selecteer de sectieknoopknoop die uw advertentiesjablonen bevat. U kunt dit van het **paneel van Lagen** doen of door direct op de sectie in het canvas te klikken.
   ![&#x200B; Sectie selecteren of variaties &#x200B;](./plugin-playground.png){width="500" zoomable="yes"}
1. Voer in het insteekmodulevenster een projectnaam in voor de variaties, kies een platform voor de inhoud en vul de andere vereiste informatie in. Klik vervolgens op de knop **[!UICONTROL Finish Setup]** .
   ![&#x200B; het projectvenster van de Opstelling &#x200B;](./setup-project.png){width="300" zoomable="yes"}
1. Selecteer de [!DNL Brand] , [!DNL Persona] en [!DNL Product] die u wilt gebruiken voor het genereren van inhoud.
1. Selecteer het aantal variaties dat u wilt maken (maximaal acht).
1. Gebruik de knop onder **[!UICONTROL Select Content]** om door afbeeldingen in uw elementen te bladeren en deze te kiezen. De 40 laatst toegevoegde elementen worden als eerste weergegeven en u kunt zoeken naar andere elementen. De grootte van geselecteerde afbeeldingen wordt automatisch aangepast aan uw sjablonen.
1. Voer een tekstprompt in. Voor elk veld in de lijst **[!UICONTROL Fields]** is de optie **[!UICONTROL Action]** ingesteld op **[!UICONTROL Generate]** voor nieuwe inhoud.
1. Wijs alle veldrollen toe. Zie [&#x200B; rolafbeelding van het Gebied &#x200B;](#field-role-mapping).
1. Klik op **[!UICONTROL Generate]** .

## Variaties vertalen of genereren en kopiëren op basis van bestaande inhoud

Gebruik GenStudio for Performance Marketing AI om variaties te genereren en te kopiëren of Figmasjablonen te vertalen.

1. Selecteer het sectieknooppunt dat uw advertentiesjablonen bevat. U kunt dit van het **paneel van Lagen** doen of door direct op de sectie in het canvas te klikken.
   ![&#x200B; Sectie selecteren of variaties &#x200B;](./plugin-playground.png){width="500" zoomable="yes"}
1. Voer in het insteekmodulevenster een projectnaam in voor de variaties en kies een platform voor de inhoud.
1. Selecteer **[!UICONTROL What is the goal?]** of **[!UICONTROL Generate Variations]** in **[!UICONTROL Translate]** en klik op de knop **[!UICONTROL Finish Setup]** .
   ![&#x200B; het projectvenster van de Opstelling &#x200B;](./setup-project.png){width="300" zoomable="yes"}
1. Selecteer de [!DNL Brand] , [!DNL Persona] en [!DNL Product] die u wilt gebruiken voor het genereren van inhoud.
1. Selecteer het aantal variaties dat u wilt maken.
1. Gebruik de knop onder **[!UICONTROL Select Content]** om door afbeeldingen in uw elementen te bladeren en deze te kiezen. De 40 laatst toegevoegde elementen worden als eerste weergegeven en u kunt zoeken naar andere elementen. De grootte van geselecteerde afbeeldingen wordt automatisch aangepast aan uw sjablonen.
1. Voer een tekstprompt in. Voor elk veld in de lijst **[!UICONTROL Fields]** is de optie **[!UICONTROL Action]** ingesteld op **[!UICONTROL Generate]** voor nieuwe inhoud.
1. Wijs alle veldrollen toe. Zie [&#x200B; rolafbeelding van het Gebied &#x200B;](#field-role-mapping).
1. Selecteer elk veldtype om variaties te genereren of vertalen in het deelvenster aan de linkerkant van de plug-in en plak de initiële inhoud in elk **[!UICONTROL Initial Content]** -vak.
   ![&#x200B; tekst van de Steekproef in de Aanvankelijke doos van de Inhoud &#x200B;](./initial-content-box.png){width="60%" zoomable="yes"}
1. Klik op **[!UICONTROL Generate]** .

## Inhoud vertalen na generatie

1. Selecteer een generatie die u wilt vertalen.
   ![&#x200B; Uitgezochte generatie &#x200B;](./select-generation.png){width="200" zoomable="yes"}
1. Kies **[!UICONTROL Translation]** en klik op **[!UICONTROL Translate]** .
1. Selecteer de doeltaal of -talen.
1. Klik op **[!UICONTROL Select]**.

De vertaalresultaten omvatten:

* Er wordt een nieuwe pagina weergegeven met vertaalde inhoud.
* Bij elke vertaling wordt de doeltaal of -landinstelling weergegeven.
* De oorspronkelijke inhoud blijft ongewijzigd op de oorspronkelijke pagina.

![&#x200B; de resultaten van de Vertaling &#x200B;](./translation-results.png){width="60%" zoomable="yes"}

## Overige acties voor inhoudsvelden na genereren

Wanneer u bestaande inhoud in een veld bewerkt, worden nuttige opties weergegeven in het deelvenster van de plug-in.

![&#x200B; opties van de Acties van de Insteekmodule &#x200B;](./figma-other-actions.png){width="300" zoomable="yes"}

U kunt onder andere de volgende opties kiezen:

* Wijzig de **[!UICONTROL Value]** als u de tekst rechtstreeks wilt wijzigen. Als u deze inhoud wijzigt, wordt deze automatisch toegepast op alle geselecteerde variaties.
* De AI kan vele **[!UICONTROL Action]** opties uitvoeren, die omvatten:

| Handeling | Beschrijving |
| --- | --- |
| **[!UICONTROL Generate]** | Genereer een nieuwe tekstvariatie. |
| **[!UICONTROL Rephrase]** | Genereer een nieuwe tekstvariatie. |
| **[!UICONTROL Shorten]** | Een kortere tekstvariatie genereren. |
| **[!UICONTROL Lengthen]** | Een langere tekstvariatie genereren. |

Nadat u een optie **[!UICONTROL Action]** hebt geselecteerd, kunt u de inhoud opnieuw genereren met de knop **[!UICONTROL Regenerate]** .

## Exportervaringen

Variaties kunnen uit Figma worden geëxporteerd als GenStudio for Performance Marketing [!DNL Experiences] .

1. Voer een van de volgende handelingen uit om de inhoud te selecteren die u wilt exporteren in het figuurcanvas:
   * Selecteer de sectie Genereren op het canvas en klik vervolgens op **[!UICONTROL Mark all for Export]** in het deelvenster Plug-in.
     ![&#x200B; de sectie van de Generatie selecteren &#x200B;](./select-generation-section.png){width="200" zoomable="yes"}
   * Selecteer een afzonderlijke generatie op het canvas en klik op **[!UICONTROL Mark for Export]** in het deelvenster Plug-in.
     ![&#x200B; Individuele generatie uitgezocht &#x200B;](./select-generation.png){width="200" zoomable="yes"}
1. Selecteer het item Exporteren in het zijbalkmenu.
   ![&#x200B; Teken voor de knoop van de Uitvoer die voor een Meta wordt getoond en &#x200B;](./mark-for-export.png){width="60%" zoomable="yes"}
1. Selecteer een doel.
1. Klik op **[!UICONTROL Export]** om de inhoud te exporteren.

Er wordt een ZIP-bestand gemaakt in het deelvenster met insteekmodules of er wordt een koppeling naar **[!UICONTROL Open in GenStudio]** weergegeven. Gebruik de koppeling ZIP om aan te geven waar u het bestand wilt opslaan of selecteer **[!UICONTROL Open in GenStudio]** .

## Generatiegeschiedenis

De plug-in bewaart een geschiedenis met wijzigingen voor elk veld. Kies op de sjabloonpagina de optie **[!UICONTROL Generation history]** in het zijpaneel van de plug-in.

![&#x200B; de geschiedenisoptie van de Generatie die voor een Meta wordt getoond en &#x200B;](./generation-history.png){width="80%" zoomable="yes"}

## Problemen oplossen

Houd rekening met de volgende tips en werkwijzen als tekst of afbeeldingen niet worden vervangen in gegenereerde variaties.

### Toegewezen velden

Als tekst of afbeeldingen niet worden vervangen, controleert u of de velden zijn toegewezen aan GenStudio-veldrollen in de gebruikersinterface van de plug-in. Zie [&#x200B; rolafbeelding van het Gebied &#x200B;](#field-role-mapping).

### Bevestig dat fonts beschikbaar zijn

Het font van een tekstveld moet beschikbaar zijn op uw computer voordat het veld tijdens het genereren kan worden vervangen. Controleer of alle lettertypen die in het bestand worden gebruikt, beschikbaar zijn op uw computer, vooral als het bestand op de computer van iemand anders is gemaakt.

### Ondersteuning voor veldrollen overwegen

Bepaalde kanalen ondersteunen alleen vervanging in specifieke velden. Ben zich bewust van uitzonderingen voor [&#x200B; kaart van de gebiedsrol &#x200B;](#field-role-mapping).
