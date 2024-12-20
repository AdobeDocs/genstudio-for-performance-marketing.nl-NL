---
title: Werken met sjablonen
description: Ontdek hoe u sjablonen effectief kunt gebruiken om uw creatieve proces in Adobe GenStudio for Performance Marketing te stroomlijnen.
feature: Templates, Content
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: e9c398cc81413fc22746d85abd6444c6bd42efe4
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 0%

---

# Werken met sjablonen

GenStudio for Performance Marketing laat inhoudsmakers toe om verenigbare on-brand marketing inhoud snel te produceren gebruikend _malplaatjes_. Een malplaatje vermindert beduidend de tijd en de inspanning die wordt vereist om nieuwe inhoud te produceren door een uitgangspunt te verstrekken dat pre-gevormde lay-outs en ontwerpelementen omvat.

Hoewel GenStudio for Performance Marketing het rechtstreeks maken van sjablonen in de toepassing niet ondersteunt, kunt u eenvoudig sjablonen ontwerpen en voorbereiden met populaire ontwerpgereedschappen, zoals Adobe InDesign, Illustrator of Express. Zodra uw ontwerp volledig is, kunt u het voor gebruik in GenStudio for Performance Marketing aanpassen. Voer de volgende stappen uit om sjablonen te gebruiken:

