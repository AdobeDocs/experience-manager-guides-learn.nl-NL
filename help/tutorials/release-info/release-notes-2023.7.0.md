---
title: Opmerkingen bij de release | Upgrade-instructies en opgeloste problemen in Adobe Experience Manager-hulplijnen, release van juni 2023
description: Meer informatie over de opgeloste problemen en hoe u een upgrade uitvoert naar de as a Cloud Service release van Adobe Experience Manager Guides van juli 2023
source-git-commit: 4ba47a803eec7bcbb106c34a1ad6a7fbed9934be
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 1%

---

# Release van Adobe Experience Manager Guides in juni 2023 as a Cloud Service

In deze releaseopmerking worden de instructies voor het bijwerken, de compatibiliteitsmatrix en de problemen behandeld die zijn opgelost in versie juli 2023 van de Adobe Experience Manager-hulplijnen (later aangeduid als *Hulplijnen AEM as a Cloud Service*).

Voor meer informatie over de nieuwe functies en verbeteringen raadpleegt u [Nieuwe functies in juli 2023 - release van AEM hulplijnen as a Cloud Service](whats-new-2023.7.0.md).

## Upgrade naar release juli 2023

Voer de volgende stappen uit om de huidige installatie van de AEM hulplijnen te upgraden:

1. Controle uit de Cloud Services Gespitscode en schakelaar aan de tak die in de Cloud Services wordt gevormd die aan het milieu beantwoordt dat u wilt bevorderen.
2. Bijwerken `<dox.version>` eigenschap in `/dox/dox.installer/pom.xml` bestand van de Git-code van de Cloud Services naar 2023.7.0.314.
3. Leg de wijzigingen vast en voer de Cloud Services-pijplijn uit om naar de release van juli 2023 van AEM as a Cloud Service hulplijnen te upgraden.

## Stappen om de trigger van een script via een servlet in te schakelen

(Alleen als u een versie hebt die ouder is dan juni 2023, release van AEM hulplijnen as a Cloud Service)

Nadat u de installatie hebt voltooid, kunt u ervoor kiezen om de trigger te HIT om de vertaaltaak te starten:

POST:

```
http://localhost:4503/bin/guides/script/start?jobType=translation-map-upgrade
```

Reactie:

```
{
"msg": "Job is successfully submitted and lock node is created for future reference",
"lockNodePath": "/var/dxml/executor-locks/translation-map-upgrade/1683190032886",
"status": "SCHEDULED"
}
```

In de vorige reactie van JSON was de sleutel `lockNodePath` bevat het pad naar het knooppunt dat in de opslagplaats is gemaakt en dat naar de ingediende taak verwijst. Het wordt automatisch verwijderd als de taak is voltooid. Tot dan kunt u naar dit knooppunt verwijzen voor de huidige status van de taak.

Wacht tot deze taak is voltooid voordat u verdergaat met de volgende stappen.

>[!NOTE]
>
> Controleer of het knooppunt nog aanwezig is en wat de status van de taak is.

```
GET
http://<aem_domain>/var/dxml/executor-locks/translation-map-upgrade/1683190032886.json
```

## Stappen om de bestaande inhoud te posten om het verbroken koppelingsrapport te gebruiken

(Alleen als u een versie hebt die ouder is dan juni 2023, release van AEM hulplijnen as a Cloud Service)

Voer de volgende stappen uit voor de naverwerking van de bestaande inhoud en het gebruik van het nieuwe verbroken koppelingsrapport:

1. (Optioneel) Als het systeem meer dan 100.000 dita-bestanden bevat, werkt u de `queryLimitReads` krachtens `org.apache.jackrabbit.oak.query.QueryEngineSettingsService` naar een hogere waarde (een waarde die groter is dan het aantal aanwezige elementen, bijvoorbeeld 200.000) en vervolgens opnieuw te implementeren.

   - Gebruik de instructies die worden gegeven in *Configuratieoverschrijvingen* in Installeer en vorm as a Cloud Service de Gidsen van Adobe Experience Manager, om het configuratiedossier tot stand te brengen.
   - In het configuratiedossier, verstrek de volgende (bezit) details om de queryLimitReads optie te vormen:

     | PID | Eigenschappensleutel | Waarde van eigenschap |
     |---|---|---|
     | org.apache.jackrabbit.oak.query.QueryEngineSettingsService | queryLimitReads | Waarde: 200000 Standaardwaarde: 100000 |

1. Voer een verzoek van de POST op de server uit (met correcte authentificatie) - `http://<server:port>//bin/guides/reports/upgrade`.

