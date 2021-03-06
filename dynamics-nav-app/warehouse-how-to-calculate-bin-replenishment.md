---
title: "Vorgehensweise: Lagerplatzauffüllung berechnen"
description: "Wenn der Lagerort so eingerichtet wurde, dass er die gesteuerte Einlagerung und Kommissionierung verwendet, werden die Prioritäten der Einlagerungsvorlage für den Lagerplatz berücksichtigt, wenn Wareneingänge eingelagert werden."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/23/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3a6ff833aad54cf98720857a8ae67492abe9af4f
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-calculate-bin-replenishment"></a>Vorgehensweise: Lagerplatzauffüllung berechnen
Wenn der Lagerort so eingerichtet wurde, dass er die gesteuerte Einlagerung und Kommissionierung verwendet, werden die Prioritäten der Einlagerungsvorlage für den Lagerplatz berücksichtigt, wenn Wareneingänge eingelagert werden. Prioritäten umfassen die minimalen und maximalen Mengen des Lagerplatzinhalts, die für einen bestimmten Lagerplatz verknüpft wurden, und die Lagerplatzprioritäten. Wenn daher gleichmäßig Artikel ankommen, werden die meistverwendeten Kommissionierlagerplätze nachgefüllt, während gleichzeitig Artikel aus ihnen entnommen werden.  

Artikel treffen jedoch nicht immer gleichmäßig im Lager ein. Manchmal werden Artikel in großen Mengen gekauft, so dass das Unternehmen einen Rabatt erhalten kann, oder Ihre Fertigung produziert eine größere Menge eines Artikels, um geringe Stückkosten zu erzielen. Dann wiederum erhält das Lager eine Zeit lang keine Artikel mehr und Lagermitarbeiter müssen regelmäßig Artikel aus Palettenlagerplätzen in Kommissionierlagerplätze umpacken.  

Es ist auch möglich, dass das Lager neue Lieferungen erwartet und daher die Palettenlagerplätze frei machen möchte, bevor die neue Ware eintrifft.  

Wenn Sie Ihre Palettenlagerplätze mit einer Lagerplatzart definiert haben, die ausschließlich die Aktion **Einlagerung** vorsieht, d. h. die Lagerplatzart hat kein Häkchen bei der Aktion **Kommissionierung**, müssen Sie immer darauf achten, dass Ihre Kommissionierlagerplätze gefüllt sind, da keine Kommissionierung aus Einlagerungslagerplätzen vorgeschlagen wird.  

## <a name="to-replenish-pick-bins"></a>So füllen Sie Kommissionierlagerplätze auf:  
1.  Wählen Sie in der rechten oberen Ecke das Symbol ![Nach Seite oder Bericht suchen] Symbol (media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben Sie **Lagerplatzumlagerungsvorschlag** ein. Wählen Sie dann den zugehörigen Link aus.  
2.  Wählen Sie die Aktion **Lagerplatzauffüllung berechnen** aus, um die Berichtanforderungsseite zu öffnen.  
3.  Füllen Sie das Anforderungsfenster der Stapelverarbeitung aus, um den Umfang der Auffüllvorschläge zu begrenzen, die berechnet werden. Beispielsweise könnten Sie nur für bestimmte Artikel, Zonen oder Lagerplätze zuständig sein.  
4.  Wählen Sie die Schaltfläche **OK** aus. Es werden Zeilen für die Auffüllumlagerungen erstellt, die ausgeführt werden müssen, entsprechend den Regeln, die für Lagerplätze und Lagerplatzinhalte (Artikel in Lagerplätzen) festgelegt wurden.  
5.  Wenn Sie alle vorgeschlagenen Auffüllungen vornehmen möchten, wählen Sie die Aktionen **Lagerplatzumlagerung erstellen** aus. Die Lagermitarbeiter finden jetzt Anweisungen unter dem Menüpunkt **Lagerplatzumlagerungen**, können diese ausführen und sie registrieren.  
6.  Wenn Sie nur einige der Vorschläge ausführen möchten, löschen Sie die weniger wichtigen Zeilen und erzeugen Sie dann eine Lagerplatzumlagerung.  

Wenn Sie das nächste Mal eine Lagerplatzauffüllung berechnen lassen, werden Ihnen wieder die Zeilen vorgeschlagen, die Sie gelöscht haben, wenn diese dann immer noch gültig sind.  

> [!NOTE]  
>  Angenommen, die folgenden Bedingungen werden für einen Artikel erfüllt:  
>   
>  -   Der Artikel weist ein Ablaufdatum auf, und  
> -   Das Feld **Gemäß FEFO kommissionieren** ist auf der Lagerortkarte aktiviert, und  
> -   Sie verwenden die Funktionalität **Lagerplatzauffüllung berechnen**.  
>   
>  In diesem Fall bleiben die Felder **Von Zone** und **Von Lagerplatz** leer, da der Algorithmus zur Berechnung des Ausgangsortes der Umlagerung nur ausgelöst wird, wenn Sie die Funktion **Lagerplatzumlagerung erstellen** aktivieren.  

## <a name="see-also"></a>Siehe auch  
[Logistik](warehouse-manage-warehouse.md)  
[Kommissionierung nach FEFO](warehouse-picking-by-fefo.md)  
[Lagerbest](inventory-manage-inventory.md)  
[Lagerortverwaltung einrichten](warehouse-setup-warehouse.md)     
[Montageverwaltung](assembly-assemble-items.md)    
[Designdetails: Logistik](design-details-warehouse-management.md)  
[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

