---
title: Middelen en ervaringen beheren
description: Vereenvoudig en verbeter het beheer van merkgoedgekeurde bedrijfsmiddelen voor gebruik en hergebruik in uw digitale marketingreis.
feature: Content, Assets, Experiences
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
source-git-commit: 624629700d8bf7d9e4c0e6d8b4373f40b14d4e05
workflow-type: tm+mt
source-wordcount: '1290'
ht-degree: 0%

---

# Middelen en ervaringen beheren

Adobe GenStudio for Performance Marketing [!DNL Content] vereenvoudigt en verbetert het beheer van merkgoedgekeurde middelen voor gebruik en hergebruik in uw digitale marketingreis.

## [!DNL Content] galerie

Op de galerie ziet u een overzicht van goedgekeurde middelen, ervaringen of sjablonen, afhankelijk van de geselecteerde weergave. Met het filterpictogram (trechter) boven de linkerkant van de tabel opent u het menu **[!UICONTROL Filter]** . Hier kunt u uit veel categorieën kiezen om de inhoud in de galerie te filteren. Klik in de _[!UICONTROL Assets]_-weergave op het pictogram Zoeken (vergrootglas) om een trefwoord te gebruiken om een element te zoeken.

In het volgende voorbeeld ziet u een zoekopdracht naar de term `space` in de [!UICONTROL Assets] -galerie:

![ de mening van Assets met onderzoek op ruimte ](/help/assets/content-assets-filter.png " die naar activa met ruimteattributen zoekt ")

### Inhoud zoeken

De filter en onderzoeksinterface is snel en ontvankelijk, en verstrekt een productieve onderzoek-eerste ervaring. Elke [!DNL Content] -weergave biedt filteropties om uw zoekopdracht te beperken tot het ideale element, de ideale ervaring of de ideale sjabloon. Voor elementen en ervaringen kunt u een campagne en specifieke richtlijnen selecteren, zoals inhoud die voor een bepaald product is gemaakt.

