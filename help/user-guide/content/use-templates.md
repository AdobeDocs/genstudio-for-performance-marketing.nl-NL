---
title: Werken met sjablonen
description: Ontdek hoe u sjablonen effectief kunt gebruiken om uw creatieve proces in Adobe GenStudio for Performance Marketing te stroomlijnen.
level: Intermediate
role: Developer
feature: Media Templates
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: 1f62546f4fc2381bcc4d8fd3acadd1d6470ed9e8
workflow-type: tm+mt
source-wordcount: '1294'
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

Een sjabloon is een set instructies die zijn gedefinieerd met HTML en inline CSS en die kunnen worden gebruikt om een e-mail, sociale advertentie of advertentie-ervaring te produceren. Sjabloonelementen bieden de structuur voor het maken van inhoud.

Hieronder volgt een lijst met elementen die worden gebruikt in sjablonen en enkele details over de kenmerken ervan:

| **Element** | **Kanaal** | **Beschrijving** |
|----------------------|------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Preheader** | E-mail | Een secundaire onderwerpregel in een e-mail, meestal tussen 40 en 50 tekens, die de hoofdonderwerpregel verbetert. Het is zichtbaar in het postvak naast het onderwerp voordat het e-mailbericht wordt geopend. |
| **Kopbal** | E-mail | In het bovenste gedeelte van de e-mail die de ontvanger ziet wanneer deze de e-mail opent, wordt de toon en context voor de opgenomen inhoud ingesteld. |
| **Titel** | Metaadvertentie, banner en weergaveadvertenties, LinkedIn | De eerste inhoud die de ontvanger ziet, zou dwingend moeten zijn om interesse te vangen. |
| **sub-headline** | E-mail-, banner- en weergaveadvertenties | Een secundair tekstelement dat de kop ondersteunt. Het is doorgaans beknopt en ontworpen om de hoofdkop aan te vullen, zodat de aandacht van de lezer verder in de inhoud wordt getrokken. |
| **Inleidende tekst** | LinkedIn | Het primaire bericht brengt het kernbericht over, gelijkend op lichaamskopie. Het kan tot 150 karakters, met inbegrip van ruimten, een maximum van vier emojis, en punctuatie gebruiken. |
| **Lichaam** | E-mail-, metagegevens-, banner- en weergaveadvertenties | De hoofdtekst van de advertentie geeft het kernbericht weer. Het zou moeten engageren, informatief, en overtuigend zijn om de gewenste actie van het publiek aan te moedigen. |
| **CTA** | E-mail-, metagegevens-, banner- en weergaveadvertenties, LinkedIn | Een call-to-action-knop gebruikt een uitdrukking en een koppeling om de ontvanger aan te moedigen een specifieke actie te ondernemen, zoals klikken op een koppeling of een aankoop doen. |
| **Beelden** | E-mail-, metagegevens-, banner- en weergaveadvertenties, LinkedIn | Verbeter visuele aantrekkingskracht, verbreek tekst en ondersteun het bericht. Afbeeldingen moeten van hoge kwaliteit en opvallend zijn. |
| **Voettekst** | E-mail | Het onderste gedeelte van het e-mailbericht bevat aanvullende inhoud, zoals contactgegevens, koppelingen naar sociale media, disclaimers en opties voor het opzeggen van abonnementen. |
| **de Bedekking van de Tekst** | Meta en | Tekst die op een afbeelding wordt geplaatst ter ondersteuning en verbetering van de kop- en tekstinhoud. |

