---
title: Spellingcontrole en zoeken/vervangen
description: Spellingcontrole gebruiken en zoeken/vervangen in AEM Guides
exl-id: 5f39618d-a919-4d3c-a4de-2896f2d1bf20
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# Spellingcontrole en Zoeken/vervangen

De AEM Guides Editor beschikt over krachtige mogelijkheden voor spellingcontrole en zoeken en vervangen.

>[!VIDEO](https://video.tv.adobe.com/v/342768?quality=12&learn=on)

Een spelfout corrigeren

1. Zoek een fout in een open onderwerp, weergegeven met een rode onderstreping.

1. Houd Ctrl ingedrukt en klik op de secundaire muisknop in het woord.

1. Kies de juiste spelling in de suggesties.

Als de juiste spelling niet wordt voorgesteld, kunt u het woord altijd handmatig bewerken.

## Overschakelen naar AEM spellingcontrole

U kunt een andere spellingcontrole dan het standaardwoordenboek van de browser gebruiken.

1. Navigeer aan **Montages van de Redacteur**.

1. Selecteer het **Algemene** montageslusje.

   ![ de Controle Config van de Spelling ](images/lesson-11/configure-dictionary.png)

1. Er zijn twee opties:

   - **Browser Controle van de Spel** — het gebrek dat waar de spellingcontrole het ingebouwde woordenboek van browser gebruikt.

   - **AEM de Controle van de Spel** — gebruik dit om een lijst van het douanewoord te bouwen gebruikend AEM douanewoordenboek.

1. Kies **AEM Controle van de Spelling**.

1. Klik [!UICONTROL **sparen**].

Een aangepast woordenboek configureren

De beheerder kan de instellingen wijzigen zodat het AEM woordenboek aangepaste woorden zoals bedrijfsnamen herkent.

1. Navigeer aan de **ruit van Hulpmiddelen**.

1. Login aan **CRXDE Lite**.

   ![ AEM UI CRXDE Lite pictogram ](images/lesson-11/crxde-lite.png)

1. Navigeer naar het knooppunt **_/apps/fmdita/config_** .

   ![ CRXDE Lite Knoop Config ](images/lesson-11/config-node.png)

1. Maak een nieuw bestand.

   a. Klik met de rechtermuisknop op de configuratiemap.

   b. Kies **creëren > Dossier** creëren.

   ![ Nieuwe Creatie van het Dossier van het Woordenboek ](images/lesson-11/new-dictionary-file.png)

   c. noem het dossier _&#x200B;**user_dictionary.txt**&#x200B;_.

   ![ tekst van het Woordenboek van de Gebruiker ](images/lesson-11/user-dictionary.png)

   d. Klik [!UICONTROL **OK**].

1. Open het bestand.

1. Voeg een lijst met woorden toe die u in het aangepaste woordenboek wilt opnemen.

1. Klik [!UICONTROL **sparen allen**].

1. Sluit het bestand.

Auteurs moeten mogelijk hun Web Editor-sessie opnieuw starten om de bijgewerkte lijst met aangepaste woorden in het AEM Woordenboek te krijgen.

## Zoeken en vervangen in één bestand

1. Klik op het pictogram Zoeken en vervangen op de bovenste werkbalk.

   ![ vind vervang Pictogram ](images/lesson-11/find-replace-icon.png)

1. Typ een woord of woordgroep in de onderste werkbalk.

1. Klik [!UICONTROL **Vondst**].

1. Typ zo nodig een woord om het gevonden woord te vervangen.

1. Klik [!UICONTROL **vervangen**].

## Zoeken en vervangen in de hele opslagplaats

1. Navigeer aan de **Bewaarplaats**.

1. Klik [!UICONTROL **Vondst en vervang**] pictogram bij de bodem verlaten van het scherm.

1. Klik het [!UICONTROL **toon het pictogram van Montages**].

1. Kies

   - **dossier van de Controle alvorens** te vervangen — als toegelaten door een Beheerder, zal het dossier automatisch worden gecontroleerd alvorens onderzoekstermijnen te vervangen.

   - **Hele woord slechts** - beperkt het onderzoek om slechts het nauwkeurige ingegane woord of de ingevoerde uitdrukking terug te keren.

   ![ vind Vervangen in Bewaarplaats ](images/lesson-11/repository-find-replace.png)

1. Klik [!UICONTROL **toepassen filter**] pictogram om de weg in Repository te selecteren waar u het onderzoek wilt uitvoeren.

1. Voer de voorwaarden in die u wilt zoeken en vervangen.

1. Indien vereist, uitgezochte **creeer nieuwe versie na vervang**.

1. Klik [!UICONTROL **Vondst**].

1. Open het gewenste bestand en gebruik de pijlen om van het ene gevonden resultaat naar het volgende te navigeren.

   ![ vind Vervangen Navigatie UI ](images/lesson-11/find-replace-navigation.png)
