---
title: Een App Builder-app maken
description: Begin met het ontwikkelen van een app, of Add-on, om GenStudio for Performance Marketing uit te breiden.
feature: Extensibility
exl-id: 4e757dd4-a02d-472c-bc13-6f27dffa48f2
source-git-commit: 04a4f6432c5db87489e39f9396a7782c86441695
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Een App Builder-app ontwikkelen

De ontwikkelaars die inheemse mogelijkheden van GenStudio for Performance Marketing uitbreiden gebruiken [ Adobe App Builder ](https://developer.adobe.com/app-builder/) om, hun verlengbare apps, of toe:voegen-ons tot stand te brengen voor te leggen en op te stellen.

>[!BEGINSHADEBOX]

**Eerste vereisten**:

* Node.js (versie 20.x of hoger)

* npm (verpakt met Node.js)

* Adobe Developer command-line interface (CLI). Voer de volgende handelingen uit om de toepassing met npm te installeren: `npm install -g @adobe/aio-cli`

>[!ENDSHADEBOX]

## Toepassingsstructuur

GenStudio for Performance Marketing-invoegtoepassingen zijn App Builder-apps en bevatten dezelfde basiscomponenten als andere App Builder-apps.

### Bestanden samenstellen en configureren

De belangrijkste componenten van App Builder-apps zijn onder andere deze build- en configuratiebestanden. Deze lijst is niet inclusief alle build- en configuratiebestanden.

* `README.md`: bevat algemene informatie over de app.

* TS-toepassingsbestanden:

   * `package.json`
   * `package-lock.json`
   * `eslint`
   * `tsconfig`
   * `jest test up`

* App Builder-configuratiebestanden:

   * `app.config.yaml`
   * `ext.config.yaml`: Het dossier van de configuratie voor toe:voegen-op.
   * `app.config.yaml`: configuratiebestand voor de invoegtoepassing (inclusief het definiëren van uw toepassing als een GenStudio for Performance Marketing-invoegtoepassing).
   * `.aio`
   * `.env`: wijs het `.env` -bestand niet toe aan het bronbesturingselement.

### Source-code

```
- src/
    - genstudiopem/
        - web-src/
            - src/
                - components/
                - utils/
                - Constants.ts
                - index.tsx
                - index.css
                - utils.ts
        - index.html
```

### Source-codecomponenten

* `ExtensionRegistration.tsx`: definieert de API&#39;s die nodig zijn voor de host-app (GenStudio for Performance Marketing) om de invoegtoepassing te laden en weer te geven.

* `App.tsx`: Hoofd-app-component die routering naar andere componenten definieert.

* `AdditionalContextDialog.tsx`: Dialoogcomponent voor het weergeven van extra contextinvoegtoepassingen.

* `RightPanel.tsx`: Dialoogcomponent voor een validatie-invoegtoepassing.

* `Helper` -componenten: Bevat `ClaimsChecker` .

## Een App Builder-app maken vanuit een bestaande app

U kunt een voorbeeld-app gebruiken om snel een add-on te maken.

**om een app van App Builder van bestaande app** tot stand te brengen:

1. Download een voorbeeld app van de [ 20&rbrace; Voorbeelden van GenStudio UIX ](https://github.com/adobe/genstudio-uix-examples) bewaarplaats.

1. Van de werkruimte van het Project van App Builder op [ Adobe Developer Console ](https://developer.adobe.com/console/), selecteer [!UICONTROL Download All] om de details van het Project te downloaden.

1. Open uw voorbeeld-app lokaal in de voorkeursomgeving voor geïntegreerde ontwikkeling (IDE).

1. Verifiëren met de Adobe Developer opdrachtregelinterface:

   ```bash
   aio login
   ```

1. Download uw JSON-bestand en maak vervolgens uw app:

   ```bash
   aio app use '/path/to/your/downloaded/app-builder/project/details/config.json'
   ```

## Aangepaste code toevoegen aan de invoegtoepassing

Definieer de invoegcode in `AdditionalContextDialog.tsx` - en `RightPanel.tsx` -bestanden. Deze twee dossiers bepalen pop-up verschijning en gedrag wanneer de gebruikers tot toe:voegen-op toegang hebben.

* `AdditionalContextDialog.tsx`: Bepaal deze component als u van plan bent om _te gebruiken voeg toe:voegen-aan Context_ toe. De gebruikers staan met deze component in wisselwerking wanneer het klikken op _toe:voegen-ons_ in de snelle lade in [!DNL Create].

* `RightPanel.tsx`: Bepaal deze component als u van plan bent om het _Juiste Comité_ toe:voegen-op (ervaringsbevestiging) te gebruiken. Gebruikers gebruiken deze component wanneer ze op de invoegtoepassing voor validatie in het rechterdeelvenster in een [!DNL Create] ervaringsconcept klikken.

## Aanbevolen procedures voor het ontwikkelen van apps

Door uw ontwikkelomgeving te onderhouden, kunt u fouten bij de ontwikkeling en implementatie van apps voorkomen:

* Als u een oudere versie van een voorbeeld-app gebruikt, moet u de afhankelijkheden upgraden door ze opnieuw te installeren:

  ```bash
  rm -rf node_modules package-lock.json && npm i
  ```

* Upgrade de GenStudio UIX SDK. Bevestig dat u de meest recente versie van [ GenStudio UIX SDK ](https://github.com/adobe/genstudio-uix-sdk) gebruikt. Verwijs naar de [ bewaarplaats van het Voorbeeld van GenStudio UIX ](https://github.com/adobe/genstudio-uix-examples) om te leren hoe te om de meest recente veranderingen van SDK te gebruiken.

Nu bent u klaar om [ uw app ](deploy-app.md) op te stellen
