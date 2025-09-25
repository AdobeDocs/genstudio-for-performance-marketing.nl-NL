---
title: Merkrechten configureren
description: Leer over het toewijzen van rechten voor de creators van GenStudio for Performance Marketing  [!DNL Brand]  en redacteurs.
level: Intermediate
feature: Brand Personalization, Generative AI
exl-id: fc33ecd3-4403-4045-87af-012a0377226c
source-git-commit: 72cd93d9d6fdd99d5a524d05cba923e9c0191960
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 1%

---

# [!DNL Brand] -machtigingen toewijzen

GenStudio-systeembeheerders kunnen standaard [!DNL Brands] maken en bewerken. De rollen van de inhoudeditor en van de medewerker hebben bewerkings- en aanmaakmachtigingen, maar vereisen mogelijk geen rechten voor systeembeheer.

Als u inhoudseditors en medewerkers deze [!DNL Brand] -gerelateerde machtigingen wilt verlenen, moet een Adobe-systeembeheerder enkele extra configuratietaken uitvoeren in de Adobe Admin Console. Zie [ Adobe Admin Console ](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview) in _de beleidsgids van de Onderneming en van Teams_.

Het toevoegen van gebruikers en gebruikersgroepen zijn basistaken gemeenschappelijk voor alle producten van Adobe met rechten die door Admin Console worden beheerd. Zie [ Adobe Admin Console gebruikers ](https://helpx.adobe.com/enterprise/using/users.html) in _de gids van de Onderneming en van het beleid van Teams_ voor een overzicht van gebruikersbeheer en procedures om gebruikers en gebruikersgroepen toe te voegen.

Bekijk deze video of volg de onderstaande stappen.

>[!VIDEO](https://video.tv.adobe.com/v/3474996?learn=on&enablevpops)

## Stap 1: Een gebruikersgroep maken

**om een gebruikersgroep** tot stand te brengen:

1. Meld u aan bij de Admin Console en navigeer naar **[!UICONTROL Users]** > **[!UICONTROL Users Groups]** .

1. Klik op **[!UICONTROL New User Group]**. _creeer een nieuwe gebruikersgroep_ popup opent.

1. Voeg een informatieve gebruikersnaam aan het veld **[!UICONTROL User group name]** toe om het doel van de nieuwe groep te identificeren. Bijvoorbeeld &#39;Merk managers&#39;.

1. Voeg desgewenst een beschrijving van de groep en het doel ervan toe.

1. Klik op **[!UICONTROL Save]**. Admin Console opent _Nieuwe groep_ popup, met de naam van de pas gecreëerde groep.

Zie [ gebruikersgroepen ](https://helpx.adobe.com/enterprise/using/user-groups.html) beheren in _de gids van de Onderneming en van het beleid van Teams_.

## Stap 2: Een GenStudio-systeembeheerprofiel toewijzen aan de gebruikersgroep

Zodra u een nieuwe gebruikersgroep en toegevoegde gebruikers hebt gecreeerd, kunt u het **profiel van de systeemmanager van Adobe GenStudio** aan deze groep toewijzen. De machtiging die aan het toegewezen profiel is gekoppeld, geeft alle gebruikers in deze groep de [!DNL Brands] -machtigingen (merk&#39;s maken, bijwerken en verwijderen).

**om een profiel aan de gebruikersgroep** toe te wijzen:

1. Navigeer aan de pas gecreëerde gebruikersgroep en klik _Toegewezen productprofielen_ tabel.

1. Van de _Toegewezen productprofielen_ tabel, klik **[!UICONTROL Assign profile]**. _wijst producten en profielen toe_ popup opent.

1. Selecteer `Adobe GenStudio` van de _Uitgezochte producten_ lijst.

1. Klik op **[!UICONTROL Apply]**. _Uitgezochte productprofielen_ popup opent, tonend de productprofielen verbonden aan Adobe GenStudio.

1. Selecteer `Adobe GenStudio system manager` .

1. Klik op **[!UICONTROL Apply]**. _wijst producten en profielen toe_ popup opent, tonend het productprofiel voor de pas gecreëerde gebruikersgroep.

1. Klik op **[!UICONTROL Save]**.

Zie [ Profielen van het Product toewijzen aan de Groepen van de Gebruiker ](https://helpx.adobe.com/enterprise/using/user-groups.html) in _de beleidsgids van de Onderneming en van Teams_.

## Stap 3: Gebruikers toevoegen aan de gebruikersgroep

Als u gebruikers de bevoegdheid wilt geven om [!DNL Brands] te maken, bewerken en publiceren, voegt u deze toe aan de nieuwe gebruikersgroep.

>[!NOTE]
>
>U moet minstens één gebruiker aan deze gebruikersgroep toevoegen alvorens de groep aan uw project toe te voegen.

**om gebruikers aan de gebruikersgroep** toe te voegen:

1. Van _Admin Console_, navigeer aan **[!UICONTROL Users]** > **[!UICONTROL User Groups]**.

1. Selecteer de naam van de gebruikersgroep die u eerder hebt gemaakt. _voegt gebruikers aan deze gebruikersgroep_ popup toe opent.

1. Voeg een nieuwe of bestaande gebruiker toe aan gebruikersnaam of e-mailadres. Wanneer u een naam of e-mailadres voor een bestaande gebruiker invoert, wordt dit veld automatisch gevuld met overeenkomende namen voor bekende gebruikers die tot deze IMS org behoren. Leer over het beheren van gebruikersgroepen in [ gebruikersgroepen ](https://helpx.adobe.com/enterprise/using/user-groups.html) in _de beleidsgids van de Onderneming en van Teams_ leiden.

Gebruikers krijgen de machtiging [!DNL Brand] om Adobe GenStudio-systeemmanagers te maken, bewerken en publiceren wanneer ze aan de groep worden toegevoegd. Gebruikers ontvangen ook een automatische e-mailuitnodiging om het Adobe GenStudio for Performance Marketing [!DNL Brands] -project te bewerken.

## Stap 4: Een [!DNL Brands] -project maken

A _project_ verstrekt een opslagplaats waar de uitgezochte gebruikers activa-in dit geval, [!DNL Brands] activa kunnen bewaren.

**om een [!DNL Brands] project van de _Opslag_ tabel** tot stand te brengen:

1. Navigeer aan het _lusje van de Opslag_ in Admin Console.

1. Klik op **[!UICONTROL Projects]** in de zijnavigatie. Het _lusje van Projecten_ opent.

1. Klik op **[!UICONTROL Create Project]**. Het _Nieuwe project_ popup opent.

1. Typ `Adobe GenStudio Brands` in het veld Projectnaam. Voer de naam van dit project precies zo in als hier wordt weergegeven. Neem geen extra spaties op en wijzig het lettertype.

1. Klik op **[!UICONTROL Create]**. _nodigt uit aan project_ popup opent.

Zie [ projecten ](https://helpx.adobe.com/enterprise/using/projects-in-business-storage.html) in de _gids van de Onderneming en van het beleid van Teams_ leiden.

## Stap 5: Gebruikersgroep uitnodigen om te project

U kunt nu de gebruikersgroep toevoegen die u net hebt gemaakt aan het `Adobe GenStudio [!DNL Brands]` -project.

**om de gebruikersgroep aan het onlangs gecreeerde project** uit te nodigen:

1. Van _Uitnodiging aan project_ popup, voeg de gebruikersgroep toe u enkel aan dit project creeerde.

1. Kies **** toestemmingenoptie kan uitgeven.

1. Klik op **[!UICONTROL Invite]**.
