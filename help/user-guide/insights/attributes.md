---
title: Overzicht van kenmerken
description: Leer hoe u de prestaties van specifieke kenmerken in Adobe GenStudio for Performance Marketing kunt beoordelen.
level: Intermediate
feature: Reporting and Insights, Content Attributes, Content Performance
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# Overzicht van kenmerken

In de weergave [!DNL Insights] _[!UICONTROL Attributes]_ziet u een lijst met kenmerken die worden gebruikt in advertentiecampagnes voor het geselecteerde kanaalaccount.

{{connect-insights}}

De tabel _[!UICONTROL Attributes]_wordt ingedeeld met de naam [!UICONTROL Attribute] . U kunt schakelen tussen de lijsttypen met de knop **[!UICONTROL Images]**en de knop **[!UICONTROL Video]**. Klik op het instellingenpictogram (cog) boven de rechterkant van de tabel om de weer te geven kolommen in en uit te schakelen.

![ de filter en lijst van Attributen ](/help/assets/insights-attributes-filter.png){zoomable="yes"}

{{filter-table}}

## Kenmerkdetails

De attributen helpen om [ advertenties ](ads.md#ad-details) en [ media ](media.md#media-details) door hun inherente details, zoals kleur, samenstelling, visuele elementen, en andere eigenschappen te identificeren.

In de weergave met kenmerkdetails kunt u zien welke advertenties het geselecteerde kenmerk gebruiken. De details omvatten totale kenmerkprestaties en een uitsplitsing van de prestatiesmetriek met betrekking tot elke advertentie.

![ de prestatiemetriek van Attributen ](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing detecteert bepaalde functies en past het juiste kenmerk toe op media-inhoud of advertentie als tag. Zie [ Categorieën ](#categories) voor voorbeelden van deze markeringen. Als u alle kenmerken wilt zien die aan een advertentie zijn gekoppeld, klikt u op het pictogram voor instellingen (cog) boven de rechterkant van de tabel om de kolom **[!UICONTROL Attributes]** te selecteren.

## Categorieën

Een attribuut _categorie_ is een classificatiegroep die verwante attributen organiseert die een gemeenschappelijk kenmerk delen. Deze categorieën helpen de ontdekking, identificatie, en begrip van specifieke attributen te stroomlijnen door grotere context te verstrekken en hun toepassing en gebruik te vergemakkelijken.

GenStudio for Performance Marketing gebruikt Adobe AI en machine het leren mogelijkheden om [ beelden ](image-features.md) te bestuderen, [ video&#39;s ](video-features.md), en [ tekst ](text-features.md) en attributen op advertenties en media toe te passen die op een waarschijnlijkheid van correctheid worden gebaseerd.

De lijst met gedetecteerde kenmerken voor advertenties en media-inhoud is niet limitatief. Inhoud die een uitgebreide reeks functies bevat, kan worden beperkt tot de drie belangrijkste kenmerken die door de AI worden geïdentificeerd. De volgende afbeelding bevat bijvoorbeeld verschillende gedetecteerde afbeeldingskenmerken, waaronder meerdere objecten, voorgrond- en achtergrondkleuren:

![ beeldattributen ](/help/assets/category/asset-attributes.png " Beeld van Toucan omvat veelvoudige ontdekte attributen "){width="300" zoomable="yes"}

>[!INFO]
>
>U kunt geen labels bewerken die worden gedetecteerd en automatisch worden toegepast.

## Kenmerkprestaties

Metrische gegevens over inzichten kunnen u helpen te evalueren welke kenmerken de klant inspireren tot meer betrokkenheid.

In de volgende tabel vindt u definities en inzichten voor de belangrijkste maatstaven voor digitale marketing in de tabelweergave van [!UICONTROL Attributes] . Elke metrisch omvat een korte definitie aangezien het op attributen betrekking heeft, hoe metrisch wordt berekend, en één of meerdere inzichten helpen zijn betekenis en effect op een advertentiecampagne begrijpen.

| Metrisch | Definitie | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attribute]** | De kenmerknaam. | U kunt de tabel sorteren door op de kolomkop voor een van de belangrijkste maateenheden te klikken. |
| **[!UICONTROL Category]** | De [ categorie ](#categories) die de inherente kwaliteit van een attribuut vertegenwoordigt. |  |
| **[!UICONTROL # of images]** | Het aantal afbeeldingen met dit kenmerk. | De telling in de lijst van Attributen kan verschillend zijn dan de telling in de de detailmening van Attributen. Deze discrepantie kan optreden als de kanaalbron, zoals Meta, en GenStudio enigszins verschillende samenvattingsberekeningen gebruiken. |
| **[!UICONTROL # of videos]** | Het aantal video&#39;s met dit kenmerk. | De telling in de lijst van Attributen kan verschillend zijn dan de telling in de de detailmening van Attributen. Deze discrepantie kan optreden als de kanaalbron, zoals Meta, en GenStudio enigszins verschillende samenvattingsberekeningen gebruiken. |
| **[!UICONTROL Impressions]** | Een telling van elke keer dat een afbeelding of video&#39;s met dit kenmerk in het kanaal worden geladen, ongeacht interactie of weergave. | Een hoog aantal impressies kan wijzen op brede zichtbaarheid, maar voor echte prestaties, insight, moet u dit in verhouding tot andere betrokkenheidsmetriek overwegen. |
| **[!UICONTROL Clicks]** | Het aantal keren dat gebruikers met een afbeelding of video communiceren met dit kenmerk. | Een hoge kliktelling wijst op sterke interesse en betrokkenheid met de inhoud, die efficiënt kan zijn en het juiste publiek bereikt. |
| **[!UICONTROL CTR]**<br>_klik-door tarief _ | Percentage (%) van de indrukkingen dat heeft geresulteerd in klikken op afbeeldingen of video&#39;s met dit kenmerk.<br>**Berekening**: `clicks` verdeeld door `impressions` | Een hoog klikthrough tarief wijst erop dat de inhoud hoogst relevant en motiverend voor het publiek in het overseinen en ontwerp is, en effectief gericht op de belangen van het publiek. |
| **[!UICONTROL CPM]**<br>_Kosten per duizend _ | Kosten voor elke duizend beelden van een beeld of video met dit attribuut.<br>**Berekening**: totaal bedrag `spent` verdeeld door bereik, dan vermenigvuldigd door 1000 | Een lage waarde kan op rendabele zichtbaarheid wijzen, vooral wanneer gecombineerd met een hoge doorkliksnelheid. |
| **[!UICONTROL CPA]**<br>_Kosten per Actie _ | Gemiddelde kosten die worden uitgegeven om een specifieke klantenactie, zoals een aankoop of een abonnement te bereiken.<br>**Berekening**: totaal bedrag `spent` gedeeld door het aantal voltooide klantenacties | Helpt om attributen te identificeren die in waardevolle klantenacties resulteren. |
| **[!UICONTROL CPC]**<br>_Kosten per klik _ | Gemiddelde kosten voor elke klik op afbeeldingen of video&#39;s met dit kenmerk.<br>**Berekening**: totaal bedrag `spent` gedeeld door `clicks` | Lagere gemiddelde kosten kunnen duiden op kostenefficiënte en bestedingen, vooral in vergelijking met een stijging van de omzettingen. |
| **[!UICONTROL Spend]** | Het uit de begroting uitgegeven bedrag heeft betrekking op kenmerken gedurende een bepaalde periode. | Een hoog bestedingsbedrag in een korte periode kan wijzen op snel gebruik, wat tot een vroegtijdige uitputting van de middelen zou kunnen leiden. Houd het uitgegeven bedrag tegen zeer belangrijke prestatiesmetriek bij helpen het algemene rendement op investering controleren. |
