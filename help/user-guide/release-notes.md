---
title: Opmerkingen bij de release van Adobe GenStudio for Performance Marketing
description: Meer informatie over de nieuwste functies en verbeteringen voor Adobe GenStudio voor prestatiemarketing.
recommendations: noDisplay
source-git-commit: b502e0a558cbc26c70d813938734a2f6f230dc8e
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 2%

---

# Opmerkingen bij de release van GenStudio for Performance Marketing

Deze release bevat informatie over de meest recente updates voor de GenStudio for Performance Marketing-toepassing.

## 2024 11 07 {#latest}

### Oplossingen

* _sparen lopend_ spinner wordt niet meer getoond wanneer een gebruiker **[!UICONTROL Upload New Image]** dan de verrichting annuleert alvorens te uploaden voltooit. <!-- GS-6780 -->

* De titels van de ervaring worden nu correct gecreeerd tijdens ervaring regeneration. <!-- GS-7006 -->

* Problemen met flikkerende schuifbalken tijdens het laden van concepten zijn opgelost. <!-- GS-5587 -->

* De `View documentation` verbinding in [!DNL Content] _voegt uw goedgekeurd malplaatje_ popup nu toe werkt zoals verwacht. <!-- GS-6881 -->

* Het verwijderen van een afbeelding uit de gereedschapslade tijdens een formaatwijziging leidt niet langer tot een fout. <!-- GS-7115 7009 -->

* Het selecteren van **[!UICONTROL Delete]** in het [!DNL Create] actiemenu (..) werkt nu zoals verwacht. <!-- GS-6871 -->

* Gebruikers kunnen nu alle interactieve elementen van Meta en sjablonen alleen met het toetsenbord besturen. <!-- GS-4066 -->

* Afbeeldingsafmetingen zijn toegevoegd uit sjabloonafbeeldingsvelden om advertentiesjablonen weer te geven. Aanvragen voor slim uitsnijden worden nu verzonden voor de werkelijke afmetingen van de afbeelding en niet voor de gehele sjabloon. <!-- GS-6926 -->

* De tekenreeks `Zoom to fit to screen` is gelokaliseerd in gegenereerde e-mail- en Meta-advertenties. <!-- GS-5063 -->

* De aanroeplade van [!DNL Create] wordt nu gesloten zoals verwacht wanneer een gebruiker weg klikt. <!-- GS-5254 -->

* Metaadvertenties die u exporteert, bevatten nu het geselecteerde aanroep-naar-actie-label zoals verwacht. <!-- GS-6504 -->

* De merkenscore wordt nu bijgewerkt en behouden zoals verwacht voor opnieuw gegenereerde ervaringen. <!-- GS-6535 -->

* HTML exporteren van Meta-advertenties en weergaveadvertenties bevat niet langer de elementen wrapper `div` en `chrome` . <!-- GS-7116 -->

* Problemen met het renderen van concepten via e-mail tijdens publicatie zijn nu opgelost. <!-- GS-6394 -->

* De knop Canvas **[!UICONTROL Brand]** wordt nu uitgeschakeld wanneer geen merkenscore wordt gegenereerd. <!-- GS-6429 -->

* De Facebook/Instagram-schakeloptie op de canvasactiebalk werkt nu de weergave bij zoals u had verwacht wanneer de `ReadOnly` Canvas-instelling is ingeschakeld. <!-- GS-7039 -->

#### Afbeeldingen opnieuw genereren

* Het wijzigen van het formaat van meerdere meta&#39;s en varianten werkt nu zoals verwacht. Eerder werden op het canvas geen geregenereerde varianten weergegeven, maar bleef het leeg. <!-- GS-7010 -->

* Fragmentregeneratie werkt nu zoals u had verwacht voor ervaringen met vergroten of verkleinen. <!-- GS-6836 -->

* Het opnieuw genereren van metagegevens en afbeeldingen nadat het formaat ervan is gewijzigd, leidt niet langer tot een fout. Eerder werden de metagegevens van het kanaal gewijzigd van `meta` in `facebook` wanneer u de grootte van afbeeldingen aanpast voordat u de afbeelding opnieuw genereerde. <!-- GS-7042 -->

