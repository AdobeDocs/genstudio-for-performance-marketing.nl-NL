---
title: Gegevensbeheer
description: Meer informatie over het opnemen en opslaan van gegevens voor Insights in GenStudio for Performance Marketing.
feature: Insights
level: Experienced
role: Admin
last-substantial-update: 2025-1-7
source-git-commit: 5dbe645f2ccf033f515da22ffdcce86edcb9fb24
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Gegevensbeheer

GenStudio for Performance Marketing gebruikt Adobe Experience Platform (AEP) voor gegevensinvoer en -opslag van de gegevens en metagegevens die [!DNL Insights] van kracht maken. AEP gebruikt _schema&#39;s_ om de gegevensstructuren en _datasets_ te bepalen voor het opslaan van en het beheren van gegevensinzamelingen.

## Gegevensverbindingen

GenStudio for Performance Marketing gebruikt Customer Journey Analytics (CJA) om veelvoudige gegevensbronnen te groeperen door een verbinding aan één of meerdere datasets van AEP te creëren. CJA gebruikt deze gegevensverbindingen om gegevensmeningen tot stand te brengen voor het analyseren van metriek met [!DNL Insights].

>[!BEGINSHADEBOX]

**Belangrijke informatie over gegevensverbindingen**

Als u een [ beheerder van het het systeemsysteem van de Adobe ](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager) bent, kunt u toestemmingen hebben die toegang tot het zandbakbeheer van AEP en componenten van het gegevensmeersysteem verlenen die GenStudio for Performance Marketing steunen.

>[!WARNING]
>
>Als u de productiesandbox opnieuw instelt in AEP, worden alle gegevensverbindingen verwijderd en werkt [!DNL Insights] niet meer.

Wees voorzichtig en verwijder de volgende gegevensverbindingen die GenStudio for Performance Marketing nodig heeft om betrouwbaar te kunnen werken niet:

- AEP-gegevenssets voorafgegaan door `GS Insights`
- AEP-schema&#39;s, -klassen en -veldgroepen, voorafgegaan door `GS Insights`
- Aangepaste veldgroep `timestamp for metadata`
- AEP-verbindingen: gegevensstromen vooraf vastgelegd met `GS Insights`
- AEP-verbindingen: GS Insights-account

Zie [ implicaties van de Schrapping ](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) in de _Customer Journey Analytics_ gids alvorens u om het even welke gegevenscomponenten in AEP schrapt.

>[!ENDSHADEBOX]

## Beleid voor gegevensbewaring

GenStudio for Performance Marketing bewaart kanaalgegevens gedurende 13 maanden. Dit bewaarbeleid omvat de zes maanden gegevens die tijdens de eerste verbinding worden ingevoerd, waardoor een uitgebreide historische gegevensanalyse en rapportage wordt gewaarborgd.

Zie [ Connect kanaal en rekening ](/help/user-guide/insights/connect-channel.md).
