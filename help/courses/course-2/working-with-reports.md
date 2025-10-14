---
title: Werken met rapporten
description: Werken met rapporten in  [!DNL Adobe Experience Manager Guides]
exl-id: 755506a6-c416-4a8c-8359-8db7e63a90a4
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Werken met rapporten

Op het tabblad Rapporten in het dashboard Kaart kunt u verbroken koppelingen, inhoud waarnaar wordt verwezen en die opnieuw wordt gebruikt (conrefs), kruisverwijzingen of andere ontbrekende informatie identificeren en oplossen.

>[!VIDEO](https://video.tv.adobe.com/v/339039?quality=12&learn=on)

## De oefening voorbereiden

U kunt hier voorbeeldbestanden downloaden voor de oefening.

[Oefening-downloaden](assets/exercises/working-with-reports.zip)

## Assets uploaden

1. Selecteer in de weergave Opslagplaats het pictogram Ovaal in de hoofdmap om het menu Opties te openen.

   ![&#x200B; ellipses-9.png &#x200B;](images/ellipses-9.png)

1. Selecteer **[!UICONTROL Upload Assets]** .

   ![&#x200B; upload-assets.png &#x200B;](images/upload-assets.png)

1. Selecteer de dossiers u aan de omslag wilt uploaden, en **selecteren uploadt**.

De DITA-bestanden worden geopend en u moet ze controleren op problemen met ontbrekende inhoud, conrefs of kruisverwijzingen.

## Een kaart maken

1. Selecteer het pictogram Ovaal in de hoofdmap om het menu Opties te openen.

   ![&#x200B; ellipses-9.png &#x200B;](images/ellipses-9.png)

1. Selecteer **creeer > Kaart**.

   ![&#x200B; create-map.png &#x200B;](images/create-map.png)

   Het dialoogvenster Nieuwe kaart maken wordt weergegeven.

1. Op het gebied van het Malplaatje, uitgezochte **Bookmap** (of **Kaart** die op het inhoudstype wordt gebaseerd u) van het drop-down menu creeert en uw kaart een titel geeft.

1. Selecteer **creeer**.

Uw kaart wordt gemaakt en de linkerrails veranderen automatisch van de weergave Opslagplaats naar de weergave Kaart.

## Toevoegen van kaartcomponenten

1. Selecteer het potloodpictogram in de linkerspoorstaaf.
Dit is het bewerkingspictogram, waarmee u de kaart in de editor kunt openen.

   ![&#x200B; uitgeven-map.png &#x200B;](images/edit-map.png)

1. Schakel terug naar de weergave Opslagplaats door het pictogram Opslagplaats te selecteren.

   ![&#x200B; bewaarplaats-button.png &#x200B;](images/repository-button.png)

1. Voeg een onderwerp aan de kaart toe door het van Repository in de kaart in de redacteur te slepen en te laten vallen.
De lijnindicator zal u tonen waar uw onderwerp zal worden geplaatst.

1. Voeg desgewenst onderwerpen toe.

1. Wanneer gebeëindigd, uitgezocht **sparen als Nieuwe Versie.**

   ![&#x200B; save-as-new-version.png &#x200B;](images/save-as-new-version.png)

1. Op *Commentaren voor het nieuwe gebied van de Versie*, ga een beschrijvende commentaar in.

1. Selecteer **sparen**.

## Een AEM Site-uitvoer genereren

1. In Bewaarplaats, selecteer het pictogram van de Ellipsis op uw kaart om het menu van Opties te openen, en dan **Open het Dashboard van de Kaart.**

   ![&#x200B; open-map-dashboard.png &#x200B;](images/open-map-dashboard.png)

   Het kaartdashboard wordt op een ander tabblad geopend.
1. In de Output stelt lusje vooraf in, uitgezochte **AEM Plaats**.

   ![&#x200B; a-plaats-checkbox &#x200B;](images/aem-site-checkbox.png)

1. Selecteer **produceren**.

1. Navigeer naar de pagina Outputs om de status van uw geproduceerde output te bekijken.
Als er fouten zijn, kan op het tabblad Uitvoer een oranje cirkel worden weergegeven onder de kolom Generatie-instelling in plaats van groen om aan te geven dat het genereren is voltooid.

1. Selecteer de koppeling onder de kolom Generatie-instelling om de gegenereerde uitvoer te openen.
Controleer de uitvoer op ontbrekende inhoud.

## Het tabblad Rapporten

Het lusje van Rapporten toont een onderwerpsamenvatting, en een lijst die onderwerpinformatie en de kwesties binnen uw kaart bevatten.

In het ideale geval controleert u altijd de Rapporten op een kaart nadat u inhoud hebt geïmporteerd.

![&#x200B; reports.png &#x200B;](images/reports.png)

De kolom Ontbrekende elementen geeft het aantal ontbrekende afbeeldingen en verbroken conrefs aan. U kunt het **pictogram van het Potlood** selecteren om het onderwerp in de redacteur te openen.

## Ontbrekende afbeeldingen oplossen

Als er afbeeldingen ontbreken in uw bestanden, kan de algemene reden hiervoor zijn dat de inhoud wel is geüpload, maar dat dit niet het geval is bij afbeeldingen. Als dat het geval is, lost u de problemen met ontbrekende afbeeldingen op door afbeeldingen te uploaden naar een specifieke map die overeenkomt met het pad en de bestandsnamen die door bestanden worden verwacht.

1. In *Mening van de Bewaarplaats*, selecteer het pictogram van de Ovaal op uw beeldenomslag om het menu van Opties te openen.

   ![&#x200B; beeld-ellipsis.png &#x200B;](images/image-ellipsis.png)

1. Selecteer **[!UICONTROL Upload Assets]** en selecteer de ontbrekende afbeeldingen.

1. Selecteer **uploaden**.

De ontbrekende afbeeldingen zijn geüpload. Deze afbeeldingen worden nu weergegeven in een nieuw gegenereerde AEM Site-uitvoer en op het tabblad Rapporten worden geen fouten meer weergegeven.

## Gebroken conrefs oplossen

Als inhoud waarnaar elders wordt verwezen (een conref), verwijst naar een bestand in een andere map (bijvoorbeeld een map met de naam &quot;reuse&quot;). en de inhoud niet is geüpload, moet een fout worden opgelost. U moet bijvoorbeeld een submap maken met de naam &quot;hergebruik&quot; en het ontbrekende bestand uploaden naar &quot;hergebruik&quot;.

### Middelen uploaden met de gebruikersinterface van [!UICONTROL Assets]

Naast de optie [!UICONTROL Upload Assets] kunt u ook elementen uploaden door deze naar de gebruikersinterface van Assets te slepen.

1. Selecteer in de weergave Opslagplaats het Ellipsis-pictogram in de map voor hergebruik om het menu Opties te openen.

   ![&#x200B; hergebruik-ellipsis.png &#x200B;](images/reuse-ellipsis.png)

1. Selecteer **Mening in Assets UI**.

   ![&#x200B; assets_ui.png &#x200B;](images/assets_ui.png)

1. Sleep het bestand naar de map.
Het bestand wordt geüpload en de fout conref is opgelost.

Alle fouten zijn nu opgelost. De pagina Rapporten geeft aan dat er geen fouten meer zijn en het genereren van een AEM Site resulteert in een volledige uitvoer zonder ontbrekende componenten.
