---
title: Activering optimaliseren
description: Leer hoe u activeringen kunt optimaliseren voor betaalde advertentiekanalen van derden.
level: Intermediate
feature: Ad Activation, Workflow
exl-id: 5bc624c2-d064-4190-8761-ed05d0629d1f
source-git-commit: 8a5d15df7a347c4ee7767610fc9bb23fc7b71db4
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# Activering optimaliseren

Het activeren van een advertentie voor betaalde advertentiekanalen omvat twee belangrijke fasen:

* Uw ervaring voorbereiden voor activering

* Uw ervaring publiceren naar het daarvoor aangewezen betaalkanaal en managers

Door de beste werkwijzen te volgen bij het maken en activeren van uw advertentie, kunt u potentiële complicaties of fouten tijdens de levering aan doelkanalen minimaliseren.

## Aanbevolen procedures

Hier volgen enkele veelvoorkomende aanbevolen procedures en de fouten die deze kunnen voorkomen.

* **Gebruik geldig, volledige bestemmingsURLs**

  Ongeldige URL&#39;s kunnen fouten activeren. Voorbeeldfout: _de URL die u hebt ingevoerd, verwijst niet naar een website. Voer een geldige URL in en probeer het opnieuw. (100)_

* **zorg ervoor dat uw toepassing symbolische vervaldatum** correct behandelt

  Toepassingen moeten zo nodig nieuwe tokens aanvragen. Verifieer en verkrijg zo nodig een nieuw toegangstoken door opnieuw aan te melden of de sessie te vernieuwen. Voorbeeldfout: _Fout bij het valideren van toegangstoken: de sessie is ongeldig omdat de gebruiker zijn wachtwoord heeft gewijzigd of omdat Facebook de sessie om beveiligingsredenen heeft gewijzigd. (190)_

* **herzie uw geplaatste advertentie en zorg ervoor dat slechts één advertentie op elk ogenblik actief is**

  Als u meerdere metagegevenssets moet activeren, maakt u voor elke set een aparte Dynamische Creative-advertentiesets. Voorbeeldfout: _Dynamische Creative Ad Set staat maximaal één actieve advertentie toe. Gebruikers mogen niet meer dan één advertentie maken onder dezelfde dynamische Creative-advertentieset. (100)_

* **Gelijke het aantal toegepaste regels met het bedrag dat door het platform** wordt gespecificeerd

  Betaalde kanalen verwachten dat het aantal toegepaste regels overeenkomt met het opgegeven formaat.  Pas indien nodig het aantal regels aan zodat deze overeenkomen met de waarde die het platform opgeeft. Voorbeeldfout: _Ad AssetFeed heeft X doel(en) voor formaat: naam van formaat, maar precies X doel regel voor dit formaat wordt verwacht. (100)_

* **kies een vraag-aan-actie (CTA) die met uw ad vastgestelde doelstelling** compatibel is

  Call-to-actions die niet compatibel zijn met het doel in Dynamic Creative Ad Sets, veroorzaken een fout. Voorbeeldfout: _de vraag aan actietype X wordt niet gesteund voor doelstelling Y in Dynamische Creative Ad Reeks. (100)_

* **verzeker het doel en de reeks GLB steunt het aantal ad ervaringen**

  Bevestig de advertentielimiet van het doel en de advertentieset voor uw geactiveerde advertentie. Verwijder zo nodig overbodige of inactieve advertenties uit de advertentieset om binnen deze limiet te blijven. U kunt ook een nieuwe advertentieset maken om extra advertenties te activeren. Voorbeeldfout: _u hebt de campagne bereikt en hebt limieten voor advertenties per advertentieaccount ingesteld of toegevoegd. Elke advertentieset kan maximaal 50 advertenties bevatten. Dit zijn onder andere gepauzeerde/inactieve/uitgeschakelde advertenties. (100)_

* **zorg ervoor dat het platform uw geselecteerd type van CTA** steunt

  Bevestig dat uw ervaring een ondersteund CTA-type bevat. Voorbeeldfout: _(#100) Ongeldige aanroep naar actietype (100)_