1. **Ontwerp Uw Malplaatje**: Gebruik uw aangewezen ontwerphulpmiddel om de visuele lay-out van uw [ malplaatje met elementen ](#template-elements) zoals preheader, titel, lichaam, CTA, beelden, en footer tot stand te brengen.

2. **Code Uw Malplaatje**: Zet uw ontwerp in HTML en gealigneerde CSS om ervoor te zorgen het schoon en ontvankelijk over diverse apparaten is. Overweeg de [ toegankelijkheidsrichtlijnen ](accessibility-for-templates.md) om in het bereiken van uw maximum voorgenomen publiek te helpen.

3. **voorbereidingen voor GenStudio for Performance Marketing**: Pas uw malplaatje van HTML aan gebruikend de het malplaatjetaal van Handlebars. Voeg plaatsaanduidingen in om aan te geven waar GenStudio for Performance Marketing inhoud dynamisch moet genereren. Zie hoe te [ een malplaatje ](customize-template.md) voor GenStudio for Performance Marketing aanpassen.

Met deze stappen kunt u professionele en effectieve sjablonen maken die klaar zijn voor gebruik in GenStudio for Performance Marketing, zodat u on-brand-inhoud snel en efficiënt kunt produceren.

## Sjabloonelementen

Een sjabloon is een set instructies die zijn gedefinieerd met HTML en inline CSS die kunnen worden gebruikt om een e-mail, sociale advertentie of een weergave en ervaring te maken. Sjabloonelementen bieden de structuur voor het maken van inhoud.

Hieronder volgt een lijst met elementen die worden gebruikt in sjablonen en enkele details over de kenmerken ervan:

- **Preheader**

   - Handelt als secundaire onderwerpregel in een e-mail, die de belangrijkste onderwerpregel verbetert
   - Tussen 40 en 50 tekens
   - Zichtbaar in het Postvak IN naast het onderwerp voordat het e-mailbericht wordt geopend
   - Gebruikt in e-mailsjablonen

- **Kopbal**

   - Bovenste gedeelte van de e-mail die de ontvanger ziet bij het openen van de e-mail
   - Hiermee wordt de tint ingesteld en wordt de context voor de opgenomen inhoud aangegeven
   - Gebruikt in e-mailsjablonen

- **Titel**

   - Eerste inhoud die de ontvanger ziet
   - Moet dwingend zijn om rente te vangen
   - Gebruikt in metagegevenssjablonen

- **Lichaam**

   - Belangrijkste inhoudsgebied waar het primaire bericht wordt overgebracht
   - Kan tekst, afbeeldingen en andere media opnemen
   - Gebruikt in e-mail en Meta-advertentiesjablonen

- **CTA (Vraag-aan-Actie)**

   - moedigt de ontvanger aan een specifieke actie te ondernemen, zoals het klikken op een koppeling of het doen van een aankoop
   - Gebruikt in e-mail en Meta-advertentiesjablonen

- **Beelden**

   - Verbetert visuele aantrekkingskracht
   - Tekst opdelen
   - Het bericht ondersteunen
   - Moet van hoge kwaliteit zijn en moet opgevangen worden
   - Gebruikt in e-mail en Meta-advertentiesjablonen

- **Voettekst**

   - Sectie onder met aanvullende inhoud, zoals contactgegevens, koppelingen naar sociale media, disclaimers en opties voor het afmelden van abonnementen
   - Gebruikt in e-mailsjablonen

- **de Bedekking van de Tekst**

   - Tekst op een afbeelding
   - Gebruik om de kop en het lichaam te ondersteunen en te verbeteren
   - Gebruikt in metagegevenssjablonen

>[!TIP]
>
>Zie [ erkende gebiedsnamen ](customize-template.md#recognized-field-names) die GenStudio for Performance Marketing voor malplaatjes van elk type van het Kanaal steunt.

## Sjabloon aanpassen

U [ past uw malplaatje ](customize-template.md) voor gebruik in GenStudio for Performance Marketing aan door inhoudplaceholders, of gebieden op te nemen, die generatieve AI gebruikt om inhoud op te nemen. GenStudio for Performance Marketing herkent bepaalde velden, zoals het veld `body` , en volgt de kanaalrichtlijnen die voor het geselecteerde merk zijn geconfigureerd.

>[!TIP]
>
>Volg [ toegankelijkheidsrichtlijnen ](accessibility-for-templates.md) en [ beste praktijken ](/help/user-guide/content/best-practices-for-templates.md) zodat u meer van uw publiek kunt bereiken en een optimale ervaring verstrekken.

## Sjablonen beheren

Op de galerie [!DNL Templates] wordt uw overzicht weergegeven van sjablonen die zijn aangepast voor het genereren van ervaringen in GenStudio for Performance Marketing. U kunt sjablonen filteren op het kanaaltype, zoals e-mail-, weergave- en metagegevensadvertenties.

![ het malplaatjelijst van de Inhoud ](/help/assets/content-templates.png){width="650" zoomable="yes"}

### Een sjabloon toevoegen

Alvorens een malplaatje te uploaden, zorg ervoor het volledig voorbereid en klaar voor gebruik in GenStudio for Performance Marketing door [ te volgen past malplaatjes ](customize-template.md) begeleiding aan.

**om een malplaatje** toe te voegen:

1. Selecteer in _[!DNL Content]_de sectie **[!UICONTROL Templates]**.

1. Klik op **[!UICONTROL Add template]**.

1. Blader in het deelvenster _[!UICONTROL Add your approved template]_naar het sjabloonbestand HTML of sleep het sjabloonbestand HTML naar de dropruimte. Klik op **[!UICONTROL Next]**.

1. Controleer de gedetecteerde velden in het deelvenster _[!UICONTROL Review discovered fields]_. Controleer of u de juiste sjabloon gebruikt en of alle details naar verwachting zijn. Klik op **[!UICONTROL Next]**.

   Voorbeeld van een e-mailsjabloon:

   ![ ontdekte gebieden van de Voorproef ](/help/assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >Als de sjabloon niet correct is, klikt u op **[!UICONTROL Back]** en gaat u terug naar de vorige stap. Upload het gecorrigeerde sjabloonbestand.

1. Geef in het deelvenster _[!UICONTROL Provide template details and upload]_de sjabloon een naam en selecteer een **[!UICONTROL Channel]**type.

   Sjabloonnaam en kanaaltype zijn vereist. Aanvullende eisen kunnen onder meer zijn:

   - **Meta**: vereist Verhouding
   - **de advertenties van de Vertoning**: vereist Dimensionen

1. Voeg zoveel details toe als u kunt om sjabloonidentificatie in zoekopdrachten en filteren te verbeteren.

1. Klik op **[!UICONTROL Done]**.

### Sjabloon vernieuwen

Sjablonen kunnen statische bestanden bevatten, zoals pictogrammen of logo&#39;s. Met Vernieuwen kunt u de sjabloonvoorvertoning bijwerken met de meest recente versies van deze elementen.

**om het malplaatje** te verfrissen:

1. Selecteer in _[!DNL Content]_de sectie **[!UICONTROL Templates]**.

1. Klik op een sjabloon voor een volledige weergave en een lijst met details.

1. Klik op **[!UICONTROL Refresh]** (cirkelende pijlen) in de rechterbovenhoek om alle elementen die in de sjabloon worden gebruikt, te vernieuwen.

### Een ervaring maken met een sjabloon

Zoek en gebruik een bestaande sjabloon in GenStudio for Performance Marketing om meer ervaringen te creëren.

**om een ervaring met een malplaatje** tot stand te brengen:

1. Selecteer in _[!DNL Content]_de sectie **[!UICONTROL Templates]**.

1. Klik op een sjabloon voor een volledige weergave en een lijst met details.

1. Klik op **[!UICONTROL Create Experience]** (penseel) in de rechterbovenhoek om de sjabloon te gebruiken.

1. Ga aan [ ](/help/user-guide/create/overview.md) tot stand brengen een ervaring.
