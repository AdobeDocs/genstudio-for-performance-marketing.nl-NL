---
title: Adobe GenStudio for Performance Marketing-gebruikersrollen en -machtigingen
description: Meer informatie over GenStudio for Performance Marketing-gebruikersrollen en -machtigingen.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: 3e9a2a4f42ba79389691705c571bf6bbd0b990c5
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Gebruikersrollen en -machtigingen

Voor het maken en implementeren van moderne marketingcampagnes is samenwerking tussen belanghebbenden met verschillende verantwoordelijkheden en vaardigheden vereist. _de rollen van de Gebruiker_ controleren toegang tot vele mogelijkheden van GenStudio for Performance Marketing. Uw toegewezen gebruikersrol bepaalt de taken die u kunt uitvoeren gebruikend dit platform. Een beheerder van het systeem van de Adobe wijst u aan een rol in het het productprofiel van GenStudio in Adobe Admin Console toe. Uw welkomstbericht geeft de rol aan die u hebt toegewezen.

>[!NOTE]
>
>Alvorens om het even welke gebruikers provisioned in deze rollen zijn, moet een systeembeheerder van het systeem van de Adobe in Adobe Admin Console worden aangewezen om eenmalige opstellingstaken uit te voeren. Deze rol van beheerder van de Adobe werkt alleen in het kader van de Adobe Admin Console. Het speelt geen rol in de interface van het GenStudio for Performance Marketing-platform. Een beheerder van een Adobe-systeem die rechten van systeembeheerders nodig heeft, moet zichzelf als GenStudio-systeembeheerder in de Adobe Admin Console aanbieden. Zie [ Voorziening GenStudio for Performance Marketing ](product-provisioning.md).

## Rechten

_verlenen de toestemmingen van de Entitlements_ toestemming om specifieke taken uit te voeren en tot beschermde middelen toegang te hebben. Rechten worden gedefinieerd in de gebruikersrol binnen het productprofiel en gebruikers krijgen deze rechten wanneer ze aan die rol worden toegewezen.

## Gebruikersrollen

Drie typen GenStudio for Performance Marketing-gebruikersrollen ondersteunen deze verscheidenheid aan organisatorische rollen. De toestemmingen worden aangepast aan elk van deze gebruikerstypes en steunen de verantwoordelijkheden van elke gebruiker in de marketing organisatie. Deze drie gebruikersroltypes zijn:

* **de redacteurs van GenStudio** gebruiken de generatieve AI van GenStudio for Performance Marketing mogelijkheden om marketing campagneactiva tot stand te brengen, om inhoudsoverzicht en goedkeuring te verzoeken, en goedgekeurde ontwerpen van deze inhoud te publiceren. Alle GenStudio for Performance Marketing-gebruikers kunnen een element openen en gebruiken zodra de editor het heeft opgeslagen in [!DNL Content] .

* **de medewerkers van GenStudio** zijn de breedste waaier van de gebruikers van GenStudio for Performance Marketing. Medewerkers kunnen inhoud weergeven en goedkeuren en vormen een essentieel onderdeel van de workflow dat ervoor zorgt dat de inhoud die u genereert, voldoet aan de behoeften en standaarden van uw organisatie.

* **het systeemmanagers van GenStudio** hebben de breedste reeks toestemmingen binnen GenStudio for Performance Marketing. Systeembeheerders voeren de essentiële taak uit om de basisvereisten voor het maken en implementeren van campagnemiddelen vast te stellen. De managers van het systeem voeren deze gidsen door merk en organisatie-specifieke informatie zoals [ merkrichtlijnen ](./guidelines/overview.md) uit te uploaden. Systeembeheerders hebben toestemming om [!DNL Brands] te maken en te publiceren, maar hebben geen bevoegdheden voor gebruikersbeheer.

### GenStudio-editors

_Editors_, of inhoudsscheppers, hebben de kerntoestemmingen nodig om GenStudio for Performance Marketing [!DNL Brands], [!DNL Campaigns], en [!DNL Content] activa tot stand te brengen. Ze kunnen ook elementen die ze hebben gemaakt bewerken en verwijderen. GenStudio for Performance Marketing ondersteunt het snel maken van honderden stukken inhoud. Deze gebruikers kunnen inhoudsfragmenten of hele ervaringen genereren die afzonderlijke goedgekeurde inhoud ordenen om aan de behoeften van specifieke marketingcampagnes te voldoen.