>[!TIP]
>
>Zie [ erkende gebiedsnamen ](customize-template.md#recognized-field-names) die GenStudio for Performance Marketing voor malplaatjes van elk type van het Kanaal steunt.

## Sjabloon aanpassen

U [ past uw malplaatje ](customize-template.md) voor gebruik in GenStudio for Performance Marketing aan door inhoudplaceholders, of gebieden op te nemen, die generatieve AI gebruikt om inhoud op te nemen. GenStudio for Performance Marketing herkent bepaalde velden, zoals het veld `body` , en volgt de kanaalrichtlijnen die voor het geselecteerde merk zijn geconfigureerd.

>[!TIP]
>
>Volg [ toegankelijkheidsrichtlijnen ](accessibility-for-templates.md) en [ beste praktijken ](/help/user-guide/content/best-practices-for-templates.md) zodat u meer van uw publiek kunt bereiken en een optimale ervaring verstrekken.

## Sjablonen beheren

Op de galerie _[!DNL Templates]_&#x200B;wordt uw overzicht weergegeven van sjablonen die zijn aangepast voor het genereren van ervaringen in GenStudio for Performance Marketing.

### Zoeksjablonen

Elke [!DNL Content] -weergave biedt filteropties om uw zoekopdracht te beperken tot het ideale element, de ideale ervaring of de ideale sjabloon. Er zijn filters die op [ richtlijnen ](/help/user-guide/guidelines/overview.md) worden gebaseerd, [ sleutelwoorden ](asset-details.md#user-defined-metadata), en [ kenmerkencategorieën ](/help/user-guide/insights/attributes.md#categories) om onderzoeksresultaten te beperken.

U kunt bijvoorbeeld een sjabloon zoeken met een specifiek kanaaltype of een bepaalde hoogte-breedteverhouding die door u is gemaakt:

- **[!UICONTROL Created by]**: hiermee wordt de lijst van _[!UICONTROL Templates]_&#x200B;beperkt, zodat alleen de sjablonen worden weergegeven die door u of een specifieke persoon zijn gemaakt.
- **[!UICONTROL Aspect Ratio]** : hiermee wordt de lijst in _[!UICONTROL Templates]_&#x200B;beperkt tot sjablonen die zijn ontworpen voor een specifieke hoogte-breedteverhouding.

In het volgende voorbeeld wordt het filter weergegeven op basis van het kanaaltype, zoals e-mail, advertenties weergeven, metagegevensadvertenties en LinkedIn-advertenties.

![ de lijst van het malplaatje van de Inhoud ](/help/assets/content-templates-filter.png " Onderzoek LinkedIn malplaatjes "){width="650" zoomable="yes"}

De zoekfunctie voor sjablonen is beschikbaar tijdens [!UICONTROL Create] wanneer u een sjabloon selecteert voor media die eigendom zijn van of betaald worden. Als bepaalde filteropties niet zichtbaar zijn, geeft dit aan dat geen sjablonen in de gegevensopslagruimte overeenkomen met de overeenkomstige metagegevenscriteria. Zorg ervoor dat sjablonen correct zijn gecodeerd met metagegevens, zodat deze kunnen worden gedetecteerd via deze filters.

### Een sjabloon toevoegen

Alvorens een malplaatje te uploaden, zorg ervoor het volledig voorbereid en klaar voor gebruik in GenStudio for Performance Marketing door de begeleiding in [ te volgen past malplaatjes ](customize-template.md) aan.

**om een malplaatje** toe te voegen:

1. Selecteer in _[!DNL Content]_&#x200B;de sectie **[!UICONTROL Templates]**.

1. Klik op **[!UICONTROL Add template]**.

1. Blader in het deelvenster _[!UICONTROL Add your approved template]_&#x200B;naar het HTML-sjabloonbestand of sleep het HTML-sjabloonbestand naar de dropruimte. Klik op **[!UICONTROL Next]**.

1. Controleer de velden in het deelvenster _[!UICONTROL Check detected fields]_. Controleer of u de juiste sjabloon gebruikt en of alle details naar verwachting zijn.

   Voorbeeld van een e-mailsjabloon:

   ![ ontdekte gebieden van de Voorproef ](/help/assets/template-detected-fields.png){width="650" zoomable="yes"}

   >[!TIP]
   >
   >Als de sjabloon niet correct is, klikt u op **[!UICONTROL Back]** en gaat u terug naar de vorige stap. Upload het gecorrigeerde sjabloonbestand. Of gebruik de [ redacteur van de malplaatjecode ](/help/user-guide/content/code-editor.md) om eenvoudige correcties aan te brengen.

1. Klik op **[!UICONTROL Next]** als u tevreden bent met de voorvertoning van de sjabloon.

1. Geef in _[!UICONTROL Provide template details and upload]_&#x200B;de sjabloon een naam en selecteer een **[!UICONTROL Channel]**&#x200B;type.

   Sjabloonnaam en kanaaltype zijn vereist. Aanvullende eisen kunnen onder meer zijn:

   - **Meta**: vereist Verhouding
   - **Banner en de advertentie van de Vertoning**: vereist Dimensies

1. Voeg zoveel details toe als u kunt om sjabloonidentificatie in zoekopdrachten en filteren te verbeteren.

1. Klik op **[!UICONTROL Done]**.

### Sjabloon vernieuwen

Sjablonen kunnen statische bestanden bevatten, zoals pictogrammen of logo&#39;s. [ de Statische inhoud ](/help/user-guide/content/customize-template.md#static-content) wordt niet opgeslagen na het creëren van de malplaatjevoorproef. GenStudio for Performance Marketing blijft verwijzen naar de bronkoppeling in de sjabloon. Met Vernieuwen kunt u de sjabloonvoorvertoning bijwerken met de meest recente versies van deze elementen.

**om het malplaatje** te verfrissen:

1. Selecteer in _[!DNL Content]_&#x200B;de sectie **[!UICONTROL Templates]**.

1. Klik op een sjabloon voor een volledige weergave en een lijst met details.

1. Klik op **[!UICONTROL Refresh]** (cirkelende pijlen) in de rechterbovenhoek om alle elementen die in de sjabloon worden gebruikt, te vernieuwen.

### Een ervaring maken met een sjabloon

Zoek en gebruik een bestaande sjabloon in GenStudio for Performance Marketing om meer ervaringen te creëren.

**om een ervaring met een malplaatje** tot stand te brengen:

1. Selecteer in _[!DNL Content]_&#x200B;de sectie **[!UICONTROL Templates]**.

1. Klik op een sjabloon voor een volledige weergave en een lijst met details.

1. Klik op **[!UICONTROL Create Experience]** (penseel) in de rechterbovenhoek om de sjabloon te gebruiken.

1. Ga aan [&#128279;](/help/user-guide/create/overview.md#create-use-cases) tot stand brengen een ervaring.

## Sjablonen uit AJO en Marketo

U kunt een sjabloon uploaden die u in Adobe Journey Optimizer (AJO) of Marketo hebt gemaakt. GenStudio for Performance Marketing detecteert toepassingsspecifieke patronen en negeert deze, waarbij het oorspronkelijke formulier behouden blijft voor verder gebruik in AJO of Marketo. U hoeft geen wijzigingen aan te brengen in de oorspronkelijke AJO- of Marketo-syntaxis.

Herkende toepassingspatronen zijn onder meer:

- **AJO**: `{{profile.*}}`, `{{context.*}}`
- **Marketo**: `{{my.*}}`, `{{lead.*}}`, `{{system.*}}`

>[!BEGINSHADEBOX]

**Eerste vereisten**

- De toepassing (AJO, Marketo) en GenStudio for Performance Marketing moeten tot dezelfde IMS Org voor integratie behoren
- Gebruikers moeten de rol Medewerker (het laagste niveau) of hoger hebben

>[!ENDSHADEBOX]

Daarna, [ pas uw malplaatje ](/help/user-guide/content/customize-template.md) met placeholders aan om erop te wijzen waar GenStudio for Performance Marketing inhoud voor u zou moeten produceren. [ voeg uw malplaatje ](#add-a-template) aan de [!DNL Content] bewaarplaats toe en bevestig het malplaatje. Breng eventuele kleine correcties aan met de code-editor.
