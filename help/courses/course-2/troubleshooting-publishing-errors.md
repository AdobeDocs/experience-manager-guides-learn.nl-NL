---
title: Problemen met publicatiefouten oplossen
description: Problemen met het publiceren van fouten oplossen in  [!DNL Adobe Experience Manager Guides]
exl-id: b37ea3e7-59cf-4fc5-8fae-e1fadd26f8d8
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Problemen met publicatiefouten oplossen

Het publiceren van een kaart is doorgaans eenvoudig. Open de kaart, selecteer een Vooraf ingestelde Output, en produceer output! Nochtans, als een kaart, of zijn onderwerpen fouten in hen hebben kan de outputgeneratie ontbreken. Wanneer dit gebeurt, is het belangrijk om te weten hoe te problemen op te lossen.

>[!VIDEO](https://video.tv.adobe.com/v/338990?quality=12&learn=on)

## De oefening voorbereiden

U kunt hier voorbeeldbestanden downloaden voor de oefening.

[&#x200B; oefening-Download &#x200B;](assets/exercises/publishing-basic-to-advanced.zip)

## Algemene oorzaken van publicatiefouten

Er kunnen fouten in de broninhoud worden ingevoegd. Bijvoorbeeld:

* Verwijzing naar bestandspad met onjuiste naam

* Onjuiste benoemde map

* Afbeelding of bestand ontbreekt

* Onjuist geconfigureerde inhoudsverwijzing

* Verbroken kruisverwijzing

* Fouten in de waarden van een kenmerk (bijvoorbeeld een tekenreeks in plaats van een getal)

* Onjuiste installatie van componenten die door [!DNL AEM Guides] worden gebruikt

## Gevolgen van fouten

Een fout kan klein zijn en in een eenvoudige nota resulteren om u te laten weten dat een dossier niet met succes werd verpakt, of ernstig genoeg dat het tot een volledig mislukken leidt om output te produceren. Op het tabblad Uitvoer worden pictogrammen met kleurcodering weergegeven om aan te tonen dat de uitvoer is gelukt, dat er fouten zijn opgetreden of dat de uitvoer is gegenereerd.

![&#x200B; fout-effect &#x200B;](images/error-impact.png)

## Logbestanden van fouten openen en bekijken

Het logbestand dat wordt gegenereerd, kan worden geopend voor revisie.

1. In het **lusje van Output**, klik de **datum/tijd onder Gegenereerd bij.**

   ![&#x200B; fout-logboek &#x200B;](images/error-log.png)

1. Blader door het foutenlogboek.

## Fouttypen weergeven en verbergen

In het foutenlogboek wordt elk fouttype in een unieke kleur weergegeven.

![&#x200B; navigate-fouten &#x200B;](images/navigate-errors.png)

1. **Uitgezochte** of **schrap** om het even welk foutentype om het benadrukken te tonen of te verbergen.

1. Navigeer fouten gebruikend **volgende** of **vorige** knopen (pijlen).

## Fouten oplossen

Afhankelijk van het type fout kan de resolutie eenvoudig of complex zijn. Het kan door een auteur in de Redacteur van XML worden voltooid, of kan een beheerder vereisen om met [!DNL AEM Guides] te werken. Specifieke correcties zijn afhankelijk van de fout, het effect en uw organisatorische workflows.

* Verwijzing naar bestandspad met onjuiste naam

       de Auteurs kunnen de wegverwijzing in het brondocument bijwerken.
     
  
* Onjuiste benoemde map

       de Auteurs kunnen de omslagnaam bijwerken of dossiers bewegen zoals nodig.
     
  
* Afbeelding of bestand ontbreekt

       de Auteurs kunnen ontbrekende grafisch/dossier uploaden, een grafisch/dossier anders noemen, of een grafisch/dossier bewegen 
     
  
* Onjuist geconfigureerde inhoudsverwijzing

       de Auteurs kunnen de plaats van de inhoud verbeteren van verwijzingen voorzien, of de weg veranderen aan de inhoudsverwijzing.
     
  
* Verbroken kruisverwijzing

       de Auteurs kunnen de plaats verbeteren de verwijzing naar, of de naam of de eigenschappen van het bestemmingsdossier veranderen 
     
  
* Fouten in de waarden van een kenmerk (bijvoorbeeld een tekenreeks in plaats van een getal)

       de Auteurs kunnen de attributen aan een correcte waarde bijwerken of de beheerders kunnen het systeem bijwerken om nieuwe waarden te steunen.
     
  
* Onjuiste installatie van componenten die door [!DNL AEM Guides] worden gebruikt

       de Beheerders kunnen de installatie van het systeem, zijn componenten, of toestemmingen bijwerken.
     
  