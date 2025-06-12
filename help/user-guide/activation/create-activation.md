---
title: Workflow voor activering
description: Meer informatie over de activeringsworkflow voor advertenties.
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
source-git-commit: a36e9611cd0e7d70ddc79de7eb688300eeb8ac88
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Workflow voor activering

[!DNL Activate] ondersteunt de activering van advertenties in kanaalspecifieke indelingen, zoals een Meta- of Google Campagne Manager 360-advertentiervaring.

Een GenStudio for Performance Marketing-ervaring is een onderdeel van een marketingcampagne, zoals een advertentie, dat wordt voorbereid als advertentie voor een specifiek publiek op een betaald advertentiekanaal of e-mail. De ervaring met activering bestaat uit drie hoofdcomponenten:

* **activa van Media**: De activa van media zijn de beelden (GIFs, PNG, JPEG) inbegrepen in uw advertentie. Activering ondersteunt momenteel statische afbeeldingen.

  Als u een afbeeldingselement wilt selecteren voor uw advertentie, moet u de juiste hoogte-breedteverhouding kiezen. De hoogte-breedteverhoudingen bepalen de proportionele verhouding tussen de breedte en hoogte van een afbeelding en zijn van cruciaal belang voor de doeltreffendheid van plaatsingen. Betaalde mediakanalen geven zorgvuldig geldige hoogte-breedteverhoudingen op voor elke advertentie op hun platform. Wanneer u afbeeldingselementen aan de activering toevoegt, moet u de hoogte-breedteverhouding selecteren op basis van de laatste en aanvullende informatie. Bestandstypen zijn beperkt tot JPEG, PNG en GIF.

* **Tekst**: De tekst bestaat uit alle vormen van exemplaar die in uw advertentie, met inbegrip van koppen, lichaamstekst, en vraag-aan-actie elementen inbegrepen zijn.

* **Meta-gegevens**: Gebruiker-bepaalde attributen die u aan inhoud kunt toewijzen. Metagegevens verbeteren de prestatie-analyse, het filteren en bijhouden. De pagina is meestal niet zichtbaar voor gebruikers.

Als u een activering maakt, moet u elk van deze advertentiecomponenten verfijnen voor een specifieke kanaalplaatsing- en marketingcampagne. GenStudio for Performance Marketing ondersteunt het activeren van één ervaring op één betaalkanaal.

## Workflowfasen

Hoewel unieke plaatsingsvereisten elk betaald kanaal bepalen, delen alle en activeringen de zelfde stappen op hoog niveau. Het activeren van een ervaring voor elk betaalkanaal heeft drie kernfasen:

1. **verbind GenStudio for Performance Marketing met uw doelkanaal**. Een GenStudio-systeembeheerder moet verbinding maken met uw kanaalaccounts voordat u een ervaring kunt activeren.

1. **bereidt uw ervaring voor activering** voor. U kunt op twee manieren ervaringen voorbereiden voor activering:

   * Activeer een goedgekeurde ervaring met vooraf gedefinieerde instellingen rechtstreeks vanuit [!DNL Content] . Op deze gestroomlijnde manier kunt u een of meer ad-hocervaringen activeren op één kanaal. Nadat u een ervaring hebt geselecteerd in de galerie [!DNL Content] , kunt u geen elementen meer bewerken of toevoegen aan uw advertentie. Activeren vanuit [!DNL Content] is beschikbaar voor Campagne Manager 360 van Meta en Google.

   * U kunt uw advertentie samenstellen door visuele elementen te selecteren in [!DNL Content] , tekstelementen toe te voegen en hoogte-breedteverhoudingen te selecteren. Deze methode omvat meer stappen, maar biedt meer creatieve flexibiliteit. De voorbereiding omvat het selecteren van media activa in de aangewezen aspectverhouding voor uw specifieke plaatsing en het toewijzen van tekst aan vraag-aan-actie elementen en lichaamskopie. U kunt informatieve metagegevens toevoegen die gebruikers helpen bij het zoeken naar een ervaring na activering. Bij elke plaatsing van een ad-kanaal worden geldige hoogte-breedteverhoudingen opgegeven voor visuele elementen die in de plaatsing zijn opgenomen.

1. **Overzicht en publiceer uw ervaring aan het doelkanaal**. Gebruik het _paneel van de Voorproef_ tijdens ervaringsopstelling om uw keus van plaatsing en tekstelementen te beoordelen alvorens uw activering te voltooien. Uw laatste revisie vóór publicatie vindt plaats in de app voor advertentiebeheer van het doelkanaal. Nadat u bijvoorbeeld een Meta-advertentie-ervaring hebt geactiveerd in GenStudio for Performance Marketing, moet u zich aanmelden bij Meta Ads Manager, uw advertentie beoordelen en vervolgens de specifieke kenmerken ervan selecteren voordat u deze publiceert.

Zodra een advertentie live is met het doel betaalde mediakanaal, kan [!DNL Insights] de prestatiegegevens bijhouden en analyseren.

## Ondersteunde kanalen

Elk betaald mediakanaal heeft een unieke activeringsworkflow. Selecteer het betaalkanaal voor activeringsrichtlijnen:

* [ Manager 360 van de Campagne van Google ](activate-cm360-ad.md)
* [ LinkedIn ](activate-linkedin-ad.md)
* [ Meta ](activate-meta-ad.md)
