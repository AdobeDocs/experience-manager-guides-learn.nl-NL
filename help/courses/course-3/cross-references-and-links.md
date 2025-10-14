---
title: Kruisverwijzingen en koppelingen
description: Kruisverwijzingen en koppelingen maken in AEM Guides
exl-id: bee7d50f-cbdd-4ac8-b15b-101febc4ae80
source-git-commit: 67ba514616a0bf4449aeda035161d1caae0c3f50
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Kruisverwijzingen en koppelingen

De Redacteur van XML en DITA verstrekken een krachtige manier om tussen onderwerpen te verbinden. Het is belangrijk dat u de verwijzingen naar inhoud op effectieve wijze beheert. U moet daarbij ook werken met unieke id-waarden.

Voorbeeldbestanden die u voor deze les wilt gebruiken, staan in het bestand
[&#x200B; crossreferencesandlinks.zip &#x200B;](assets/crossreferencesandlinks.zip)

>[!VIDEO](https://video.tv.adobe.com/v/342764?quality=12&learn=on)

## Een kruisverwijzing naar een extern onderwerp maken

Het is mogelijk om een externe kruisverwijzing te maken door een onderwerp vanuit de opslagplaats naar een geopend bestand te slepen. Als u echter verbroken kruisverwijzingen wilt voorkomen, moet een id eerst worden gedefinieerd voor een waarde die gerelateerd is aan het bovenliggende element. Dit is een eenvoudige manier om een kruisverwijzing te maken en er tegelijkertijd voor te zorgen dat id&#39;s correct worden toegewezen.

1. Open een bestand waarin u een externe kruisverwijzing wilt invoegen.

1. Wijs een id toe aan het element waarnaar moet worden verwezen.

   a. Klik in het element.

   b. Op het paneel van Eigenschappen van de Inhoud, kies **identiteitskaart** van het drop-down Attribuut.

   c. Typ een logische naam in het veld Waarde.

   d. Bekijk het element en zijn waarde in **Mening van het Overzicht** indien gewenst.

1. **sparen** het onderwerp om Repository te verzekeren heeft bijgewerkte identiteitskaart.

1. Klik het [!UICONTROL **pictogram van de Verwijzing**] op de hoogste toolbar.

   ![&#x200B; Toolbar &#x200B;](images/lesson-7/references-icon.png)

1. Van het **lusje van de Verwijzing van de Inhoud**, selecteer identiteitskaart en element die u als verwijzing wilt opnemen.

1. Klik [!UICONTROL **Uitgezocht**].

De kruisverwijzing is toegevoegd aan het onderwerp.

## Koppelen naar een website

U kunt een koppeling invoegen naar een website in een willekeurig onderwerp. Raadpleeg de video AEM Guides Cursus 1 over Koppelen naar websites voor meer informatie.


## verbroken koppelingen weergeven

Sommige wijzigingen kunnen leiden tot verbroken kruisverwijzingen. Deze omvatten het schrappen van een onderwerp, het reorganiseren van een sectie die een verwijzing bevat, of het veranderen van identiteitskaart nadat de verwijzing is opgenomen. Merk op dat een steekproefonderwerp _crossreferencesandlinks.zip_ van deze les wordt voorzien die verscheidene van bulleted verwijzingen naar interne inhoud zal veroorzaken om te breken.

1. Navigeer aan de **Mening van het Overzicht** op het linkerpaneel.

1. Klik het [!UICONTROL **pictogram van de Filter**].

1. Selecteer **Verbroken verbindingen**.

   ![&#x200B; Dropdown van de Filter &#x200B;](images/lesson-7/broken-links.png)

Verbroken koppelingen worden weergegeven als klikbare objecten. U kunt ze in rode tekst in het onderwerp identificeren.
