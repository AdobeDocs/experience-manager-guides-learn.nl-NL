---
title: Mapprofielen
description: Maken en gebruiken van mapprofielen voor AEM Guides
exl-id: 5a0daa68-51ae-42d0-8320-6e8bdb1fe545
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 0%

---

# Mapprofielen

AEM biedt snelle toegang tot configuratiehulpmiddelen. Door de Profielen van de Omslag aan te passen, kunnen de verschillende afdelingen of de producten unieke malplaatjes, auteursmilieu&#39;s, voorwaardelijke attributenprofielen, Fragmenten, of zelfs de configuraties van de Redacteur van het Web hebben.

De dossiers van de steekproef die u kunt verkiezen om voor deze les te gebruiken worden verstrekt in het dossier [&#x200B; folderprofiles.zip &#x200B;](assets/folderprofiles.zip).

>[!VIDEO](https://video.tv.adobe.com/v/342758?quality=12&learn=on)

## Mapprofielen openen

Configuraties worden beheerd via het pictogram Mapprofielen.

1. Van het scherm van de Navigatie, klik het [!UICONTROL **pictogram van Hulpmiddelen**].

   ![&#x200B; Pictogram van Hulpmiddelen &#x200B;](images/reuse/tools-icon.png)

1. Selecteer **Gidsen** op het linkerpaneel.

1. Klik de **tegel van Profielen van de 1&rbrace; omslag 0&rbrace;.**

   ![&#x200B; Profielen van de Omslag &#x200B;](images/reuse/folder-profiles-tile.png)

1. Selecteer het gewenste profiel. Bijvoorbeeld, kies **Globaal Profiel**, dat het standaardprofiel is.

   ![&#x200B; Globaal Profiel &#x200B;](images/lesson-3/global-profile-tile.png)

## Voorwaardelijke kenmerken bewerken in het algemene profiel

Zodra u het Globale Profiel hebt betreden kunt u zijn configuratie uitgeven. De instellingen voor het algemene profiel worden toegepast op alle gebruikers, tenzij anders aangegeven.

1. In het Globale Profiel, selecteer de **Voorwaardelijke Attributen** tabel.

1. Klik [!UICONTROL **uitgeven**] in de hoogste linkerhoek van het scherm.

   ![&#x200B; Voorwaardelijke Attributen &#x200B;](images/lesson-3/edit-conditional-attributes.png)

1. Klik [!UICONTROL **toevoegen**].

1. Vul de **Naam**, **Waarde**, en **Etiket** gebieden voor de nieuwe voorwaarde.

   ![&#x200B; nieuwe Voorwaarde &#x200B;](images/lesson-3/new-condition.png)

1. Klik [!UICONTROL **sparen**] bij de hoogste linkerhoek van het scherm.
De nieuwe voorwaarde is nu beschikbaar voor alle gebruikers. U kunt het selecteren in het deelvenster Eigenschappen van inhoud en het toepassen op de gewenste inhoud.

## Een nieuw mapprofiel maken

Naast het standaard algemene profiel kunt u ook uw eigen aangepaste profielen maken.

1. Van het scherm van de Navigatie, klik het [!UICONTROL **pictogram van Hulpmiddelen**].

   ![&#x200B; Pictogram van Hulpmiddelen &#x200B;](images/reuse/tools-icon.png)

1. Selecteer **Gidsen** op het linkerpaneel.

1. Klik de **tegel van Profielen van de 1&rbrace; omslag 0&rbrace;.**

   ![&#x200B; Profielen van de Omslag &#x200B;](images/reuse/folder-profiles-tile.png)

1. Klik [!UICONTROL **creëren**].

1. In het dialoogvenster Mapprofiel maken.

   a. Geef het profiel een naam.

   b. Geef een pad op.

   c. Klik [!UICONTROL **creëren**].

   ![&#x200B; creeer het Profiel van de Omslag &#x200B;](images/lesson-3/create-folder-profile.png)

Er wordt een tegel met de nieuwe profielnaam weergegeven op de pagina Mapprofielen.

## Beheerders toevoegen via het tabblad Algemeen

Administratieve gebruikers hebben rechten om de Voorwaardelijke Attributen, het Authoring Malplaatje, en de Voorinstellingen van de Output voor het Profiel van de Omslag bij te werken.

1. Klik op de tegel om het gewenste mapprofiel te openen.

   ![&#x200B; geef het Profiel van de Omslag uit &#x200B;](images/lesson-3/edit-folder-profile.png)

1. Selecteer het **Algemene** lusje.

1. Klik [!UICONTROL **uitgeven**] bij de bovenkant verlaten van het scherm.

1. Selecteer onder Admin-gebruikers een gebruiker in het vervolgkeuzemenu of typ de naam van een gebruiker.

1. Klik [!UICONTROL **toevoegen**].

   U kunt desgewenst meerdere Admin-gebruikers toevoegen.

   ![&#x200B; voeg Admin &#x200B;](images/lesson-3/add-admin.png) toe

1. Klik [!UICONTROL **sparen**] in de hoogste juiste hoek van het scherm wanneer alle gebruikers zijn toegevoegd.

Administratieve gebruikers worden nu toegewezen aan dit profiel.

## Een nieuw publiek toevoegen via het tabblad Voorwaardelijke kenmerken

Zodra u het Globale Profiel hebt betreden kunt u zijn configuratie uitgeven. De instellingen voor het algemene profiel worden toegepast op alle gebruikers, tenzij anders aangegeven.

1. Van binnen het gewenste Profiel van de Omslag, selecteer de **Voorwaardelijke Attributen** tabel.

1. Klik [!UICONTROL **uitgeven**] in de hoogste linkerhoek van het scherm.

   ![&#x200B; geef Voorwaardelijke Attributen 2 &#x200B;](images/lesson-3/edit-conditional-attributes-2.png) uit

1. Klik [!UICONTROL **toevoegen**].

1. Vul de **Naam**, **Waarde**, en **Etiket** gebieden voor de nieuwe voorwaarde.

   Het klikken van [!UICONTROL **plus**] teken staat u toe om extra paren van de Waarde en van het Etiket voor de genoemde attributen toe te voegen.

   ![&#x200B; voegt Voorwaarden &#x200B;](images/lesson-3/add-conditions.png) toe

1. Klik [!UICONTROL **sparen**] bij de hoogste linkerhoek van het scherm.

De nieuwe voorwaardelijke kenmerken zijn toegevoegd aan dit profiel.

## Kies een sjabloon en een kaart op het tabblad Ontwerpsjablonen

AEM Guides wordt geleverd met kant-en-klare ontwerpsjablonen en -kaarten. U kunt deze beperken tot specifieke auteurs. Standaard worden de sjablonen opgeslagen op de Assets-locatie in een map met DITA-sjablonen.

1. Selecteer het tabblad Ontwerpsjablonen in het gewenste mapprofiel.

1. Klik op Bewerken in de linkerbovenhoek van het scherm.

1. Voeg een Kaartsjabloon toe.

   a. Van **Malplaatjes van de Kaart** dropdown, selecteer een optie van de beschikbare kaarten.

   b. Klik [!UICONTROL **toevoegen**].

   ![&#x200B; Malplaatjes van de Kaart &#x200B;](images/lesson-3/map-templates.png)

1. Voeg een onderwerpsjabloon toe.

   a. Van **Malplaatjes van het Onderwerp** dropdown, selecteer een optie van de beschikbare malplaatjes.

   ![&#x200B; de Malplaatjes van het Onderwerp &#x200B;](images/lesson-3/topic-templates.png)

1. Klik [!UICONTROL **toevoegen**].

1. Voeg desgewenst aanvullende onderwerpsjablonen toe.

1. Wanneer gebeëindigd, klik [!UICONTROL **sparen**] bij de bovenkant verlaten van het scherm.

De nieuwe ontwerpsjablonen zijn toegevoegd aan dit profiel.

## Niet-essentiële voorinstellingen verwijderen op het tabblad Voorinstellingen voor uitvoer

U kunt elke voorinstelling voor uitvoer configureren op basis van het mapprofiel. Uitvoervoorinstellingen die niet nodig zijn, moeten worden verwijderd.

1. Van binnen het gewenste Profiel van de Omslag, selecteer de **Output vooraf instelt** tabel.

1. Schakel in het linkerdeelvenster de selectievakjes in van alle voorinstellingen die niet vereist zijn.

   ![&#x200B; schrapt vooraf instelt &#x200B;](images/lesson-3/delete-presets.png)

1. Klik [!UICONTROL **Vooraf ingestelde Schrapping**] in de hoogste linkerhoek van het scherm.

1. In de Schrapping stelt dialoog vooraf in, klik [!UICONTROL **Schrapping**].

   ![&#x200B; Schrapping &#x200B;](images/lesson-3/delete.png)

De enige voorinstellingen voor uitvoer die worden weergegeven, zijn de voorinstellingen die worden gebruikt.

## Een fragment uploaden vanaf het tabblad Configuratie van de XML-editor

1. Van binnen het gewenste Profiel van de Omslag, selecteer het **lusje van de Configuratie van de Redacteur van 0&rbrace; XML.**

1. Onder de Fragmenten van de Redacteur van XML, klik [!UICONTROL **uploadt**].

   ![&#x200B; uploadt Fragment &#x200B;](images/lesson-3/upload-snippet.png)

1. Navigeer naar een eerder gemaakt fragment.

1. Klik [!UICONTROL **Open**].

1. Klik [!UICONTROL **sparen**] bij de bovenkant verlaten van het scherm.

U hebt met succes de Configuratie van de Redacteur gewijzigd om Fragmenten op te nemen.

## Geef het mapprofiel op in de opslagplaats

In de Editor ziet u de resultaten van de wijzigingen die u hebt aangebracht in de mapprofielen.

1. Navigeer aan **Mening van de Bewaarplaats**.

1. Klik op de map voor de inhoud waarmee u wilt werken.

1. Klik het [!UICONTROL **pictogram van de Voorkeur van de Gebruiker**] op de hoogste toolbar.

   ![&#x200B; Voorkeur van de Gebruiker &#x200B;](images/lesson-3/hr-user-prefs.png)

1. Selecteer in het dialoogvenster Gebruikersvoorkeuren het gewenste mapprofiel in de vervolgkeuzelijst.

   ![&#x200B; Uitgezochte de Voorkeur van de Gebruiker &#x200B;](images/lesson-3/select-user-pref.png)

1. Klik [!UICONTROL **sparen**].

U hebt het mapprofiel toegepast op uw inhoud. Nu, wanneer u een nieuw onderwerp DITA creeert, zult u een beperkte lijst van onderwerptypes zien die op het Profiel van de Omslag wordt gebaseerd. De voorwaarde van het publiek bevat de Globale montages evenals die specifiek voor het Profiel van de Omslag. In het geüploade fragmentbestand is een set standaardfragmenten gemaakt waaruit u kunt kiezen. Op het dashboard Kaart worden de beperkte uitvoervoorinstellingen weergegeven.
