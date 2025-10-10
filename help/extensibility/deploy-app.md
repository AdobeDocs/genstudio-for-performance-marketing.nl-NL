---
title: App Builder-app implementeren
description: Implementeer uw App Builder-app, of invoegtoepassing, voor GenStudio for Performance Marketing.
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
source-git-commit: e783976dd035f64f5561a562471d4cc876162326
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# Uw app implementeren

Het uitvoeren van uw app biedt een voorlopige momentopname van het gedrag van uw Add-on alvorens het op te stellen. Dit kan helpen bij het opsporen van fouten.

## De app uitvoeren

Voer de app uit in `https://localhost:9080` :

```bash
aio app run
```

## De app implementeren

1. Navigeer naar uw implementatiewerkruimte:

   ```bash
   aio app use -w [deployment_workspace]
   ```

2. Implementeer de app:

   ```bash
   aio app deploy
   ```

## Nieuwe implementatie forceren

U kunt een build en implementatie van uw app forceren zonder deze opnieuw ter goedkeuring in te dienen.

>[!NOTE]
>
>Door een build en implementatie te forceren, wordt uw bestaande implementatie overschreven. **test eerst grondig uw app** in een testmilieu.

```bash
aio app build --force-build
```

```bash
aio app deploy --force-deploy
```

## Tezelfdertijd bouwen en implementeren

```bash
aio app deploy --force-build --force-deploy
```

## Uw nieuwe app zoeken

Na de implementatie kunt u de nieuwe app weergeven in GenStudio for Performance Marketing.

### Weergeven met een URL

Zie de nieuwe app door een parameter `query` aan de GenStudio for Performance Marketing-URL toe te voegen:

```txt
https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create
```

### Weergeven in de gebruikersinterface

De nieuwe uitbreidingen worden gevonden in verschillende plaatsen in UI, afhankelijk van het type van uitbreiding u opstelde. De momenteel beschikbare extensiepunten zijn:

* De uitbreiding van de naleving, die omvat:
   * [*snelle uitbreidingspunten*](#find-prompt-extensions), die klanten toestaan om extra context aan generatie toe te voegen LLM, en
   * [*de punten van de bevestigingsuitbreiding*](#find-validation-extensions), die klanten toestaan om de geproduceerde inhoud van LLM te bevestigen. Validatie wordt vaak gekoppeld aan de extensie Prompt om ervoor te zorgen dat inhoud die met een uitgebreide prompt wordt gegenereerd, wordt geklaagd met de vereisten van de klant (bijvoorbeeld claims met betrekking tot medische geneesmiddelen of wettelijk).
* [DAM-extensie (Digital Asset Management)](#find-dam-extensions)
* [Sjabloonextensie](#find-template-extensions)
* [Vertaalextensie](#find-translation-extensions)

### Snelle extensies zoeken

De snelle uitbreidingen worden gevonden in **toe:voegen-ons** dropdown, in de **parametersectie** van een malplaatje.

![&#x200B; Snelle uitbreidingen &#x200B;](./select-prompt-ext.png){width="600" zoomable="yes"}

Het dialoogvenster Add-on wordt geopend, zodat u de extra context kunt selecteren die u voor de LLM-generatie wilt toevoegen.

![&#x200B; Prompt extensie dropdown &#x200B;](./select-prompt-dropdown.png){width="600" zoomable="yes"}

### Validatie-extensies zoeken

De uitbreidingen van de bevestiging kunnen worden gevonden na een snelle generatie, in het juiste voorzitterschap dat met de resultaten wordt getoond.

![&#x200B; uitbreidingen van de Bevestiging &#x200B;](./validation-ext.png){width="600" zoomable="yes"}

Voer de extensie uit die u hebt geselecteerd om de gegenereerde inhoud te valideren.

![&#x200B; Geldige Bevestiging &#x200B;](./validation-valid.png){width="600" zoomable="yes"}

### DAM-extensies zoeken

De uitbreidingen van het Beheer van het Digitale Middel (DAM) worden gevonden wanneer het selecteren van inhoud in de **parametersectie** van een malplaatje. Zie de bodem van **Uitgezochte plaats** dropdown om het even welke toe:voegen-ons te zien.

![&#x200B; DAM uitbreidingen &#x200B;](./dam-ext.png){width="600" zoomable="yes"}

### Sjabloonextensies zoeken

De uitbreidingen van het malplaatje worden gevonden in het **Externe lusje van de Toepassing van het Malplaatje** wanneer het selecteren van een malplaatje. Dit tabblad wordt alleen weergegeven als er sjabloonapps zijn die moeten worden geselecteerd.

![&#x200B; uitbreidingen van het Malplaatje &#x200B;](./template-ext.png){width="600" zoomable="yes"}


### Vertaalextensies zoeken

Gebruik Extensiepunten voor vertaling om uw eigen vertaalservice via een proxy te gebruiken in plaats van de standaardvertaling van GenStudio.
Er is geen UI-locatie voor deze extensies.

Als de extensie is geregistreerd, wordt de aangeboden vertaaldienst gebruikt. Anders wordt de standaard GenStudio-vertaalservice gebruikt.



Als u tevreden bent met uw toe:voegen-op, bent u bereid om het zonder de `query` parameter te verdelen.

Nu, kunt u uw app [&#x200B; distribueren 0&rbrace;.](distribute-app.md)
