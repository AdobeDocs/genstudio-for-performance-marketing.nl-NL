---
title: Gegevens van element
description: Adobe GenStudio for Performance Marketing slaat goedgekeurde inhoud op met rijke metagegevens voor zoekbaarheid en het bijhouden van prestaties.
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: f401f93e7dd08db4837b8709e28acec5571052f7
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# Gegevens van element

Adobe GenStudio for Performance Marketing slaat goedgekeurde inhoud op met rijke metagegevens voor ontdekkingsmogelijkheden en het bijhouden van prestaties.

Elk element (met inbegrip van ervaringen en malplaatjes) heeft _details_ (meta-gegevens) geassocieerd die helpen zich identificeren, volgen, gebruiken, en van inhoudsprestaties leren.

**om activa details** te bekijken:

1. Selecteer in _[!DNL Content]_een element, ervaring of sjabloon. Als u op een element klikt, wordt een gefocuste weergave van het element geopend.

1. Reviseer in de elementweergave de _[!UICONTROL Details]_-sectie aan de rechterkant.

1. Als de sectie _[!UICONTROL Details]_niet zichtbaar is, klikt u op het pictogram **[!UICONTROL Information]**(i).

De gegevens van elementen omvatten metagegevens die zijn toegepast tijdens het maken of uploaden van bestanden. De meta-gegevenstypes van activa omvatten [ systeemmeta-gegevens ](#system-metadata) en [ user-defined meta-gegevens ](#user-defined-metadata).

Het volgende afbeeldingselement bevat systeemmetagegevens die het bestandstype, de grootte en andere kenmerken, één door de gebruiker gedefinieerd trefwoord en diverse door AI gedetecteerde kenmerken en kleuren beschrijven.

![ details van activa met veelvoudige markeringen ](/help/assets/content-asset-details.png)

>[!NOTE]
>
>Assets van AEM-opslagplaatsen geven verschillende metagegevens weer. Zie [ activa zicht ](connect-aem-repo.md#step-4-configure-asset-visibility) vormen om te leren hoe te om [!DNL AEM Assets Content Hub] activa details te vormen.

## Systeemmetagegevens

Bepaalde metagegevens van elementen worden automatisch verzameld wanneer een element wordt geüpload, zoals bestandstype, grootte, afmetingen, bron en meer. Met uitzondering van de bestandsnaam kunt u de standaardmetagegevens van het systeem niet bewerken.

### Gegenereerde tags

Als u een goedgekeurd element opslaat in [!DNL Content] , gebruikt GenStudio for Performance Marketing de leermogelijkheden van Adobe AI en computers om het middel te bestuderen en labels toe te passen op basis van de functies van het element. Een afbeelding van een kat kan bijvoorbeeld kenmerkcodes als `pet photography` of `cat` opleveren en kleurcodes die dominante kleuren in de afbeelding identificeren. U kunt geen labels bewerken die worden gedetecteerd en automatisch worden toegepast.

Zie [!DNL Insights] [ categorieën van Attributen ](/help/user-guide/insights/attributes.md#categories) voor gedetailleerde lijsten van beeld, video, en teksteigenschappen.

### Metagegevens over gegenereerde inhoud

De informatie die wordt gebruikt om een nieuw middel of een nieuwe ervaring te produceren wordt meta-gegevens, zoals de herinnering die werd gebruikt. U kunt de vraag niet bewerken nadat de inhoud is goedgekeurd, maar u kunt deze wel gebruiken als beginplaats voor het genereren van iets nieuws.

## Door gebruiker gedefinieerde metagegevens

Door de gebruiker gedefinieerde metagegevens voegen marketingcontext toe aan de inhoud van het element, zodat marketers kunnen begrijpen hoe het element moet worden gebruikt en hoe het moet worden gebruikt.

Wanneer u [ activa ](/help/user-guide/content/manage-assets.md#add-assets) uploadt, kunt u een reeks facultatieve activadetails bepalen die in GenStudio for Performance Marketing als meta-gegevens bestaan. Het opnemen van meer details kan activa identificatie in onderzoeken en het filtreren verbeteren.

**om de user-defined meta-gegevens** uit te geven:

1. Selecteer in _[!DNL Content]_een element, ervaring of sjabloon. Als u op een element klikt, wordt een gefocuste weergave van het element geopend.

1. Reviseer in de elementweergave de _[!UICONTROL Details]_-sectie aan de rechterkant.

1. Klik op **[!UICONTROL Edit details]** (potlood) om de metagegevens van elementen, ervaringen of sjablonen te bewerken.

   Hoe meer details u verstrekt, hoe meer u de robuuste mogelijkheden van GenStudio for Performance Marketing ervaart. Selecteer een of meer details in de lijst of voer een nieuwe in, indien van toepassing, bijvoorbeeld met trefwoorden. Elk detail dat u toevoegt, wordt onder de lijst weergegeven. Klik op **`x`** om een detail te verwijderen.

### Metagegevens

In de volgende tabel worden de metagegevens (elementdetails) weergegeven die u kunt definiëren wanneer u een element maakt.

| Veld | Beschrijving |
| -------------- | ----------- |
| Titel | Naam van het element; de standaardtitel kan de oorspronkelijke bestandsnaam zijn |
| [!DNL Campaigns] | [[!DNL Campaigns]](/help/user-guide/campaigns/overview.md) omvat promotionele inhoud met verenigbaar overseinen voor het bereiken van een bedrijfsdoel <br> het klikken op een campagneverbinding neemt u aan de overzichtspagina van de campagne |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) toegevoegd aan GenStudio for Performance Marketing en gepubliceerd voor gebruik |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) toegevoegd aan GenStudio for Performance Marketing voor gebruik |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) toegevoegd aan GenStudio for Performance Marketing voor gebruik |
| Kanalen | Platforms voor het distribueren van bepaalde inhoudstypen, zoals e-mail en banner en advertentie weergeven |
| [!UICONTROL Timeframe] | Tijdsduur waarvoor het actief wordt gebruikt, zoals kwartaal, seizoen, jaar enz. Voorbeeld: `Winter 2023` |
| Regio | Regio’s waarvoor het actief wordt gebruikt. Voorbeelden: `North America` , `APAC` , `Italy` |
| Taal | Talen waarvoor het middel wordt gebruikt. Voorbeeld: `Spanish` |
| Trefwoorden | Door de gebruiker gedefinieerde trefwoorden worden gebruikt voor de verdere identificatie van de kenmerken en het doel van het element |

>[!TIP]
>
>Klik op **[!UICONTROL Edit details]** (potlood) om metagegevens van elementen te bewerken. U kunt bijvoorbeeld de elementnaam wijzigen of trefwoorden toevoegen of verwijderen.

## Algemene context

In de sectie [!UICONTROL Generative Context] ziet u welke informatie is gebruikt om de ervaring te genereren, zoals de sectie `Prompt` die tijdens het [!DNL Create] -proces wordt gebruikt. Dit inzicht kan u helpen om nog succesvollere varianten te bouwen.

De informatie kan omvatten:

- De parameters `Brand` , `Product` en `Persona` zijn geselecteerd tijdens het [!DNL Create] -proces
- `Subject line` en `Preheader` voor e-mailervaringen
- `Headline` en `Body` voor Meta-advertenties

## Historie

Vouw de sectie _[!UICONTROL History]_in een ervaring uit om een tijdlijn van goedkeuringen en activiteit weer te geven. Een goedgekeurde ervaring onthult bijvoorbeeld de goedkeuringsdatum, -tijd en -fiatteur:

```
Approved

December 10, 2024 at 6:00 PM by Username
```
