---
title: App Builder-app implementeren
description: Implementeer uw App Builder-app, of invoegtoepassing, voor GenStudio for Performance Marketing.
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
source-git-commit: 7fdd3f54a0a031bfe26b48983de9cd24baad2f62
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Uw app implementeren

Het uitvoeren van uw app biedt een voorlopige momentopname van het gedrag van uw Add-on alvorens het op te stellen. Deze informatie kan het zuiveren vergemakkelijken.

**om app** in werking te stellen:

Voer de app uit in `https://localhost:9080` :

```bash
aio app run
```

**om app** op te stellen:

1. Navigeer naar uw implementatiewerkruimte:

   ```bash
   aio app use -w [deployment_workspace]
   ```

2. Implementeer de app:

   ```bash
   aio app deploy
   ```

**om re-plaatsing** te dwingen:

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

**om tezelfdertijd te bouwen en op te stellen**:

```bash
aio app deploy --force-build --force-deploy
```

**om app** te bekijken:

Na de implementatie kunt u de app in GenStudio for Performance Marketing weergeven door een parameter `query` aan de GenStudio for Performance Marketing-URL toe te voegen:

```txt
https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create
```

Als u tevreden bent met uw toe:voegen-op, bent u bereid om het zonder de `query` parameter te verdelen.

Nu, kunt u uw app [ distribueren 0}.](distribute-app.md)
