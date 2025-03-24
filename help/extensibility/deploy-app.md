---
title: Uw App Builder-app implementeren
description: Implementeer uw App Builder-app, of invoegtoepassing, voor GenStudio for Performance Marketing.
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
source-git-commit: 52e8e078bc013fe686b5cc2105089f7098cce575
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Uw app implementeren

Het uitvoeren van uw app biedt een voorlopige momentopname van uw gedrag van de invoegtoepassing voordat u deze implementeert. Deze informatie kan het zuiveren vergemakkelijken. U kunt het samenstellen en implementeren van een geïmplementeerde app forceren zonder deze opnieuw ter goedkeuring in te dienen.


**om app** in werking te stellen:

Voer de app uit in `https://localhost:9080` :

```bash
aio app run
```

**om app** op te stellen:

1. Navigeer naar uw implementatiewerkruimte. Als u bijvoorbeeld naar de werkruimte Productie wilt navigeren:

   ```bash
   aio app use -w Production
   ```

1. Implementeer de app:

   ```bash
   aio app deploy
   ```

**om re-plaatsing** te dwingen:

>[!NOTE]
>
>Door het forceren van build en implementatie wordt uw bestaande implementatie overschreven. Test uw toepassing eerst grondig in een testomgeving.

```bash
aio app build --force-build
```

```bash
aio app deploy --force-deploy
```

**om tezelfdertijd te bouwen en op te stellen**:

```bash
aio app deploy --force-build --force-deploy
```

**om app** te bekijken:

Na de implementatie kunt u de app in GenStudio for Performance Marketing weergeven door een parameter `query` aan de GenStudio for Performance Marketing-URL toe te voegen:

`https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create`

Als u tevreden bent met de invoegtoepassing, kunt u deze zonder de parameter `query` verspreiden.

U kunt nu [ uw app ](distribute-app.md) verspreiden.
