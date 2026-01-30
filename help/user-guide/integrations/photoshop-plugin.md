---
title: Photoshop-insteekmodule voor Adobe GenStudio for Performance Marketing
description: Leer hoe u de Photoshop-insteekmodule voor GenStudio for Performance Marketing installeert, configureert en gebruikt.
feature: Generative AI
role: User
source-git-commit: bb6b8de80bdf6089e70756bea5dbf3e6a7945052
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# Photoshop-insteekmodule voor GenStudio for Performance Marketing

Met de GenStudio for Performance Marketing Photoshop-plug-in voegt u een deelvenster toe aan Adobe Photoshop waarmee u on-brand-inhoud kunt genereren.

Op deze pagina wordt beschreven hoe u de plug-in kunt installeren en configureren en hoe u deze kunt gebruiken.

Functies van deze plug-in:

* Aanmelden bij een GenStudio for Performance Marketing-instantie met een Adobe ID
* GenStudio for Performance Marketing-velden voor het genereren van inhoud toewijzen aan tekstlagen in een Photoshop-document
* Geef een merk, product, persona en tekstprompt op voor het genereren van inhoud
* Voeg desgewenst een afbeelding toe ter vervanging van de sjabloonafbeelding
* Voorvertoning van gegenereerde variaties in inhoud van het merk
* Gegenereerde inhoud toepassen op toegewezen lagen in het huidige document
* Online-brand-inhoud-vertalingen maken
* Gegenereerde [!DNL Experiences] exporteren naar GenStudio for Performance Marketing