Er zijn filters die op [ worden gebaseerd sleutelwoorden ](asset-details.md#user-defined-metadata) en [ attributencategorieën ](/help/user-guide/insights/attributes.md#categories) aan smalle onderzoeksresultaten. U kunt bijvoorbeeld een element van een bepaald bestandstype of een bepaald onderwerp zoeken om een nieuwe ervaring voor uw campagne op te bouwen. Of u kunt inhoud filteren op basis van uw gebruikersnaam of de naam van een teamlid:

- **[!UICONTROL Uploaded by]** beperkt de lijst van _[!UICONTROL Assets]_om alleen de elementen te tonen die door u of een specifieke persoon zijn geüpload.
- **[!UICONTROL Created by]** beperkt de lijst van _[!UICONTROL Experiences]_om slechts de ervaringen te tonen die door u of een specifieke persoon worden gecreeerd.

**om naar inhoud te zoeken om** opnieuw te gebruiken:

1. Selecteer in _[!DNL Content]_de sectie **[!UICONTROL Assets]**.

1. Selecteer een opslagplaats voor middelen in de lijst **[!UICONTROL Location]** of controleer of u naar de juiste opslagplaats voor middelen kijkt. `GenStudio assets` is de standaardopslagplaats.

   >[!IMPORTANT]
   >
   >De _lijst van de Plaats_ is beschikbaar slechts wanneer u [ met een bewaarplaats van AEM ](connect-aem-repo.md) verbindt.

1. Klik op **[!UICONTROL Search]** (vergrootglas) om een trefwoord of beschrijving in te voeren.

1. Verfijn uw zoekopdracht door een categorie in de lijst _[!UICONTROL Filter]_te selecteren. Bijvoorbeeld, als u een PNG- dossier zoekt, klik **[!UICONTROL File format]**en kies **PNG**.

   Hoe meer u uw zoekopdracht beperkt, hoe minder filteropties beschikbaar zijn. Klik op **[!UICONTROL Clear all]** om alle filters te verwijderen.

1. Selecteer een element voor een volledige weergave en een lijst met details.

   Klik op **[!UICONTROL Download]** (pijl-omlaag) om het element in uw lokale werkstation te gebruiken.

### Locatie

Elementen die u via het [!DNL Create] -proces of uploaden toevoegt aan [!DNL Content] , worden standaard opgeslagen in de `GenStudio assets` -opslagplaats. De gegevensopslagruimte van `GenStudio assets` is een gegevensopslagruimte voor lezen en schrijven in GenStudio for Performance Marketing. Dit betekent dat u elementen kunt opslaan, bewerken en verwijderen in de `GenStudio assets` -opslagplaats.

In de **[!UICONTROL Location]** -lijst boven de _[!UICONTROL Assets]_-galerie aan de rechterkant kunt u een van de verbonden Adobe Experience Manager (AEM) [!DNL Assets Content Hub] -opslagruimten selecteren.

![ lijst van de Plaats van bewaarplaatsen ](/help/assets/content-location-selection.png " Selecteer een inhoudsbewaarplaats "){width="350"}

Wanneer u een AEM-opslagplaats selecteert, wordt in de galerie een overzicht van de middelen van die opslagplaats weergegeven, zodat u goedgekeurde elementen van deze opslagplaatsen kunt gebruiken als input voor het maken van inhoud. De filteropties veranderen om de categorieën te weerspiegelen die in [!DNL AEM Assets Content Hub] worden gevormd.

Zie [ verbinden een bewaarplaats van AEM ](connect-aem-repo.md) voor begeleiding bij het toevoegen van uw [!DNL AEM Assets Content Hub] bewaarplaats aan GenStudio for Performance Marketing.

De AEM-opslagplaats heeft het kenmerk Alleen-lezen, wat betekent dat u toegang kunt krijgen tot de inhoud, maar dat u geen concepten, nieuwe elementen of metagegevens kunt opslaan in de AEM-opslagplaats. Alle concepten en definitieve updates voor activa, ervaringen, en malplaatjes sparen aan de `GenStudio assets` bewaarplaats met nieuwe [ systeemmeta-gegevens ](asset-details.md#system-metadata).

{{note-aem-assets}}

Een AEM-opslagplaats kan bepaalde licentievereisten afdwingen, zoals het vervallen van activa. Deze elementen zijn mogelijk niet beschikbaar voor gebruik in [!DNL Create] -workflows. Verlopen activa kunnen moeten worden vernieuwd of worden vervangen om de continuïteit van uw projecten te handhaven. Raadpleeg de [!DNL AEM Assets Content Hub] -beheerder voor hulp bij deze middelen.

## Assets-beheer

In [!UICONTROL Content] kunt u uw digitale elementen eenvoudig opslaan, ophalen en beheren. Door gebruik te maken van zowel de `GenStudio assets` repository als de AEM repositories, kunt u ervoor zorgen dat uw middelen goed zijn georganiseerd en toegankelijk zijn voor verschillende marketingcampagnes. Deze benadering met meerdere opslagplaatsen biedt flexibiliteit en controle over het gebruik van bedrijfsmiddelen in verschillende omgevingen, zodat bij marketingactiviteiten alleen goedgekeurde en actuele bedrijfsmiddelen worden gebruikt.

De volgende lijst maakt een lijst van de beheerstaken beschikbaar voor activa, ervaringen, en malplaatjes:

| Taken | Assets | Ervaringen | Sjablonen |
| --------------------------------------------------------- | :----: | :---------: | :-------: |
| [ de details van de Mening ](/help/user-guide/content/asset-details.md) | ✓ | ✓ | ✓ |
| [ creeer ervaring ](/help/user-guide/create/overview.md) |        |             | ✓ |
| [ geef in Adobe Express uit ](#edit-in-express) | ✓ |             |           |
| [ Uitvoer voor Activering ](#export-for-activation) |        | ✓ |           |
| [ verfrissen zich ](/help/user-guide/content/use-templates.md#refresh-template) |   |      | ✓ |
| [ Download ](#download-assets) | ✓ |             | ✓ |
| [ Schrapping ](#delete-assets) | ✓ | ✓ | ✓ |

### Elementen toevoegen

Wanneer u elementen toevoegt aan [!DNL Content] , worden deze standaard opgeslagen in de `GenStudio assets` -opslagruimte. De knop _[!UICONTROL Add assets]_is alleen beschikbaar wanneer de_[!UICONTROL Location]_ de `GenStudio assets` -opslagplaats is.

![ het gebied van de Plaats ](/help/assets/content-location.png " gebied van de Plaats "){width="350"}

**om één of meerdere activa** toe te voegen:

1. Klik in _[!DNL Content]_op **[!UICONTROL Add assets]**.

1. In _voeg uw goedgekeurde activa_ mening toe, laat vallen een dossier of dossiers in de dalingsruimte. U kunt desgewenst bestanden van lokale bestanden selecteren met **[!UICONTROL Browse]** of bestanden importeren uit Dropbox of Microsoft OneDrive.

1. In _voeg details_ sectie toe, selecteer a **[!UICONTROL Campaign name]** of ga een nieuwe naam in.

1. Om ontdekkingscapaciteit te verbeteren, voeg facultatieve details zoals _,_ Naam van het Merk _,_ Gebied _en_ Trefwoorden _in de **Meer details**sectie toe._

   Hoe meer details u verstrekt, hoe meer u de robuuste mogelijkheden van GenStudio for Performance Marketing ervaart. Selecteer een of meer details in de lijst of voer een nieuwe in, indien van toepassing, bijvoorbeeld met trefwoorden. Elk detail dat u toevoegt, wordt onder de lijst weergegeven. Klik op **`x`** om een detail te verwijderen.

   Alle details die u toevoegt, worden toegepast op alle elementen die in deze handeling worden toegevoegd.

   Zie [ details van Meta-gegevens ](/help/user-guide/content/asset-details.md#system-metadata).

1. Klik op **[!UICONTROL Add assets]**.

1. Wanneer de activa uploaden wordt voltooid, klik **Gedaan**.

1. Om uw nieuwe geüploade activa te bekijken, klik **[!UICONTROL Refresh]** van het _Nieuwe beschikbare activa_ bericht bij de bodem van het Canvas.

### Elementen downloaden

**om activa** te downloaden:

1. Selecteer een element of sjabloon in _[!DNL Content]_. Als u op een element klikt, wordt een gefocuste weergave van het element geopend.

1. Klik in de elementweergave op het pictogram **[!UICONTROL Download]** (pijl die omlaag wijst) rechtsboven.

1. De download begint een kopie van het element op de standaarddownloadlocatie te plaatsen.

### Elementen verwijderen

**om activa** te schrappen:

1. Selecteer in _[!DNL Content]_een element, ervaring of sjabloon. Als u op een element klikt, wordt een gefocuste weergave van het element geopend.

1. Klik in de elementweergave op **[!UICONTROL Delete]** (prullenbak) rechtsboven.

1. In de _activa van de Schrapping_ popup, verifieer de activa en klik **[!UICONTROL Delete]**.

## Exporteren voor activering

U kunt een goedgekeurde ervaring voor activering exporteren in een indeling die compatibel is met uw doelkanaal.

**om een ervaring** uit te voeren:

1. Selecteer een ervaring in _[!DNL Content]_. Als u op een ervaring klikt, wordt de gedetailleerde weergave geopend of klikt u op het snelmenu (`...`).

1. Klik op **[!UICONTROL Export for activation]** (vak met pijl naar buiten).

1. In de _Uitvoer voor activering_ popup, selecteer één van de beschikbare formaten:

   - E-mail: `HTML`, `CSV`
   - Meta-, Banner- en Display-advertentie: `HTML`, `JPEG`, `PNG`

Zie [ Activering ](/help/user-guide/activation/overview.md).

## Bewerken in Express

U kunt afbeeldingselementen (JPG of PNG) rechtstreeks in GenStudio for Performance Marketing bewerken met Adobe Express. Het _[!UICONTROL Powered by Adobe Express]_Canvas biedt handige functies om uw afbeeldingen te verbeteren zonder de GenStudio-toepassing te verlaten. U kunt eenvoudig achtergronden verwijderen, generatieve vullingen toepassen, effecten aanpassen en afbeeldingen uitsnijden.

>[!BEGINSHADEBOX]

Criteria voor het verbeteren van afbeeldingen met de functie [!DNL Edit in Adobe Express] :

- Tot de ondersteunde MIME-typen behoren `image/png` en `image/jpeg`
- De minimale afbeeldingsafmetingen zijn 50 x 50 pixels
- De maximale afmetingen van de afbeelding zijn 8000x8000 pixels
- De maximale grootte is 40 MB (40.000.000 bytes)

>[!ENDSHADEBOX]

**om activa met Uitdrukkelijke** uit te geven:

1. Selecteer in _[!DNL Content]_een afbeeldingselement. Als u op een element klikt, wordt een gefocuste weergave van het element geopend.

1. Klik in de elementweergave op het pictogram **[!UICONTROL Edit in Adobe Express]** rechtsboven.

1. Gebruik in het canvas van _[!UICONTROL Powered by Adobe Express]_de Uitdrukkelijke controles op het linkerpaneel om uw beeld te verbeteren.

1. Als u tevreden bent met de bijgewerkte afbeelding, klikt u op **[!UICONTROL Save a copy]** rechtsboven.

1. Selecteer de bestandsindeling JPG of PNG en klik op **[!UICONTROL Save a copy]** .

1. Werk de **[!UICONTROL Asset name]** bij in het pop-upmenu _[!UICONTROL Save a copy of asset]_.

   - Selecteer **[!UICONTROL Same details as original asset]** om de elementdetails over te brengen naar de nieuwe afbeelding.

   - Vouw de sectie **[!UICONTROL More details]** uit om de hulplijnen en andere metagegevens bij te werken.

   >[!TIP]
   >
   >Hoe meer details u verstrekt, hoe meer u de robuuste mogelijkheden van GenStudio for Performance Marketing ervaart. Selecteer een of meer details in de lijst of voer een nieuwe in, indien van toepassing, bijvoorbeeld met trefwoorden. Elk detail dat u toevoegt, wordt onder de lijst weergegeven. Klik op **`x`** om een detail te verwijderen.

1. Klik op **[!UICONTROL Save]**.
