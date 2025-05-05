---
title: Verbind met een  [!DNL AEM Assets Content Hub]  bewaarplaats
description: Leer hoe te om Adobe GenStudio for Performance Marketing met een Adobe Experience Manager (AEM) te verbinden  [!DNL Content Hub]  bewaarplaats en hefboomwerking bestaande goedgekeurde inhoud.
level: Experienced
role: Admin, Data Engineer
feature: Content Management
recommendations: noDisplay
exl-id: abb587fd-593c-4b9f-baad-993d92400d9b
source-git-commit: 85948ccd9b6d198a2064d95639f96a045ea61743
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Verbinding maken met een [!DNL AEM Assets Content Hub] -opslagplaats

Als u middelen hebt in Adobe Experience Manager (AEM), kunt u deze stappen volgen om ze toegankelijk te maken in GenStudio for Performance Marketing.

>[!BEGINSHADEBOX]

**Eerste vereisten**:

De volgende stappen vereisen administratieve toegang tot Admin Console en AEM Assets as a Cloud Service.

>[!ENDSHADEBOX]

## Stap 1: Inschakelen [!DNL AEM Assets Content Hub]

Volg **stel Content Hub** zelfbedieningsproces op om [!DNL Content Hub] voor uw bestaande AEM Assets in Cloud Manager toe te laten. Zie [ opstellen  [!DNL Content Hub] ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub) in de _AEM as a Cloud Service_ documentatie.

Nadat u [!DNL AEM Assets Content Hub] hebt ingeschakeld, hebt u een nieuwe instantie met het `contenthub` achtervoegsel [!DNL AEM Assets as a Cloud Service] op Admin Console.

>[!IMPORTANT]
>
>Beheerders moeten controleren of de [!DNL AEM Assets Content Hub] -opslagplaats zich binnen dezelfde organisatie bevindt als GenStudio for Performance Marketing.

## Stap 2: GenStudio-gebruikers aan boord

Voeg in [!DNL Admin Console] een GenStudio for Performance Marketing-gebruiker of -gebruikersgroep toe aan het productprofiel van [!DNL AEM Assets Content Hub] . Als een inhoudscontroleur geen toegang heeft tot dezelfde organisatie als de [!DNL AEM Assets Content Hub] -opslagplaats, kunnen deze problemen ondervinden bij het evalueren en goedkeuren van inhoud.

- [ Onboard  [!DNL Content Hub]  beheerder ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-administrator)
- [ Onboard  [!DNL Content Hub]  gebruikers ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-users)

## Stap 3: activa goedkeuren

Goedkeuren van elementen voor gebruik in [!DNL AEM Assets Content Hub] , zodat deze beschikbaar zijn in GenStudio for Performance Marketing.

Zie [ activa in Experience Manager ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/approve-assets) in de _AEM as a Cloud Service_ documentatie goedkeuren.

## Stap 4: Zichtbaarheid van middelen configureren

Controleer in de configuratieopties van _[!DNL AEM Assets Content Hub]_&#x200B;elke set configuratieopties voor filters, elementdetails, zoeken en brandmerken.

Zie [ Content Hub gebruikersinterface ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/configure-content-hub-ui-options) in de _AEM as a Cloud Service_ documentatie vormen.

## Stap 5: Controleer de verbinding

In GenStudio for Performance Marketing Content is de lijst _[!UICONTROL Location]_&#x200B;beschikbaar boven de galerie aan de rechterkant. De lijst is niet beschikbaar als u geen toegang hebt of als uw organisatie een [!DNL AEM Assets Content Hub] -opslagplaats niet heeft geïmplementeerd en aangesloten.

Zie [ plaats van Assets ](manage-assets.md#assets-location) om over de lijst van de Plaats en veranderende bewaarplaatsen te lezen.