## 2024 10 31

### Nieuwe functies

* Het zoekfilter **[!DNL Content]** ondersteunt nu zoeken op basis van kleurtag. <!-- GS-5501 -->

* Op het canvas van **[!DNL Create]** worden nu tekenaantallen voor e-mailfragmenten weergegeven. <!-- GS-5819 -->

### Oplossingen

* Ontbrekende schermlezerlabels zijn toegevoegd aan mobiele en desktopelementen `view` . <!-- GS-5624 4729 -->

* De onderwerpregel en tekstgebieden vóór de koptekst van de **[!DNL Create]** Canvas-e-mail zijn nu dynamisch van hoogte. <!-- GS-6258 -->

* Layoutproblemen met e-mailranden zijn opgelost. <!-- GS-6631 -->

* Toetsenbordfocus werkt nu zoals u had verwacht op de knop **[!DNL Content]** **[!UICONTROL Delete]** . Eerder kon deze knoop niet worden bereikt of door het toetsenbord in werking worden gesteld.  <!-- GS-4065 -->

## 2024.10.14 Algemene beschikbaarheidsrelease

Deze release introduceert Adobe GenStudio for Performance Marketing, een generatieve AI-toepassing die de planning, ontwikkeling en analyse van marketingcampagnes versnelt. Met GenStudio for Performance Marketing kunnen marketingteams on-brand- en multikanaalsinhoud voor advertenties, e-mails en campagnes maken en real-time inzichten bieden om de prestaties van inhoud te optimaliseren.

### Functies

De belangrijkste productfuncties zijn:

**[!DNL Create]** introduceert het canvas, dat een gestructureerde herinneringservaring biedt die inhoudsredacteurs toelaat om inhoud en varianten snel te produceren. Systeembeheerders trainen het product op volgens richtlijnen voor organisatiemerken. [!DNL Create] zorgt ervoor dat alle door AI gegenereerde inhoud aansluit bij uw richtlijnen voor merken (merken, klantspecifieke kenmerken en productbeschrijvingen) en de productie van merkconsistente marketinginhoud stroomlijnt.

**[!DNL Content]** slaat gekrulde, merkcompatibele, goedgekeurde middelen en ervaringen op. GenStudio for Performance Marketing-gebruikers kunnen eenvoudig goedgekeurde middelen zoeken, bewerken, opnieuw gebruiken en delen, waardoor het voor elke campagne minder nodig is om inhoud helemaal opnieuw te maken.

**[!DNL Reviews and Approvals]** stelt een framework in waarmee belanghebbenden gegenereerde varianten kunnen beoordelen en goedkeuren voordat ze worden opgeslagen in **[!DNL Content]** of geëxporteerd.

**[!DNL Campaigns]** organiseert en beheert marketingcampagnes, zodat de uitvoering en tracering worden gestroomlijnd. Medewerkers kunnen campagnes visualiseren, plannen en volgen om meerdere initiatieven effectief te beheren en tijdige levering te garanderen.

**[!DNL Insights]** biedt realtime evaluatie van de prestaties van inhoud, zodat marketeers hun strategieën kunnen optimaliseren en gegevensgestuurde beslissingen kunnen nemen.

GenStudio for Performance Marketing integreert met andere Adobe Experience Cloud-producten, waaronder Adobe Express en Adobe AEM Assets.

### Aanvullende informatie

Zie de volgende handige bronnen:

* [ de Gids van de Gebruiker van Adobe GenStudio for Performance Marketing ](https://experienceleague.adobe.com/en/docs/genstudio/user-guide/home)

* [ de Academie van de Adobe GenStudio ](genstudioacademy.md), online het leren platform van de Adobe voor het gebruiken van generatieve AI technologieën in het creatieve proces. [ Register voor de Academie van GenStudio ](http://adobe.ly/genstudioacademyregistration).