De redacteurs staan met de generatieve technologieën van GenStudio for Performance Marketing in wisselwerking door _het veroorzaken_. De snelle lade in het canvas verstrekt hulpmiddelen om herinneringen in de context van een specifieke campagnerichtlijnen te plaatsen. Als gevolg hiervan is de kwaliteit en het succes van gegenereerde inhoud gedeeltelijk afhankelijk van de kwaliteit van de merkrichtlijnen die uw organisatie heeft geüpload en de specificiteit van uw vraag. Zie [ efficiënte herinneringen ](effective-prompts.md) schrijven.

In de volgende tabel worden de standaardmachtigingen voor editors weergegeven:

| Functie | Maken | Bijwerken | Verwijderen | Weergave |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | nee | nee | nee | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Create] | ja | ja | ja | ja |
| [!DNL Insights] | kan slechts en schakelaars vormen |    |     | ja |
| [!DNL Personas] | ja | ja* | ja* | ja |
| [!DNL Products] | ja | ja* | ja* | ja |
| [!DNL Reviews and approvals] | ja | ja | ja | ja |

Editors kunnen de gemaakte [!DNL Personas] en [!DNL Products] bewerken en verwijderen.

GenStudio-systeembeheerders kunnen editors toestemming geven om een [!DNL Brand] te bewerken en te verwijderen.

### GenStudio-medewerkers

_de Medewerkers_ kunnen activa in GenStudio for Performance Marketing bekijken maar creëren, uitgeven, of schrappen niet deze activa. Deelnemers zijn belanghebbenden die van essentieel belang zijn voor het welslagen van het beoordelings- en goedkeuringsproces voor inhoud, maar die geen inhoud hoeven te maken of rechtstreeks hoeven te bewerken. Juridische deskundigen en managers van creatieve personen zijn voorbeelden van potentiële medewerkers. Medewerkers van GenStudio for Performance Marketing hebben mogelijk toestemming om elementen in andere producten van het Creative Cloud te maken en weer te geven.

In de volgende tabel worden de standaardmachtigingen voor medewerkers weergegeven:

| Functie | Maken | Bijwerken | Verwijderen | Weergave |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | nee | nee | nee | ja |
| [!DNL Campaigns] | nee | nee | nee | ja |
| [!DNL Content] | nee | nee | nee | ja |
| [!DNL Create] | nee | nee | nee | ja |
| [!DNL Insights] | nee | nee | nee | ja |
| [!DNL Personas] | nee | nee | nee | ja |
| [!DNL Products] | nee | nee | nee | ja |
| [!DNL Reviews and approvals] | nee | nee | nee | ja |

### GenStudio-systeembeheerders

_het systeemmanagers van GenStudio_ hebben de krachtigste reeks toestemmingen binnen GenStudio for Performance Marketing. Systeembeheerders voeren de essentiële taak uit om de basisvereisten voor het maken en implementeren van campagnemiddelen vast te stellen. De managers van het systeem voeren deze gidsen door merk en organisatie-specifieke informatie zoals [ merkrichtlijnen ](./guidelines/overview.md) uit te uploaden. Systeembeheerders hebben toestemming om [!DNL Brands] te maken en te publiceren, maar hebben geen bevoegdheden voor gebruikersbeheer.

In de volgende tabel worden de standaardmachtigingen voor systeembeheer weergegeven:

| Functie | Maken | Bijwerken | Verwijderen | Weergave |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | ja | ja | ja | ja |
| [!DNL Campaigns] | ja | ja | ja | ja |
| [!DNL Content] | ja | ja | ja | ja |
| [!DNL Insights] | ja | ja | ja | ja |
| [!DNL Personas] | ja | ja | ja | ja |
| [!DNL Products] | ja | ja | ja | ja |
| [!DNL Reviews and approvals] | ja | ja | ja | ja |

Zie [ begonnen worden met Adobe GenStudio for Performance Marketing ](get-started.md) voor een overzicht van voorlopige opstellingstaken.
