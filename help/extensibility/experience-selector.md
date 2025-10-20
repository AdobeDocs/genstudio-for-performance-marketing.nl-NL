---
title: GenStudio Experience Selector MFE
description: Begrijp en implementeer de Experience Selector Micro FrontEnd voor uw GenStudio-apps en -invoegtoepassingen.
feature: Extensibility, Extensions, Experiences
source-git-commit: e30e43bd8d226628b425c341d19195f7f860e560
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# GenStudio Experience Selector MFE

Experience Selector is een MFE (Micro Front) die een `ExperienceSelectorDialog` -component biedt voor het selecteren van ervaringen met GenStudio. Gebruik de component in uw toepassing door de functie `renderExperienceSelectorWithSUSI` te importeren uit de zelfstandige JavaScript-bundel, die automatisch de meest recente geïmplementeerde Micro Frontend laadt en een natuurlijke componentinterface presenteert.

Met de GenStudio Experience Selector MFE kunnen gebruikers:

- Bladeren en GenStudio-ervaringen selecteren
- De ervaringen van de filter door diverse criteria
- Ondersteuning voor zowel enkelvoudige als meervoudige selectiemodi
- Verificatie verwerken via integratie met SUSI (Sign-Up)
- Verstrek verenigbare UI over verschillende kaders

## Integratieopties

De MFE kan op twee verschillende manieren worden geïntegreerd:

### ESM (ES-modules) - aanbevolen

```javascript
import { renderExperienceSelectorWithSUSI } from 'https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/esm/standalone.js';
```

### UMD (Universal Module Definition)

```html
<script src="https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/umd/standalone.js"></script>
```

## Configuratieeigenschappen

De functie `renderExperienceSelectorWithSUSI` accepteert een configuratieobject met de volgende eigenschappen:

| Eigenschap | Type | Vereist | Beschrijving |
|----------|------|----------|-------------|
| `apiKey` | string | Ja | API-sleutel voor GenStudio-services |
| `imsOrg` | string | Ja | IMS-organisatie-id |
| `env` | string | Ja | Omgeving (`stage`, `prod`) |
| `susiConfig` | object | Ja | [&#x200B; SUSI authentificatieconfiguratie &#x200B;](#susi-configuration) |
| `onSelectionConfirmed` | function | Ja | Callback wanneer de selectie wordt bevestigd |
| `onDismiss` | function | Ja | Callback wanneer de dialoog wordt gesloten |
| `locale` | string | Nee | Landinstelling (bijvoorbeeld `en-US`) |
| `isOpen` | boolean | Nee | Oorspronkelijke dialoogstatus |
| `selectionType` | string | Nee | De selectiemodus (`single` of `multiple`) |
| `customFilters` | array | Nee | Aangepaste filtercriteria |
| `dialogTitle` | string | Nee | Aangepaste dialoogtitel |

### SUSI-configuratie

Het object `susiConfig` kan het volgende bevatten:

```javascript
{
  clientId: 'genstudio',
  environment: 'stg1', // or 'prod'
  scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
  locale: 'en_US',
  modalSettings: {
    width: 500,
    height: 700
  }
}
```

## QuickStart

1. **kies uw kader** van de beschikbare hieronder voorbeelden
1. **navigeer aan de voorbeeldfolder**
1. **installeer gebiedsdelen** (voor Reactie/de voorbeelden van de Waarde)
1. **configuratie van de Update** met uw API sleutels en organisatie IMS:

   ```javascript
   const experienceSelectorProps = {
     locale: 'en-US',
     apiKey: 'exc_app',           
     imsOrg: 'your-ims-org@AdobeOrg',  // Replace with your IMS Org
     env: 'stage', // or 'prod'
     susiConfig: {
        clientId: 'genstudio',
        environment: 'stg1', // or 'prod'
        scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
        locale: 'en_US',
        modalSettings: {
          width: 500,
          height: 700,
        },
     },
     customFilters: ['genstudio-channel:email'],
     selectionType: 'single', // or 'multiple'
     dialogTitle: 'Select Email Templates'
   };
   ```

1. **stel de ontwikkelingsserver** in werking

### Voorbeeldimplementaties

Deze gegevensopslagruimte bevat werkvoorbeelden voor verschillende frameworks:

- [&#x200B; A **volledige toepassing van het Reageren** het demonstreren integratie met Vite bouwt systeem &#x200B;](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/react-js).

- [&#x200B; A **Vue 3 toepassing** met de integratie van compositie API &#x200B;](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vue-js).

- [&#x200B; Twee **Vanilla JavaScript implementaties** &#x200B;](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js):

   - [&#x200B; Deze **Vanilla ESM** versie gebruikt ES6 modules en moderne JavaScript &#x200B;](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-esm).

   - [&#x200B; Deze **Vanilla UMD** versie gebruikt de bundel van UMD die via manuscriptmarkering &#x200B;](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-umd-global-var) wordt geladen.

## Verificatiestroom

De Selecteur van de Ervaring behandelt authentificatie automatisch door SUSI:

1. Wanneer het dialoogvenster wordt geopend, wordt gecontroleerd op bestaande verificatie.
1. Als niet voor authentiek verklaard, opent het een SUSI login stroom.
1. Na succesvolle authentificatie, wordt de ervaringsselecteur getoond.
1. Gebruikers kunnen door ervaringen bladeren en deze selecteren.
1. Geselecteerde ervaringen worden geretourneerd via de callback van `onSelectionConfirmed` .
