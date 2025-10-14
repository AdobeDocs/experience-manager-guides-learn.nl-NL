---
title: Toetsen
description: Met toetsen kunt u variabele informatie opnemen voor wanneer u met DITA werkt in AEM Guides
exl-id: cb64e094-fe6d-4a5e-8f0e-25ae58aaa2c6
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Toetsen

Verschillende materiaalsets kunnen vergelijkbare informatie bevatten die op bepaalde plaatsen moet worden aangepast. De sleutels staan u toe om veranderlijke informatie aan te omvatten wanneer het werken met DITA.

De dossiers van de steekproef die u kunt verkiezen om voor deze les te gebruiken worden verstrekt in het dossier [&#x200B; keys.zip &#x200B;](assets/keys.zip).

>[!VIDEO](https://video.tv.adobe.com/v/342756?quality=12&learn=on)

## Toetsen inschakelen

1. Upload de set met beschikbare voorbeeldbestanden.

   a. Laad het ZIP-bestand.

   b. Vernieuw de AEM.

   c. Selecteer het bestand voor extractie.

   ![&#x200B; Uitgezochte Zip &#x200B;](images/lesson-9/select-zip.png)

   d. Klik [!UICONTROL **het Archief van het Extraheren**] in de hoogste toolbar.

   ![&#x200B; Toolbar &#x200B;](images/lesson-9/extract-archive.png)

   e. Kies in het dialoogvenster de specifieke locatie voor bestanden die u wilt uitpakken, zoals een map met de naam Toetsen.

   f. Klik [!UICONTROL **daarna**].

   g. Sla eventuele conflicten over omdat deze niet bestaan voor inhoud die nog niet eerder is geüpload.

   h. Selecteer [!UICONTROL **Extraheren**] bij het hoogste recht van het scherm.

1. Wanneer het extract volledig is, klik [!UICONTROL **gaan naar de doelomslag**].

   ![&#x200B; Bevestiging &#x200B;](images/lesson-9/go-to-target.png)

## Toetsen omzetten in waarden waarnaar wordt verwezen

Om sleutels correct te gebruiken, moet de Voorkeur van de Gebruiker een specifieke kaart als Kaart van de Wortel van verwijzingen voorzien. Binnen deze kaart is een inzameling van Sleutels, die samen binnen een topicgroep wordt gegroepeerd. Als u de kaart opent en de onderwerpen opent, worden de Toetsen omgezet in de waarden waarnaar deze kaart verwijst.

1. Geef een hoofdmap op.

   a. Open een kaart vanuit het scherm Toetsen.

   b. Gebruikersvoorkeuren configureren.

   c. Klik het [!UICONTROL **pictogram van de Voorkeur van de Gebruiker**] op de hoogste toolbar.

   ![&#x200B; Hoogste Toolbar &#x200B;](images/lesson-9/author-view.png)

   d. Klik het belangrijkste pictogram om a **Kaart van de Wortel** te specificeren die zal worden gebruikt om Sleutels op te lossen.

   e. Schakel de selectievakjes in voor elke gewenste Assets.

   ![&#x200B; Assets Dropdown &#x200B;](images/lesson-9/select-assets.png)

   f. Klik [!UICONTROL **Uitgezocht**].

   g. **sparen** de Voorkeur van de Gebruiker.

1. Navigeer aan de **Mening van de Kaart**.

1. Open de opgegeven kaart.

De sleutels worden opgelost.

## Handmatig een nieuw sleuteldef toevoegen

1. Open een kaart met een opgegeven hoofdmap.

1. Selecteer een toets.

   ![&#x200B; Zeer belangrijke Dropdown &#x200B;](images/lesson-9/hybrid-key.png)

1. Voeg een nieuw sleutelwoord in.

   a. Klik op een geldige locatie op de kaart.

   b. Selecteer het **Keydef** pictogram op de hoogste toolbar.

   ![&#x200B; Werkbalk Keydef &#x200B;](images/lesson-9/key-icon.png)

   c. Voer in het dialoogvenster Keydef invoegen een unieke waarde in voor Toetsen die voor de definitie die u maakt, zinnig is.

   d. Klik [!UICONTROL **Tussenvoegsel**].

1. Voeg topicmeta binnen keydef toe.

   a. Klik het [!UICONTROL **pictogram van het Element van het Tussenvoegsel**] op de hoogste toolbar.

   ![&#x200B; Werkbalk Keydef &#x200B;](images/lesson-9/add-icon.png)

   b. Zoek en selecteer &quot;topicmeta&quot; in het dialoogvenster Element invoegen.

1. Voeg sleutelwoorden binnen topicmeta toe.

   a. Klik het [!UICONTROL **pictogram van het Element van het Tussenvoegsel**] op de hoogste toolbar.

   ![&#x200B; Werkbalk Keydef &#x200B;](images/lesson-9/add-icon.png)

   b. Zoek in het dialoogvenster Element invoegen naar &quot;trefwoorden&quot; en selecteer deze.

1. Voeg een sleutelwoord binnen topicmeta toe.

   a. Klik het [!UICONTROL **pictogram van het Element van het Tussenvoegsel**] op de hoogste toolbar.

   ![&#x200B; Werkbalk Keydef &#x200B;](images/lesson-9/add-icon.png)

   b. In de **dialoog van het Element van het Tussenvoegsel**, onderzoek en selecteer &quot;sleutelwoord&quot;

1. Typ de waarde voor het trefwoord in het trefwoord.

Op de kaart zou uw keydef er nu ongeveer als volgt moeten uitzien:

![&#x200B; Keydef voltooide &#x200B;](images/lesson-9/keydef.png)

## Een sleuteldefinitie configureren als een fragment

Fragmenten zijn kleine inhoudsfragmenten die over verschillende onderwerpen in uw documentatieproject opnieuw kunnen worden gebruikt. In plaats van handmatig elk sleuteldef te genereren, kunt u één enkel sleuteldef configureren als een fragment.

1. Selecteer een keydef-element op de kaart.

1. In het contextuele menu, klik [!UICONTROL **Create Fragment**].

1. Voeg een titel en beschrijving toe in het dialoogvenster Nieuw fragment.
U kunt ook bestaande toetsen of trefwoorddefinities uit de inhoud verwijderen.

1. Klik [!UICONTROL **creëren**].

1. Voor het linkerpaneel, uitgezochte **Fragmenten**.

1. Sleep het fragment dat u zojuist hebt gemaakt van het deelvenster Fragmenten naar de kaart.

1. Werk het toetsontwerp zo nodig bij met de eigenschappen van de inhoud.
Wanneer bewaard en verfrist, zal deze reeks Sleutels voor om het even welke gebruiker beschikbaar zijn die een kaart heeft bepaald die de zelfde Kaart van de Wortel bevat.