>[!VIDEO](https://video.tv.adobe.com/v/3478808?learn=on)

## De insteekmodule installeren

Volg deze instructies om de plug-in te installeren.

### Vereisten

* Creative Cloud-bureaubladtoepassing
* Photoshop, minimaal versie 25.6.0

### Installatiestappen

1. Download en werk de plug-in bij op de Creative Cloud Marketplace in Adobe Exchange.
1. Onderzoek naar **Insteekmodule van GenStudio voor Photoshop** in Adobe Exchange.
1. Volg de aanwijzingen om de plug-in te installeren.

### De insteekmodule verwijderen

1. Start de Creative Cloud-bureaubladtoepassing.
1. Klik op de optie **[!UICONTROL Plugins]** .
1. Klik op de ellips, **[!UICONTROL (...)]** , op de GenStudio for Creative Cloud-kaart voor opties.
1. Kies **Uninstall**.

## Een sjabloon maken

Als u inhoud wilt genereren, hebt u een GenStudio for Performance Marketing-sjabloon nodig die op basis van uw Photoshop-document is gemaakt.

Een GenStudio-ready sjabloon maken:

1. Open een document in Photoshop.
1. Een tekstlaag identificeren voor gegenereerde inhoud.
1. Wijzig de naam van de laag met de conventie voor veldnamen: `{<name_of_generated_field>}` . Bijvoorbeeld `{body}` , `{headline}` , `{cta}` .
1. Verander lagen voor alle [ gebieden die door het kanaal worden vereist voor het malplaatjetype ](../../user-guide/templates/customize-template.md#recognized-field-names) worden bedoeld.

| Kanaal | Vereiste velden voor genereren | Optionele velden voor genereren |
| --- | --- | --- |
| LinkedIn | `{on_image_text}`, `{image}` | `{headline}`, `{introductory_text}`, `{cta}`, `{website_url}` |
| Meta | `{on_image_text}`, `{image}` | `{body}`, `{headline}`, `{cta}`, `{website_url}`, `{display_link}` |
| Weergave | `{body}`, `{image}` | `{headline}`, `{cta}`, `{website_url}` |

Meerdere lagen kunnen dezelfde veldaanduiding hebben, maar elke laag kan slechts één veld opgeven. Als het document bijvoorbeeld meerdere tekengebieden bevat:

* U kunt een `{headline}` -laag in elk tekengebied opgeven.
* U kunt meerdere `{headline}` lagen in één tekengebied opgeven.
* U kunt niet opgeven dat één laag de veldnamen `{headline}` en `{cta}` ontvangt.

### Vereisten voor sjabloongrootte

#### Meta-sjablonen

Voor Instagram- en Facebook-berichten:

* Breedte: 1080 px (vast)
* Hoogte: 1080 px of 1350 px

Voor Instagram- en Facebook-artikelen:

* Breedte: 1080 px (vast)
* Hoogte: 1920 px

De insteekmodule bepaalt de chroom van de gegenereerde ervaring op basis van de hoogte van de sjabloon.

#### Sjablonen weergeven

Er is geen vaste grootte vereist. Weergavesjablonen ondersteunen elke gewenste grootte.

#### LinkedIn-sjablonen

* Breedte: 1200 px (vast)
* Hoogte: 1200 px, 628 px, 2292 px, 1800 px of 1500 px

Het document kan nu worden gebruikt met de plug-in.

## Nieuwe inhoud genereren

1. Open Photoshop.
1. Open een GenStudio-klaar sjabloondocument dat u hebt gemaakt (zie bovenstaande instructies) of gebruik de startsjabloon van GenStudio for Performance Marketing: `branding-template-acrobat-handlebars.psd` .
1. Open het deelvenster met plug-ins op **[!UICONTROL Plugins]** > **[!UICONTROL GenStudio]** .
1. Klik op **[!UICONTROL Login]** . Als ertoe aangezet voor toestemming om een URL te openen, naar keuze controle **mijn keus** onthoudt, dan klik **[!UICONTROL Allow]**.
1. Gebruik de webbrowser om u aan te melden met een profiel dat toegang heeft tot GenStudio for Performance Marketing.
1. Selecteer het kanaal (Meta, LinkedIn of Weergave) dat van toepassing is op de sjabloon die u hebt geopend.
   ![ uitgezochte Kanaal ](./ps-select-channel.png){width="300" zoomable="yes"}
1. Selecteer de context [!DNL Brand] , [!DNL Persona] en [!DNL Product] voor het genereren van inhoud.
   ![ Brand, Persona, en Uitgezocht Product ](./ps-select-box.png){width="300" zoomable="yes"}
1. Selecteer het aantal variaties dat u wilt maken.
1. Gebruik de knop onder **[!UICONTROL Select Content]** om door afbeeldingen in uw elementen te bladeren en deze te kiezen. De 40 laatst toegevoegde elementen worden als eerste weergegeven en u kunt zoeken naar andere elementen. De grootte van geselecteerde afbeeldingen wordt automatisch aangepast aan uw sjablonen.
1. Geef een tekstprompt op voor de inhoud in het vak **[!UICONTROL Text Prompt]** .
1. Klik op **[!UICONTROL Generate]** . Variaties worden weergegeven op kaarten in het deelvenster van de plug-in.

Nieuwe documenten worden toegevoegd aan de Photoshop-werkruimte en er wordt gegenereerde inhoud toegepast op de sjabloonvelden. Deze documenten krijgen een genummerd variatieachtervoegsel.

## Inhoud vertalen

Gebruikers kunnen inhoud na het genereren van de kopie vertalen naar ondersteunde talen.

1. Klik op **[!UICONTROL Translate]** nadat u de plug-in hebt gegenereerd en gekopieerd.
1. Selecteer een of meer talen voor de vertaling.
1. Klik op **[!UICONTROL Translate]** .

Nieuwe documenten worden toegevoegd aan de Photoshop-werkruimte en er wordt gegenereerde inhoud toegepast op de sjabloonvelden. Deze documenten krijgen een genummerd variatieachtervoegsel.

## Ervaringen exporteren naar GenStudio

Gebruikers kunnen exporteren nadat inhoud is gegenereerd of vertaald. Geëxporteerde ervaringen worden weergegeven in de inhoudssectie van GenStudio for Performance Marketing.

![ Geëxporteerde die activa in de sectie van de Inhoud worden getoond ](./content-assets.png){width="90%"}

## Problemen oplossen

Houd rekening met de volgende tips en werkwijzen als tekst of afbeeldingen niet worden vervangen in gegenereerde variaties.

### Toegewezen velden

Als tekst of afbeeldingen niet worden vervangen, controleert u of velden correct zijn toegewezen met accolades `{}` (geen haakjes `()` ).

### Bevestig dat fonts beschikbaar zijn

Het font van een tekstveld moet beschikbaar zijn op uw computer voordat het veld tijdens het genereren kan worden vervangen. Controleer of alle lettertypen die in het bestand worden gebruikt, beschikbaar zijn op uw computer, vooral als het bestand op de computer van iemand anders is gemaakt.

### Uitzonderingen voor veldtoewijzing

{{$include /help/_includes/field-mapping-exceptions.md}}
