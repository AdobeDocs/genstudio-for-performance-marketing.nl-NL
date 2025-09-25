---
source-git-commit: 8ed1e6853c9f844c72431dc692b556ece9c215a8
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---
## Doel

Help AI-coderingsassistenten om kleine, veilige bewerkingen uit te voeren in het GenStudio for Performance Marketing-documentatierapport.

## Architectuur op hoog niveau (kort)- Dit repo is een documentatiesite die bestaat uit Markdown onder `help/` en gedeelde include-bestanden in `help/_includes/` en gekrulde afbeeldingen onder `help/_includes/assets/` .- Release-opmerkingen, gebruikershandleiding en inhoud voor uitbreidbaarheid live onder `help/` . Bij grote inhoudswijzigingen moeten de voorgrond en de bestaande kopstructuur behouden blijven.- De site wordt gebouwd met Jekyll en gehost op GitHub-pagina&#39;s. Het bouwstijlproces gebruikt standaardovereenkomsten van Jekyll met sommige douaneplug-ins.

## Projectspecifieke conventies- Cursorregels: Aangepaste automatisering en richtlijnen vinden plaats in `.cursor/rules/*.mdc` . Voorbeelden: `.cursor/rules/docs-lint.mdc` (lint process), `.cursor/rules/generate-release-notes.mdc` (release notes format). Volg deze voor geautomatiseerde taken.- Bestandsnamen en voorgrond:   - Voor opmerkingen bij de release is een specifieke voorgrond vereist (zie `.cursor/rules/generate-release-notes.mdc`).   - Gebruik kebab-case voor regelbestanden en `.mdc` -extensie.- Opmaakconventies: Docs gebruikt GitHub-gearomatiseerde Markering. De koppen volgen doorgaans het geval van een zin en korte alinea&#39;s. Voorkeur voor `*` opsommingstekens voor lijsten in releaseopmerkingen en `###` voor functiesecties.

## Richtlijnen voor documentatiestijl- Volg [ Microsoft die de Gids van de Stijl ](https://learn.microsoft.com/en-us/style-guide/) voor technische documentatie beste praktijken schrijft:   - Duidelijke, beknopte zinnen schrijven die zijn gericht op gebruikersacties   - Actieve stem en huidige spanning gebruiken   - Tekst onderverdelen in korte, scannbare blokken   - Houd warme, directe toon terwijl het handhaven van technische nauwkeurigheid- Markering maken:   - Zin als hoofdletter gebruiken voor koppen (alleen eerste woord met hoofdletter)   - Alinea&#39;s kort houden (2-3 zinnen) voor leesbaarheid   - Lege regels toevoegen voor en na koppen en lijsten   - Achtergronden gebruiken voor UI-elementen, bestandspaden en code   - Alternatieve tekst opnemen voor alle afbeeldingen   - Koppeling maken naar specifieke secties met behulp van beschrijvende tekst

## Veiligheidsvoorschriften voor bewerkingen (wat AI moet doen)- Voeg nooit jira-id&#39;s, interne koppelingen of verwijzingen naar openbare documenten toe. Zie `generate-release-notes.mdc` &quot;Issue Tracking&quot;.- Voorgrond-YAML behouden bij het bewerken van bestanden die deze bevatten. Veel sjablonen en releaseopmerkingen zijn afhankelijk van vaste sleutels (titel, beschrijving, rol, exl-id).- Voor lintcorrecties geeft u de voorkeur aan automatische, epidemische bewerkingen uit `.cursor/rules/docs-lint.mdc` (gebruik de laatste nieuwe regel om de volgspaties te verwijderen). Voorbeeldopdrachten die door mensen worden gebruikt:

```sh
sed -i '' 's/ $//' <file>
sed -i '' '$ { /^$/d; }' <file> && echo "" >> <file>
```

## Voorbeelden (wat moet worden gewijzigd en hoe)- Kleine correcties voor kopiëren: werk tekst bij in `help/` Markeringsbestanden, houd koppen en ankers intact.- Afbeeldingsupdates: verwijs naar afbeeldingen onder `help/_includes/assets/` . Verplaats of wijzig de naam van afbeeldingen niet zonder alle referenties bij te werken.

## Waar moet eerst worden gekeken?- `help/_includes/` — gedeelde fragmenten en afbeeldingen.- `.cursor/rules/` — Richtlijnen voor automatisering en uitlijning; gebruik deze als gezaghebbende regels voor opmaak en processen.- `markdownlint_custom.json` — lokale markdownlint overschrijft.- `.github/pull_request_template.md` — PR-verwachtingen.

## Wanneer vraagt u de mens- Als een verandering het lopen of wijzigen van op docker-Gebaseerde tooling vereist (de lintregel noemt Docker) of plaatshulpleidingen beïnvloedt.- Als een bestand verwijst naar een onbekende externe configuratie (bijvoorbeeld `markdownlint.json` ontbreekt) — vraag dan of u het bestand wilt maken of negeren.

## Minimale opdrachten voor mensen

```sh
# Install linter (if not present)
npm install -g markdownlint-cli

# Run lint locally using project config
markdownlint --config markdownlint_custom.json "help/**/*.md"

# Project lint via yarn (preferred if available in environment)
yarn lint
```

&#x200B;---
Desgewenst kunt u deze gegevens samenvoegen in `.github/copilot-instructions.md` in de reactie (of de tekst/lengte aanpassen). Wat moet ik wijzigen of toevoegen?
