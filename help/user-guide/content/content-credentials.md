---
title: Content Credentials for Organisations
description: Meer informatie over het toepassen en beoordelen van Content Credentials in GenStudio for Performance Marketing.
level: Intermediate
feature: Content Management, Content Attributes
source-git-commit: b7e3d1c3b20149eee85670098ddd100b41e27f2c
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# Content Credentials voor organisaties

Leer hoe u de verificatiegegevens voor inhoud die de authenticiteit van het merk en de compatibiliteit van het station aantonen, rechtstreeks in uw marketingworkflow kunt insluiten.

>[!WARNING]
>
>Deze functie is momenteel in bèta beschikbaar voor organisaties die toegang hebben gekregen. Neem indien nodig contact op met uw Adobe-accountteamvertegenwoordiger voor deelname.


## Aan de slag met Content Credentials

Nadat Content Credentials in de Admin Console is geactiveerd, kunnen GenStudio for Performance Marketing-gebruikers Content Credentials inschakelen voor alle middelen in de app. Als de algemene optie voor het toepassen van referenties is uitgeschakeld, kunnen gebruikers Content Credentials toepassen op elk afzonderlijk element.

Als de inhoud eenmaal is gepubliceerd, is Content Credentials zichtbaar op externe platforms, zoals LinkedIn.

Beheerders zijn verantwoordelijk voor het uploaden van een geldig X.509-certificaat in de Admin Console. Deze stap zorgt ervoor dat de digitale handtekening van het bedrijf correct is geconfigureerd en klaar voor gebruik in ondersteunde Adobe DX-toepassingen.

>[!NOTE]
>
>De controle over deze instelling kan in de toekomst naar de Admin Console gaan, het beheer van Content Credentials in alle toepassingen stroomlijnen en het administratieve toezicht verbeteren.

## Wat is Content Credentials? 

Content Credentials is een duurzaam, industriestandaard type metagegevens met informatie over hoe inhoud is gemaakt en identiteitsgegevens over de makers. Content Credentials kan worden bekeken wanneer de inhoud online aan het steunen van platforms wordt gepubliceerd, of door hulpmiddelen zoals [ het hulpmiddel van de Inspectie van Adobe te gebruiken ](https://contentauthenticity.adobe.com/inspect) of de [ browser van Adobe Content Authenticity Chrome uitbreiding ](https://helpx.adobe.com/creative-cloud/help/cai/adobe-content-authenticity-chrome-browser-extension.html).  

Door Content Credentials toe te passen, kunt u de transparantie over de manier waarop inhoud is gemaakt, verhogen en kunt u gebruikers helpen zich aan te sluiten op hun inhoud.

[ leer meer over Content Credentials ](https://helpx.adobe.com/creative-cloud/help/content-credentials.html) bij Adobe.

## Handtekening merk en asset tracking

Inhoud met een merk speelt een belangrijke rol bij het bevorderen van de brandintegriteit en het vertrouwen van de gebruiker. Organisaties kunnen hun inhoud ondertekenen met een unieke merkhandtekening in Adobe-toepassingen wanneer hun certificaat correct is geconfigureerd in de Admin Console. Deze waarborg van authenticiteit blijft behouden met behulp van onzichtbare technologieën voor watermerken en vingerafdrukken, die de duurzaamheid van de handtekening gedurende de gehele levenscyclus van de inhoud helpen behouden.

Naast merkondertekening kunnen bedrijven id&#39;s van middelen rechtstreeks aan hun inhoud koppelen. Dit vergemakkelijkt het efficiënt volgen van activa, vooral wanneer zij worden gedeeld of op sociale media platforms worden geplaatst. Door middel van id&#39;s van bedrijfsmiddelen kunnen organisaties de herkomst en het verspreidingspad van hun inhoud traceren en het toezicht en de verantwoordingsplicht verbeteren.

## Content Credentials in de marketingworkflow

Het toepassen van Content Credentials kan tijdens de gehele marketingworkflow rechtstreeks in GenStudio for Performance Marketing worden uitgevoerd, van import en detectie van inhoud tot activering en export. U zult ook geloofsbrieven die op inhoud voor overzicht door app worden getoond vinden.

### Importeren en ontdekken

In de galerie Inhoud worden referenties weergegeven op geïmporteerde elementen.

Het Content Credential-symbool in de rechterbovenhoek van de miniatuur geeft &quot;Door merk ondertekende&quot; inhoud aan.

![ een ingevoerd middel met geloofsbrieven ](./images/import-discovery1.png){width="350"}

Als u ondertekende inhoud selecteert, worden de gedetailleerde metagegevens weergegeven: gepubliceerd merk, recorder, gebruikt gereedschap, tijdstempel.

Inhoud kan worden gefilterd op referentie.

![ Referentiegegevens over activa ](./images/import-discovery2.png)

### Maken en selecteren

Content Credential-badges worden weergegeven in de elementenkiezer Canvas.

Referentiemetagegevens blijven behouden omdat elementen zijn geselecteerd voor ervaringen om de herkomst tijdens het bewerken te behouden.

![ de badges van Content Credential in de de activaselecteur van het Canvas ](./images/creation-selection1.png)

### Bewerken en transformeren

Tijdens de export van een concept worden de gewijzigde activa automatisch opnieuw ondertekend en wordt de nieuwe referentie gekoppeld aan het origineel.

![ Referentiegegevens over een uitgevoerd element ](./images/edit-and-transformation1.png){width="300"}

### Herziening en goedkeuring

In de voorvertoning Beoordeling en Goedkeuren wordt de status van referentie weergegeven voor elementen op de rechterspoorstaaf.

![ Referentiegegevens over goedgekeurde activa ](./images/review-and-approve1.png){width="300"}

Gegevens per variant worden weergegeven als revisoren inspecteren de elementen. Goedgekeurde ervaringen worden opnieuw ondertekend wanneer gebruikers op **[!UICONTROL Save to Content]** klikken.

![ Referentiegegevens over goedgekeurde activa ](./images/review-and-approve2.png)

### Activeren en exporteren

Tijdens Activering wordt de status van de referentie weergegeven in de Experience-kiezer.

![ Referentiegegevens over een geactiveerd element ](./images/activate-export1.png){width="350"}

Geëxporteerde bestanden hebben C2PA-compatibele inloggegevens.

De integriteit van de referentie blijft behouden in alle ondersteunde indelingen (JPEG, PNG, MP4).

![ Referentiegegevens over een uitgevoerd element ](./images/activate-export2.png)

