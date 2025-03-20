---
title: Gegevensbeheer
description: Leer over gegevensopname en opslag voor  [!DNL Insights]  in GenStudio for Performance Marketing.
feature: Reporting and Insights
level: Experienced
role: Admin
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
source-git-commit: 3448392bc3f1496dafdbed2995f40bdba9c91c31
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Gegevensbeheer

GenStudio for Performance Marketing gebruikt Adobe Experience Platform (AEP) voor het invoeren en opslaan van gegevens en metagegevens die [!DNL Insights] van kracht maken. AEP gebruikt _schema&#39;s_ om de gegevensstructuren en _datasets_ te bepalen voor het opslaan van en het beheren van gegevensinzamelingen.

## Gegevensverbindingen

GenStudio for Performance Marketing gebruikt Customer Journey Analytics (CJA) om meerdere gegevensbronnen samen te voegen door een verbinding met een of meer AEP-gegevenssets te maken. CJA gebruikt deze gegevensverbindingen om gegevensmeningen tot stand te brengen voor het analyseren van metriek met [!DNL Insights].

>[!BEGINSHADEBOX]

**Belangrijke informatie over gegevensverbindingen**

Als u een [ het systeembeheerder van Adobe ](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager) bent, kunt u toestemmingen hebben die toegang tot het zandbakbeheer van AEP en componenten van het gegevensmeersysteem toestaan die GenStudio for Performance Marketing steunen.

>[!WARNING]
>
>Als u de productiesandbox in AEP opnieuw instelt, worden alle gegevensverbindingen verwijderd en werkt [!DNL Insights] niet meer.

Wees voorzichtig en verwijder de volgende gegevensverbindingen die GenStudio for Performance Marketing nodig heeft om betrouwbaar te kunnen werken niet:

- AEP-gegevenssets voorafgegaan door `GS Insights`
- AEP-schema&#39;s, -klassen en -veldgroepen, voorafgegaan door `GS Insights`
- Aangepaste veldgroep `timestamp for metadata`
- AEP-verbindingen: gegevensstromen vooraf vastgelegd met `GS Insights`
- AEP Connections: GS Insights-account

Zie [ implicaties van de Schrapping ](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) in de _Customer Journey Analytics_ gids alvorens u om het even welke gegevenscomponenten in AEP schrapt.

>[!ENDSHADEBOX]

## Beleid voor gegevensbewaring

GenStudio for Performance Marketing bewaart kanaalgegevens gedurende 13 maanden. Dit bewaarbeleid omvat de zes maanden gegevens die tijdens de eerste verbinding worden ingevoerd, waardoor een uitgebreide historische gegevensanalyse en rapportage wordt gewaarborgd.

Zie [ Connect kanaal en rekening ](/help/user-guide/insights/connect-channel.md).
