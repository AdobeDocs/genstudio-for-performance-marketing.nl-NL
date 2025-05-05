---
title: Overzicht van media
description: Leer hoe u de mediaprestaties in Adobe GenStudio for Performance Marketing kunt evalueren.
level: Intermediate
feature: Reporting and Insights, Media Performance, Content Attributes
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
source-git-commit: 817a7bf425732cefd57da55e6bb41154567bca46
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 0%

---

# Overzicht van media

In de weergave [!DNL Insights] _[!UICONTROL Media]_&#x200B;ziet u een lijst met media die worden gebruikt in advertenties en advertentiecampagnes voor de geselecteerde account._ Media _vertegenwoordigt een beeld, een video, tekst, of andere creatieve inhoud die voor gebruik in uw marketing initiatieven wordt goedgekeurd.

{{connect-insights}}

De tabel _[!UICONTROL Media]_&#x200B;wordt ingedeeld met **[!UICONTROL Media ID]**. U kunt schakelen tussen de weergaven met behulp van het pictogram voor de weergavelijst (tabel) en het pictogram voor de galerieweergave (raster). Klik op het instellingenpictogram (cog) boven de rechterkant van de tabel om de weer te geven kolommen in en uit te schakelen.

![ de filter en lijst van Media ](/help/assets/insights-media-filter.png){zoomable="yes"}

In de galerieweergave van _[!UICONTROL Media]_&#x200B;ziet u een collage van voorvertoningen van media en een metrische waarde, zoals doorklikfrequentie. Klik op het pictogram Instellingen (cog) boven de rechterkant van de galerie om **[!UICONTROL Card settings]**&#x200B;te openen en een van de drie meeteenheden die u kunt bekijken in- en uit te schakelen:

- CPA (Kosten per actie)
- CTR (Klikdoorhalingsfrequentie)
- CPC (kosten per klik)
- Draaien

{{empty-table}}

## Media filteren

Met het filterpictogram (trechter) boven de linkerzijde wordt het menu **[!UICONTROL Filter]** geopend waarin u uit meerdere lijsten kunt kiezen. Selecteer **[!UICONTROL Clear all]** boven de tabel of galerie met advertenties om alle geselecteerde filters te verwijderen.

Met sommige filters kunt u exacte trefwoorden gebruiken om de lijst met criteria te verfijnen. Trefwoordfilters zijn vooral handig voor campagnes en advertenties die een complexe naamgevingsconventie volgen met meerdere unieke id&#39;s, zoals:

- Naam of code van specifiek gebied: `NA`, `EMEA`
- Inhoudstype acroniemen: `EB`, `CHT` of `DSP`
- Aanbiedingscodes of acroniemen: `OFFER2023`, `PROMO`

**aan filter door campagnes**:

1. Vouw het filter **[!UICONTROL Campaigns]** uit en klik op **[!UICONTROL Select]** .
1. Voer in het zoekveld trefwoorden in, gescheiden door komma&#39;s.

   Gebruik zoveel trefwoorden als u nodig hebt om de lijst te verfijnen:

   ![ Uitgezochte campagnes ](/help/assets/insights-select-campaign.png){width=400}

1. Selecteer een of meer campagnes in de resulterende zoekopdracht en klik op **[!UICONTROL Apply]** .

   De geselecteerde campagnes staan nu in de lijst _[!UICONTROL Filter by]_&#x200B;boven de advertentietabel of galerie, zodat u zich kunt concentreren op de media die aan de geselecteerde campagnes zijn gekoppeld.

1. _Facultatief_: Aan verdere filtermedia, voer een gelijkaardige sleutelwoordfilter op **[!UICONTROL Ads]** uit.

>[!NOTE]
>
>Het toegepaste filter blijft in alle weergaven in [!DNL Insights] bestaan. Selecteer **[!UICONTROL Clear all]** boven de tabel of galerie met advertenties om alle geselecteerde filters te verwijderen.

### Tabelresultaten downloaden

{{$include /help/_includes/download-insights.md}}

## Mediadetails

In de _mening van de Details van Media_, kunt u zien welke advertenties de geselecteerde media gebruiken. De details omvatten totale media prestaties, Advertenties die de media gebruiken, user-defined attributen, en AI-ontdekte eigenschappen verbonden aan de media.

