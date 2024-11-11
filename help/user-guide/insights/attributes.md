---
title: Overzicht van kenmerken
description: Leer hoe u de prestaties van specifieke kenmerken in Adobe GenStudio for Performance Marketing kunt beoordelen.
feature: Insights, Attributes
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
source-git-commit: d6ea1a34a8679ae958fb184e40ad0673abbab0a4
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 0%

---

# Overzicht van kenmerken

In de weergave [!DNL Insights] _[!UICONTROL Attributes]_ziet u een lijst met kenmerken die worden gebruikt in advertentiecampagnes voor het geselecteerde kanaalaccount.

De tabel _[!UICONTROL Attributes]_wordt ingedeeld met de naam [!UICONTROL Attribute] . U kunt schakelen tussen de lijsttypen met de knop **[!UICONTROL Images]**en de knop **[!UICONTROL Video]**. Klik op het instellingenpictogram (cog) boven de rechterkant van de tabel om de weer te geven kolommen in en uit te schakelen.

Het filterpictogram (trechter) boven de linkerkant van de tabel opent het menu **[!UICONTROL Filter]** , waarin u de kenmerken in de tabel kunt selecteren in de [!UICONTROL Account] en [!UICONTROL Attribute category] om deze te filteren. In het volgende voorbeeld wordt een lijst met kenmerken in de categorie `Lighting Condition` getoond.

![ de filter en lijst van Attributen ](/help/assets/insights-attributes-filter.png){zoomable="yes"}

## Kenmerkdetails

Kenmerken helpen elementen te identificeren aan de hand van de inherente details, zoals kleur, compositie, visuele elementen en andere eigenschappen.

In de weergave met kenmerkdetails kunt u zien welke ervaringen het geselecteerde kenmerk gebruiken. De details omvatten totale kenmerkprestaties en een uitsplitsing van de prestatiesmetriek met betrekking tot elke ervaring.

![ de prestatiemetriek van Attributen ](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing detecteert bepaalde functies en past het juiste kenmerk toe op een element of ervaring als tag. Zie [ Categorieën ](#categories) om voorbeelden van deze markeringen te zien. Klik op het pictogram Instellingen (cog) boven de rechterkant van de tabel om de kolom **[!UICONTROL Attributes]** te selecteren om alle kenmerken weer te geven die aan een ervaring zijn gekoppeld.

## Categorieën

GenStudio for Performance Marketing herkent bepaalde functies van afbeeldingen, video&#39;s en tekst en past een functietag toe op het element. A _categorie_ is een reeks eigenschappen die een specifiek kenmerk delen. Bijvoorbeeld, heeft de _categorie van de beeldrichtlijn_ een `landscape`, `portrait`, of `square` waarde.

U kunt geen labels bewerken die worden gedetecteerd en automatisch worden toegepast.

Zie [ categorieën van Attributen ](/help/user-guide/insights/attribute-category.md) voor gedetailleerde lijsten van beeld, video, en teksteigenschappen.

## Kenmerkprestaties

Metrische gegevens over inzichten kunnen u helpen te evalueren welke kenmerken de klant inspireren tot meer betrokkenheid.

In de volgende tabel vindt u definities en inzichten voor de belangrijkste maatstaven voor digitale marketing in de tabelweergave van [!UICONTROL Attributes] . Elke metrisch omvat een korte definitie aangezien het op een activa betrekking heeft, hoe metrisch wordt berekend, en één of meerdere inzichten helpen zijn betekenis en effect op een advertentiecampagne begrijpen.

| Metrisch | Definitie | Inzicht |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attribute]** | De kenmerknaam. | U kunt de tabel sorteren door op de kolomkop voor een van de belangrijkste maateenheden te klikken. |
| **[!UICONTROL Category]** | De [ categorie ](#categories) die de inherente kwaliteit van een attribuut vertegenwoordigt. |  |
| **[!UICONTROL # of images]** | Een aantal afbeeldingen met dit kenmerk. |  |
| **[!UICONTROL # of videos]** | Een aantal video&#39;s met dit kenmerk. |  |
| **[!UICONTROL Impressions]** | Een telling van elke keer dat een afbeelding of video&#39;s met dit kenmerk in het kanaal worden geladen, ongeacht interactie of weergave. | Een hoog aantal impressies kan wijzen op brede zichtbaarheid, maar voor echt prestatieinzicht, denk aan andere betrokkenheidsmetriek. |
| **[!UICONTROL Clicks]** | Aantal keren dat gebruikers met een afbeelding of video werken met dit kenmerk. | Een hoge kliktelling wijst op sterke interesse en betrokkenheid met de inhoud, die efficiënt kan zijn en het juiste publiek bereikt. |
| **[!UICONTROL CTR]**<br>_klik-door tarief _ | Percentage (%) van de indrukkingen dat heeft geresulteerd in klikken op afbeeldingen of video&#39;s met dit kenmerk.<br>**Berekening**: `clicks` verdeeld door `impressions` | Een hoog klikthrough tarief wijst erop dat de inhoud hoogst relevant en motiverend voor het publiek in het overseinen en ontwerp is, en effectief gericht op de belangen van het publiek. |
| **[!UICONTROL CPM]**<br>_Kosten per duizend _ | Kosten voor elke duizend beelden van een beeld of video met dit attribuut.<br>**Berekening**: totaal bedrag `spent` verdeeld door bereik, dan vermenigvuldigd door 1000 | Een lage waarde kan op rendabele zichtbaarheid wijzen, vooral wanneer gecombineerd met een hoge doorkliksnelheid. |
| **[!UICONTROL CPA]**<br>_Kosten per Actie _ | Gemiddelde kosten die worden uitgegeven om een specifieke klantenactie, zoals een aankoop of een abonnement te bereiken.<br>**Berekening**: totaal bedrag `spent` gedeeld door het aantal voltooide klantenacties | Helpt om attributen te identificeren die in waardevolle klantenacties resulteren. |
| **[!UICONTROL CPC]**<br>_Kosten per klik _ | Gemiddelde kosten voor elke klik op afbeeldingen of video&#39;s met dit kenmerk.<br>**Berekening**: totaal bedrag `spent` gedeeld door `clicks` | Lagere gemiddelde kosten kunnen duiden op kostenefficiënte en bestedingen, vooral in vergelijking met een stijging van de omzettingen. |
| **[!UICONTROL Spend]** | Het uit de begroting uitgegeven bedrag heeft betrekking op kenmerken gedurende een bepaalde periode. | Een hoog bestedingsbedrag in een korte periode kan wijzen op snel gebruik, wat tot een vroegtijdige uitputting van de middelen zou kunnen leiden. Houd het uitgavenbedrag bij de belangrijkste prestatiemetriek om het algemene rendement op investering te helpen controleren. |
