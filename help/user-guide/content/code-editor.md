---
title: Sjablooncode-editor
description: Leer hoe u de sjablooncode-editor in GenStudio for Performance Marketing kunt gebruiken.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 3739a218ce67749d0038059e3504ab9a4df8f065
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 0%

---

# Sjablooncode-editor

De redacteur van de malplaatjecode wordt ontworpen om u te helpen uw malplaatje voor optimaal gebruik verifiëren en verfijnen wanneer het produceren van nieuwe ervaringen met GenStudio for Performance Marketing. De redacteur steunt de syntaxis van Handlebars, die placeholders binnen het malplaatje gebruikt om erop te wijzen waar GenStudio for Performance Marketing inhoud voor u zou moeten produceren.

>[!TIP]
>
>Alvorens uw malplaatjeHTML code in de [!DNL Content] __ mening van Malplaatjes te uploaden, bereidt uw malplaatje voor door inhoudsplaceholders op te nemen die in [ worden bepaald past malplaatjes ](customize-template.md) begeleiding aan.

## Gevonden velden controleren

Het deelvenster _[!UICONTROL Check detected fields]_&#x200B;bevat een lijst met velden die GenStudio for Performance Marketing herkent in uw sjabloon. Controleer de lijst en u kunt door de HTML-code bladeren om te kijken naar de vormgeving van de sjabloon.

![ de redacteursmening van de Code ](/help/assets/template-detected-fields.png " Controle ontdekte gebieden "){width="600" zoomable="yes"}

Als u merkt dat een veld ontbreekt in de lijst, zoekt u in de sjablooncode naar de locatie van het ontbrekende veld. Tussenvoegsel correcte placeholder gebruikend de syntaxis van Handlebars en a [ erkende gebiedsnaam ](/help/user-guide/content/customize-template.md#recognized-field-names). Gebruik het formulier Zoeken en vervangen, dat onder aan de code-editor wordt weergegeven, om te zoeken naar specifieke tekenreeksen in de code. (Windows `CTRL`+`F` of macOS `CMD`+`F`)

### Een correctie aanbrengen

Als uw sjabloon fouten bevat, ziet u mogelijk een `Template is invalid` -bericht met een korte uitleg van de uitgave. In het volgende voorbeeld geeft het bericht aan dat het veld `_image` niet voldoet aan de conventie voor veldnamen die in de sjabloon voor meerdere pods is vastgelegd. In het bericht wordt verder aangegeven dat u de veldnaam moet bijwerken met het juiste voorvoegsel. Zoek het veld `_image` in de code-editor van de sjabloon en werk de naam zoals aanbevolen bij.

![ Correct ongeldig malplaatje ](/help/assets/animation/template-code-editor.gif){width="600" zoomable="yes"}

Het deelvenster _[!UICONTROL Check detected fields]_&#x200B;wordt bijgewerkt met de wijzigingen die u hebt aangebracht. Zodra u wordt tevreden dat de gebieden correct en volledig zijn, klik **[!UICONTROL Next]**&#x200B;om [ verder te gaan uploadend uw malplaatje ](/help/user-guide/content/use-templates.md#add-a-template).

## Algemene sjabloonproblemen en oplossingen

| **Fout** | **Beschrijving** | **Oplossing** |
|-----------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| Parseren mislukt | De sjablooninhoud kan niet worden geparseerd als geldige handgrepen. | Controleer uw malplaatje voor de syntaxisfouten van HTML en Handlebars en verbeter hen om het geldige formatteren voor [ inhoudplaceholders ](/help/user-guide/content/customize-template.md#content-placeholders) te verzekeren. |
| Groep niet toegewezen | Een afbeeldingsveld in een e-mailsjabloon met meerdere groepen wordt niet aan een groep toegewezen. | Controleren op consistent gebruik van sectievoorvoegsels. Elke [ sectie ](/help/user-guide/content/customize-template.md#sections-or-groups) kan slechts één van elk gebiedstype gebruiken (`headline`, `body`, `image` `cta`). Wijs het veld `image` toe aan een geldige groep in de sjabloon. |
| Afbeelding ontbreekt | Een vereist afbeeldingsveld ontbreekt. | Er is precies één `image` -veld vereist voor bepaalde sjabloontypen, zoals een metagegevens-, weergave- of banneradvertentie. Voeg het vereiste `image` veld toe aan uw sjabloon. |
| Ongeldige enkele groep | De e-mailsjabloon bevat precies één groep, die ongeldig is. | Een basis e-mailmalplaatje bevat één enkele reeks malplaatjeelementen, die niet de groep het noemen overeenkomst zoals bepaald in [ Secties of groepen ](/help/user-guide/content/customize-template.md#sections-or-groups) vereisen. Pas de sjabloon aan zodat deze secties nul hebben door een naamgevingssyntaxis voor groepen te verwijderen. |
| Geen velden | De sjabloon bevat geen velden. | Voeg [ erkende gebiedsnamen ](/help/user-guide/content/customize-template.md#recognized-field-names) toe gebruikend de syntaxis Handlebars aan uw malplaatje waar u GenStudio for Performance Marketing nodig hebt om een bepaald type van inhoud te produceren. |
| Vereiste eigenschappen ontbreken | Enkele vereiste metagegevenseigenschappen ontbreken. | Elk sjabloontype heeft vereisten en beperkingen op basis van de kanaalrichtlijnen. Meta vereist bijvoorbeeld een hoogte-breedteverhouding en voor weergaveadvertenties zijn afmetingen nodig. [ volg kanaal-specifieke malplaatjerichtsnoeren ](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines). |
| Gereserveerde naam gebruikt | Er wordt een verboden of gereserveerde veldnaam gebruikt. | Bepaalde [ gebiedsnamen ](/help/user-guide/content/customize-template.md#recognized-field-names), zoals `subject` of `introductory_text`, zijn gereserveerd. Wijzig de naam van velden die gereserveerde of niet-toegestane namen gebruiken. |
| Te veel velden | Het aantal velden is groter dan de globale limiet van 20. | Verwijder onnodige velden om ervoor te zorgen dat het totaal niet groter is dan 20. |
| Te veel groepen | Het aantal groepen overschrijdt het toegestane maximum van het kanaal. | Meta-, display- en LinkedIn-sjablonen staan geen meerdere secties toe. Voor e-mail is groepsnaamgeving vereist wanneer u twee of drie secties definieert. Verminder het aantal groepen in uw malplaatje om aan de [ vereisten van het kanaal ](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) te voldoen. |
| Niet-ondersteund veld | De sjabloon gebruikt een veld dat het kanaal niet ondersteunt. | Vervang of verwijder niet gestaafde gebieden volgens de [ erkende gebiedsnamen ](/help/user-guide/content/customize-template.md#recognized-field-names). |