![ Details van Media ](/help/assets/insights-media-details.png){zoomable="yes"}

### Mediakenmerken

{{$include /help/_includes/generated-attributes.md}}

## Mediaprestaties

Metrische gegevens over inzichten kunnen u helpen evalueren welke media bijdragen aan het succes van een campagne en welke mediakenmerken het meest effectief zijn.

In de volgende tabel vindt u definities en inzichten voor de belangrijkste maatstaven voor digitale marketing in de tabelweergave van [!UICONTROL Media] . Elke metrisch omvat een korte definitie aangezien het op media betrekking heeft, hoe metrisch wordt berekend, en één of meerdere inzichten helpen zijn betekenis en effect begrijpen.

| Metrisch | Definitie | Inzicht |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Media ID]** | De naam die is gekoppeld aan een afbeelding, video, tekst of andere creatieve inhoud. | U kunt de tabel sorteren door op de kolomkop voor een van de belangrijkste maateenheden te klikken. |
| **[!UICONTROL Impressions]** | Een telling van elke keer dat de media in het kanaal worden geladen, ongeacht interactie of weergave. | Een hoog aantal impressies kan wijzen op brede zichtbaarheid, maar voor echte prestaties, insight, moet u dit in verhouding tot andere betrokkenheidsmetriek overwegen. |
| **[!UICONTROL Clicks]** | Het aantal keren dat gebruikers communiceren met een klikbaar element, zoals een koppeling, op het medium. | Een hoge kliktelling wijst op sterke interesse en betrokkenheid met de inhoud, die efficiënt kan zijn en het juiste publiek bereikt. |
| **[!UICONTROL CTR]**<br>_klik-door tarief _ | Percentage (%) van de indrukken die hebben geleid tot het klikken van media binnen een advertentie.<br>**Berekening**: `clicks` verdeeld door `impressions` | Een hoge doorkliksnelheid geeft aan dat de media zeer relevant en aantrekkelijk zijn voor het publiek. Het stelt voor dat het overseinen en het ontwerp effectief de interesse van het publiek vangen en hen ertoe aanzetten om actie te ondernemen. Bovendien, kan een hoge CTR impliceren dat de media doelgericht is en met het voorgenomen publiek resoneert, die tot betere algemene campagneprestaties leiden. |
| **[!UICONTROL CPM]**<br>_Kosten per duizend _ | De gemiddelde kosten voor elke duizend media-indrukkingen.<br>**Berekening**: totaal bedrag `spent` gedeeld door het aantal beelden, dan vermenigvuldigd met 1000 | Een lage CPM-waarde kan de kosteneffectieve mediaprestaties aangeven, vooral wanneer deze zijn gecombineerd met een hoge doorkliksnelheid. |
| **[!UICONTROL CPA]**<br>_Kosten per Actie _ | Gemiddelde kosten die worden uitgegeven om een specifieke klantenactie, zoals een aankoop of een abonnement te bereiken.<br>**Berekening**: totaal bedrag `spent` gedeeld door het aantal voltooide klantenacties | Helpt om media te identificeren die in waardevolle klantenacties resulteren. |
| **[!UICONTROL CPC]**<br>_Kosten per klik _ | Gemiddelde kosten voor elke klik op het medium.<br>**Berekening**: totaal bedrag `spent` gedeeld door `clicks` | Lagere gemiddelde kosten kunnen duiden op kostenefficiënte en bestedingen, vooral in vergelijking met een stijging van de omzettingen. |
| **[!UICONTROL Spend]** | Het uit de begroting uitgegeven bedrag heeft betrekking op individuele media gedurende een bepaalde periode. | Een hoog bestedingsbedrag in een korte periode kan wijzen op snel gebruik, wat tot een vroegtijdige uitputting van de middelen zou kunnen leiden. Houd het uitgegeven bedrag tegen zeer belangrijke prestatiesmetriek bij helpen het algemene rendement op investering controleren. |
| **[!UICONTROL Used in these ads]** | Het aantal advertenties dat deze media gebruikt. | |
| **Attributen** | Lijst met inherente functies in deze media. | Kenmerken helpen u creatieve elementen te identificeren die het meest op uw publiek lijken. |
