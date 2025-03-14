---
title: Sjablooncode-editor
description: Leer hoe u de sjablooncode-editor in GenStudio for Performance Marketing kunt gebruiken.
level: Intermediate
feature: Templates, Content
source-git-commit: 96ed2b3e1a1d854b35bdddb5aa694fdfec727e1a
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Sjablooncode-editor

De redacteur van de malplaatjecode wordt ontworpen om u te helpen uw malplaatje voor optimaal gebruik verifiëren en verfijnen wanneer het produceren van nieuwe ervaringen met GenStudio for Performance Marketing. De redacteur steunt de syntaxis van Handlebars, die placeholders binnen het malplaatje gebruikt om erop te wijzen waar GenStudio for Performance Marketing inhoud voor u zou moeten produceren.

>[!TIP]
>
>Alvorens uw malplaatjeHTML code in de [!DNL Content] __ mening van Malplaatjes te uploaden, bereidt uw malplaatje voor door inhoudsplaceholders op te nemen die in [ worden bepaald past malplaatjes ](customize-template.md) begeleiding aan.

## Gevonden velden controleren

Het deelvenster _[!UICONTROL Check detected fields]_bevat een lijst met velden die GenStudio for Performance Marketing herkent in uw sjabloon. Controleer de lijst en u kunt door de HTML-code bladeren om te kijken naar de vormgeving van de sjabloon.

![ de redacteursmening van de Code ](/help/assets/template-detected-fields.png " Controle ontdekte gebieden "){width="600" zoomable="yes"}

Als u merkt dat een veld ontbreekt in de lijst, zoekt u in de sjablooncode naar de locatie van het ontbrekende veld. Tussenvoegsel correcte placeholder gebruikend de syntaxis van Handlebars en a [ erkende gebiedsnaam ](/help/user-guide/content/customize-template.md#recognized-field-names). Gebruik het formulier Zoeken en vervangen, dat onder aan de code-editor wordt weergegeven, om te zoeken naar specifieke tekenreeksen in de code. (Windows `CTRL`+`F` of macOS `CMD`+`F`)

### Een correctie aanbrengen

Als uw sjabloon fouten bevat, ziet u mogelijk een `Template is invalid` -bericht met een korte uitleg van de uitgave. In het volgende voorbeeld geeft het bericht aan dat het veld `_image` niet voldoet aan de conventie voor veldnamen die in de sjabloon voor meerdere pods is vastgelegd. In het bericht wordt verder aangegeven dat u de veldnaam moet bijwerken met het juiste voorvoegsel. Zoek het veld `_image` in de code-editor van de sjabloon en werk de naam zoals aanbevolen bij.

![ Correct ongeldig malplaatje ](/help/assets/animation/template-code-editor.gif){width="600" zoomable="yes"}

Het deelvenster _[!UICONTROL Check detected fields]_wordt bijgewerkt met de wijzigingen die u hebt aangebracht. Zodra u wordt tevreden dat de gebieden correct en volledig zijn, klik **[!UICONTROL Next]**om [ verder te gaan uploadend uw malplaatje ](/help/user-guide/content/use-templates.md#add-a-template).