1. De API retourneert een jobId. Als u de status van de taak wilt controleren, kunt u een aanvraag van een GET met taak-id naar hetzelfde eindpunt verzenden - `http://<server:port>/bin/guides/reports/upgrade?jobId= {jobId}`
(Bijvoorbeeld: `http://localhost:8080/bin/guides/map-find/indexing?jobId=2022/9/15/7/27/7dfa1271-981e-4617-b5a4-c18379f11c42_678`)

1. Wanneer de taak is voltooid, reageert de vorige GET-aanvraag met succes. Als de taak om een of andere reden mislukt, kan de fout worden gezien in de serverlogboeken.

1. Terugkeren naar de standaardwaarde of vorige bestaande waarde van `queryLimitReads` als u dit in stap 1 hebt gewijzigd.

## Stappen om de bestaande inhoud te indexeren om de nieuwe zoek- en vervangings- en onderwerpenlijst onder het tabblad Rapporten te gebruiken:

(Alleen als u een versie hebt die ouder is dan juni 2023, release van AEM hulplijnen as a Cloud Service)

Voer de volgende stappen uit om de bestaande inhoud te indexeren en de nieuwe vondst en vervangt tekst op kaartniveau en onderwerpenlijst onder het rapportlusje te gebruiken:

1. Een verzoek van een POST uitvoeren op de server \(met correcte verificatie\) - `http://<server:port\>/bin/guides/map-find/indexing`. (Optioneel: U kunt specifieke paden van de kaarten doorgeven om deze te indexeren. Standaard worden alle kaarten geïndexeerd \|\| Bijvoorbeeld: `https://<Server:port\>/bin/guides/map-find/indexing?paths=<map\_path\_in\_repository\>`)

1. U kunt ook een hoofdmap doorgeven om de DITA-kaarten van een specifieke map (en de bijbehorende submappen) te indexeren. Bijvoorbeeld, `http://<server:port\>/bin/guides/map-find/indexing?root=/content/dam/test`. Wanneer zowel de parameter paths als de hoofdparameter worden doorgegeven, wordt alleen de parameter paths gebruikt.

1. De API retourneert een jobId. Als u de status van de taak wilt controleren, kunt u een aanvraag van een GET met taak-id naar hetzelfde eindpunt verzenden - `http://<server:port\>/bin/guides/map-find/indexing?jobId=\{jobId\}`\(Bijvoorbeeld: `http://localhost:8080/bin/guides/map-find/indexing?jobId=2022/9/15/7/27/7dfa1271-981e-4617-b5a4-c18379f11c42`\)


1. Wanneer de taak is voltooid, reageert het vorige verzoek van de GET met succes en wordt vermeld of kaarten zijn mislukt. De met succes geïndexeerde kaarten kunnen van de serverlogboeken worden bevestigd.

## Compatibiliteitsmatrix

In deze sectie wordt een overzicht gegeven van de compatibiliteitsmatrix voor de softwaretoepassingen die worden ondersteund door AEM in de release van juli 2023 as a Cloud Service hulplijnen.

### FrameMaker en het Publiceren FrameMaker Server

| Hulplijnen AEM als Cloud Release | FMPS | FrameMaker |
| --- | --- | --- |
| 2023.07.0 | Niet compatibel | 2022 of hoger |
| | | |


### Zuurstofaansluiting

| Hulplijnen AEM als Cloud Release | Oxygeenaansluiting, Windows | Oxygeenconnector Mac | Bewerken in Oxygen Windows | Bewerken in Oxygen Mac |
| --- | --- | --- | --- | --- |
| 2023.07.0 | 2.9-uuid-2 | 2.9-uuid-2 | 2.3 | 2.3 |
|  |  |  |  |


## Opgeloste problemen

De fouten die in verschillende gebieden zijn gecorrigeerd, worden hieronder weergegeven:

### Authoring

- De inline-/weergavekenmerken worden niet weergegeven in de layoutweergave van de webeditor. (12498)
- Bestanden uploaden in de insteekmodule Oxygen voor AEM hulplijnen werkt niet in cloudservices als u dat hebt! in de bestandsnaam. (12207)
- Het publiceren van DITA-kaarten gaat erg langzaam met bewerkbare sjablonen. (12075)
- De globale configuratie van het Profiel UI past niet met het Profiel van de Omslag aan. (11970)
- Inhoudsverwijzingen worden verbroken wanneer DITA-bestanden worden gekopieerd en geplakt. (11959)
- Kan inhoudsfragment niet bewerken in de kolomweergave met AEM hulplijnen geïnstalleerd. (7342)
- Inhoud gaat verloren wanneer een onverpakt xref zich onder subelementtags bevindt. (12532)

### Publiceren

- De goedkeuringswerkstroom werkt niet wanneer de documentstatus wordt gewijzigd in &quot;eindstatus&quot; in de bestandseigenschappen van het rechterdeelvenster. (11026)

