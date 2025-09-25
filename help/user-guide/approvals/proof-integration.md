---
title: Workfront Proof-integratie met revisie en goedkeuring
description: Workfront Proof-integratie met Adobe GenStudio for Performance Marketing.
feature: Content Review, Content Management
exl-id: 149db773-4787-4cfb-b29e-c49f13abf39a
source-git-commit: 47195c08f500e50a01db127c6badc461c10afaf9
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---

# Workfront Proof-integratie met GenStudio for Performance Marketing

De integratie met Workfront Proof verbetert de overzicht-en-goedkeuringslevenscyclus van GenStudio for Performance Marketing met geavanceerde eigenschappen, met inbegrip van goedkeuringsmalplaatjes, multi-stage werkschema&#39;s, en de capaciteit om proefversies [ te vergelijken ](https://experienceleague.adobe.com/nl/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs). Deze gestructureerde versie zorgt voor transparantie, verantwoordingsplicht en gestroomlijnde samenwerking gedurende de volledige levenscyclus van de inhoudsherziening.

>[!BEGINSHADEBOX]

**Eerste vereisten**:

Installeer de [ uitbreiding van de Kijker van het Web van Adobe Workfront ](https://experienceleague.adobe.com/nl/docs/workfront/using/review-and-approve-work/proofing/review-proofs-in-workfront/review-a-proof/review-proof-in-web-viewer-extension)

>[!ENDSHADEBOX]

Workfront Proof [!DNL Proofing Viewer] is een rijke werkruimte voor het weergeven, gebruiken en vergelijken van proefdrukken. Vanuit [!DNL Proofing Viewer] kunt u

* Verschillende versies van de inhoud vergelijken
* Opmerkingen en markeringen voor tekeningen toevoegen aan een proefdruk
* Het bewijs goedkeuren

[!DNL Proofing Viewer] wordt geladen wanneer u op de proef-URL klikt in uw goedkeuringsaanvraag per e-mail of in-product melding. De [!DNL Proofing Viewer] _Mijn nieuwe goedkeuring_ mening opent. In deze weergave kunt u inhoud reviseren en opmerkingen maken met de belangrijkste annotatiegereedschappen van [!DNL Proofing Viewer] .

Klik op [!DNL Proofing Viewer] om **[!UICONTROL Return to GenStudio]** af te sluiten.

## Genstudio for Performance Marketing en Workfront Proof: vergelijking van functies

In de onderstaande tabel worden de standaard GenStudio for Performance Marketing-functies voor beoordeling en goedkeuring vergeleken met de meer geavanceerde mogelijkheden die de integratie met Workfront Proof biedt.

| Functie        | GenStudio for Performance Marketing                                                                 | Workfront Proof                                                                 |
|-------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| **Ontwerp/proefdruk levenscyclus**        | Conceptinhoud verloopt na publicatie. | Goedkeuringsketens met meerdere fasen, op rollen gebaseerd, met tijdstempels, persistente logbestanden.<br> Alle versies blijven onbeperkt behouden. |
| **Commentaren**                | Opmerkingen zijn gekoppeld aan concept-id en worden na publicatie genegeerd.                                           | Blijvende opmerkingen en aantekeningen blijven behouden voor controle en naleving.     |
| **Versies**           | Concepten worden als unieke instanties behandeld.<br> geen zij-aan-zij vergelijking.                                      | Volledige versiecontrole met de hulpmiddelen van de zij-aan-zij en bedekking vergelijking.        |
| **Projectbeheer** | Basis campagnebeheer. | Volledig levenscyclusbeheer van de campagne, met inbegrip van aanpassing, malplaatjes, rapportering, en gedetailleerde controles. |

### Licenties en gebruikersrollen

In vergunningen wordt de reeks gebruikersrechten binnen een product aangegeven. Workfront Proof biedt meer licentietypen of gebruikersrollen dan GenStudio for Performance Marketing. [ overzicht van de rollen van het proef ](https://experienceleague.adobe.com/nl/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles) introduceert gebruikersrollen verbonden aan het overzicht-en-goedkeuringswerkschema van Workfront Proof.

| GenStudio for Performance Marketing-licentie       | Workfront-licentie                 | Beschrijving                                                                                                                                                      |
|---------------------------------------------------|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| GenStudio System Manager                          | Workfront-beheerder/Power-gebruiker | Volledige toegang tot GenStudio Performance Marketing-functies zoals merk, persoonlijk gebruik en productbeheer. Beheert workflows en instellingen. Maakt goedkeuringssjablonen. |
| Inhoudsmaker en -editor (licentie voor energiegebruikers)   | Proefmaker (standaardlicentie)  | Genereert en verzendt inhoudsconcepten. In de Proofing Viewer uploadt u elementen en initieert u proefdrukken. Vereist een Workfront Proof-licentie.                              |
| Revisor/fiatteur (Collaborator-licentie)        | Revisor/fiatteur                 | Deelneemt aan revisies in meerdere stadia, voegt opmerkingen toe en keurt of verwerpt inhoud.                                                                             |

Adobe-systeembeheerders beheren gebruikersinvoer en -rechten voor beide producten in de Adobe Admin Console.

>[!NOTE]
>
> Workfront Proof verstrekt [ extra gebruikersrollen ](https://experienceleague.adobe.com/nl/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles). Niet alle rollen zijn zichtbaar binnen de Marketing van Prestaties. Het systeem houdt echter wel rekening met alle rollen die in een Workfront Proof-sjabloon zijn ingesteld.

### Concepten en proefdrukken

Workfront [!DNL Proofing Viewer] breidt het basisproces voor beoordeling en goedkeuring van GenStudio for Performance Marketing uit met meer gestructureerde herbeoordeling- en goedkeuringsfuncties. Proofs die in deze integratie worden beoordeeld, zijn beperkt tot de indelingen die door GenStudio for Performance Marketing worden ondersteund.

### Versiebeheer

GenStudio for Performance Marketing ondersteunt geen goedkeuringssjablonen, maar Workfront Proof wel. Dankzij de mogelijkheden van de proefversiemogelijkheden is het proces voor het beoordelen en goedkeuren van GenStudio-inhoud aanzienlijk verbeterd. Elke voorlegging in het werkschema van het Bewijs wordt behandeld als afzonderlijke versie van het inhoudsontwerp of _proef_. Proefdrukken worden automatisch opgeslagen en kunnen naast elkaar worden vergeleken met vorige herhalingen. Belanghebbenden kunnen wijzigingen bijhouden, nauwkeurige feedback geven en de uitlijning gedurende de volledige beoordelingscyclus handhaven. Het bewijs bewaart een volledige geschiedenis van alle commentaren, besluiten, en versies, ondersteunend controlebereidheid en nalevingsvereisten. Elke versie steunt ook multi-stadium, op rol-gebaseerde goedkeuringswerkschema&#39;s, met elke actie-goedkeuring, verwerping, of commentaar-duidelijk geregistreerd en timestamped.

### Goedkeuringssjablonen

Workfront Proof-goedkeuringssjablonen bevatten vooraf opgemaakte stappen waarmee de workflow voor proefdrukgoedkeuring kan worden gestroomlijnd. Deze sjablonen bevatten geselecteerde revisoren en fiatteurs, proefrollen en deadlines, zodat consistentie en efficiëntie worden gegarandeerd. De makers van inhoud die een revisie starten, kunnen kiezen uit een set vooraf gedefinieerde sjablonen voor zowel enkelfasige als meerfasentalige goedkeuringswerkstromen.

In elk stadium van de werkstroomsjabloon worden de toegewezen controleurs geïdentificeerd. Alle statusupdates en opmerkingen uit de Workfront Proof-workflow zijn zichtbaar in de Proofing Viewer, wat de transparantie en de samenwerking ten goede komt.

Goedkeuringsmodellen ondersteunen meerfasentalige goedkeuringen, die de coördinatie van beoordelingen door verschillende groepen belanghebbenden ondersteunen.

### Opmerkingen

Revisoren kunnen rechtstreeks op specifieke delen van de proefdruk klikken om exacte, contextuele opmerkingen te behouden. Alle opmerkingen krijgen een tijdstempel en worden opgeslagen als onderdeel van de versiegeschiedenis van de proefdruk. De geschiedenis van opmerkingen is niet beschikbaar in GenStudio for Performance Marketing.

U kunt [ twee versies van een proef ](https://experienceleague.adobe.com/nl/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs) vergelijken om overzichtscommentaren en inhoud te evalueren.

## Meldingen en herinneringen

Revisoren en fiatteurs ontvangen e-mailmeldingen wanneer er een nieuwe proefversie beschikbaar is voor revisie of wanneer de status van een doorlopende revisie is gewijzigd.
[ de berichten en herinneringen van het Bewijs ](https://experienceleague.adobe.com/nl/docs/workfront/using/workfront-proof/proof-notifications-and-reminders/proof-notifications-and-reminders/proof-notifications-and-reminders) omvatten een gepersonaliseerde verbinding aan de proef, details over de proef en zijn vooruitgang door het goedkeuringsproces, en versioning informatie.
