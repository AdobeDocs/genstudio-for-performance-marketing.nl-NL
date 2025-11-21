---
title: Aanbevolen procedures voor sjablonen
description: Volg de beste praktijken wanneer het gebruiken van malplaatjes met Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: 71b46454fa6fe2037ea6b103c0dfeedad74b8919
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Aanbevolen procedures voor het gebruik van sjablonen

De malplaatjes verminderen beduidend de tijd en de inspanning die wordt vereist om nieuwe inhoud te produceren door een uitgangspunt te verstrekken dat pre-gevormde lay-outs en ontwerpelementen omvat.

Houd u aan de volgende aanbevelingen wanneer u sjablonen gebruikt met GenStudio for Performance Marketing:

1. Kennis over [ malplaatjeelementen ](#know-about-template-elements)
1. Vorm [ kanaalrichtlijnen ](#configure-channel-guidelines) voor efficiënte verpersoonlijking van inhoud
1. Ontwerp met [ toegankelijkheidsnormen ](accessibility-for-templates.md) voor een optimale ervaring
1. Volg [ kanaal-specifieke malplaatjerichtlijnen ](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Leer de grondbeginselen van malplaatjeelementen en procedures in [ Werk met Malplaatjes ](use-templates.md). En diep-duik in [ het aanpassen van een malplaatje ](customize-template.md) voor specifieke instructies in uw volgende campagne te gebruiken.

## De juiste sjabloonelementen gebruiken

Elk sjabloontype gebruikt verschillende elementen om een structuur te maken voor het maken van kanaalspecifieke inhoud. [ vertrouwt me met de delen van een malplaatje ](use-templates.md#template-elements) en omvat de beste elementen voor uw inhoud en malplaatjetype.

Wanneer u uw sjabloon aanpast, gebruikt u de veldnamen in plaats van deze elementen waar u GenStudio for Performance Marketing nodig hebt om inhoud te genereren.

Zie [ elementen van het Malplaatje ](use-templates.md#template-elements).

## Plaatsaanduidingstekst gebruiken in sjablonen

Plaatsaanduidingstekst kan helpen bij het definiëren van syntaxis of structuur voor inhoud die later in een sjabloon moet worden ingevuld door een gebruiker. Bijvoorbeeld {first_name} .{last_name}@email.etc. om een e-mailadres te definiëren. Enkele gangbare scheidingstekens zijn echter al gereserveerd voor andere betekenissen in GenStudio for Performance Marketing:

❌ &lt; > - Wordt gebruikt voor HTML-tags.
❌ {{ }}{{} - Wordt gebruikt voor Handlebar-expressies.

Gebruik enkele haakjes (recht of gekruld) om plaatsaanduidingstekst aan te geven om verwarring met bestaande labels te voorkomen.

✅ {first_name} - Tijdelijke aanduiding voor voornaam.

## Kanaalrichtlijnen configureren

Het definiëren van duidelijke kanaalrichtlijnen is van essentieel belang om ervoor te zorgen dat de gegenereerde inhoud aansluit bij de vereisten en doelstellingen van uw merk. Met kanaalrichtlijnen kunt u regels opgeven voor elementen zoals toon, lengte en stijl die in de sjabloon worden gebruikt. U kunt bijvoorbeeld een maximum aantal tekens instellen voor de hoofdtekst of een specifieke call-to-action-stijl vereisen. Door deze richtlijnen vooraf in te stellen, vermindert u de behoefte om gedetailleerde instructies in elke AI herinnering te schrijven, het proces van de inhoudgeneratie te stroomlijnen en consistentie over uw e-mails te verzekeren.

Het overzicht en bepaalt de 0} kanaalrichtlijnen van uw Merk [ voor alle zeer belangrijke gebieden in uw malplaatje. ](/help/user-guide/guidelines/brands.md#channel-guidelines) Als u geen richtlijnen bepaalt, dan worden de [ standaardkanaalrichtlijnen ](/help/user-guide/guidelines/brands.md#default-channel-guidelines) toegepast, die niet uw merkvereisten volledig kunnen weerspiegelen.

![ de specificaties van het Lichaam ](/help/assets/channel-email-body.png)

Leer hoe [ Merken, Producten, en de richtlijnen van Persona ](/help/user-guide/guidelines/overview.md) geproduceerde inhoud beïnvloeden en hoe te om hen voor uw marketing doelstellingen aan te passen.

## Afbeeldingen uploaden voor sjablonen

Afbeeldingen die in sjablonen worden gebruikt, moeten afkomstig zijn uit de opslagplaats voor inhoud en moeten correct worden geüpload om ervoor te zorgen dat de afbeelding correct wordt weergegeven.

Als een sjabloon een rand-tot-rand (volledig afloopgebied) afbeelding bevat, wordt de grootte van de geselecteerde afbeelding automatisch aangepast aan de volledige sjabloonafmetingen. Als de afbeelding echter niet overeenkomt met de hoogte-breedteverhouding van de sjabloon, wordt de afbeelding uitgesneden zodat deze binnen de sjabloonafmetingen past en wordt deze mogelijk niet naar behoren weergegeven.

Er is geen functie voor automatisch passend maken voor afbeeldingen die in sjablonen zijn opgenomen.

Om het uitsnijden van afbeeldingen te verhelpen, moeten gebruikers de hoogte-breedteverhouding definiëren van de afbeelding die in de sjabloon moet worden gebruikt wanneer deze naar de opslagplaats voor inhoud wordt geüpload. Bij het uploaden van een goedgekeurde sjabloon:

1. [ ga door het malplaatje te werk uploadt proces ](/help/user-guide/templates/use-templates.md#add-a-template) tot u de **[!UICONTROL Add details]** pagina bereikt.

2. Definieer de hoogte-breedteverhouding van de afbeelding die in de sjabloon in **[!UICONTROL Ad width (px)]** en **[!UICONTROL Ad height (px)]** moet worden gebruikt. Hiermee definieert u het afbeeldingsvenster voor het gedeelte van de sjabloon waarin de afbeelding wordt weergegeven.

3. In de **[!UICONTROL More details]** sectie, selecteer **[!UICONTROL Image size]** dropdown en kies _Gewas aan een vaste grootte_.
   ![ Uitgesneden aan een vaste grootte ](images/crop-to-fixed-size.png " Uitgesneden aan een vaste grootte "){width="80%"}

De grootte en hoogte-breedteverhouding van een afbeelding bepalen in een browser:

1. Controleer de afbeelding.
   - In Windows/Linux:
      - Druk op F12.
   - Op macOS:
      - Druk op Command + Option + I.

1. Houd de muisaanwijzer boven de afbeelding.

1. Noteer de hoogte-breedteverhouding. Hiermee definieert u de hoogte-breedteverhouding van de afbeelding in de sjabloon.

Wanneer deze details niet worden toegepast tijdens het uploaden, wordt aangenomen dat de afbeelding de volledige hoogte-breedteverhouding van de sjabloon is en worden afbeeldingen die niet overeenkomen met die hoogte-breedteverhouding uitgesneden.

![ Beeld bijgesneden in een vertoning en ](images/cropped-display.png " Beeld uitsnijdend "){width="60%"}

**❌Uitgesneden afbeelding in een weergave- en sjabloonweergave**

![ Beeld dat in een vertoning wordt getoond en ](images/full-fit.png " Beeld dat in vertoning wordt getoond en "){width="60%"}

**✅Afbeelding volledig weergegeven**

## Volg kanaalspecifieke sjabloonrichtlijnen

Wanneer het creëren van malplaatjes, zorg ervoor zij aan de specifieke vereisten van het voorgenomen kanaal voldoen. Bouw malplaatjes die de lay-out en visuele vereisten voor elk kanaal aanpassen. Er zijn algemene richtlijnen die op om het even welk malplaatje van toepassing zijn, zoals:

- Onbewerkte en responsieve HTML en inline CSS gebruiken
- Adobe- of Google-lettertypen gebruiken
- Gebruik **niet** JavaScript

{{note-css-effects}}

Zie verdere tips en beperkingen wanneer u met elk sjabloontype werkt voor optimale prestaties:

- [E-mails](/help/user-guide/templates/email-template.md)
- [Advertenties weergeven en banner maken](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Meta-advertenties](/help/user-guide/templates/meta-template.md)
