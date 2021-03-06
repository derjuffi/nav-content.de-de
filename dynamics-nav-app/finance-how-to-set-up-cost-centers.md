---
title: Vorgehensweise beim Kostenstellen einrichten
description: "Kostenstellen sind Abteilungen, die für die Kosten und die Einnahmen zuständig sind. Der Kostenstellenplan ähnelt den Dimensionsinformationen für das Sachkonto."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 97c462edcfbc15153eb64037869c7e9e048e1fa1
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-cost-centers"></a>So geht's: Kostenstellen einrichten
Kostenstellen sind Abteilungen, die für die Kosten und die Einnahmen zuständig sind. Der Kostenstellenplan ähnelt den Dimensionsinformationen für das Sachkonto. Sie können den Kostenstellenplan auf die folgenden Weisen einrichten:  

-   Transferieren Sie Dimensionswerte im Sachkonto zum Kostenstellenplan. Sie können alle notwendigen Änderungen nach der Übertragung vornehmen.  
-   Erstellen Sie einen neuen Kostenstellenplan, der unabhängig vom Sachkonto ist, oder fügen Sie einem vorhandenen Kostenstellenplan eine neue Kostenstelle hinzu. Sie müssen jede Kostenstelle einzeln erstellen.  

## <a name="to-transfer-dimension-values-in-the-general-ledger-to-the-chart-of-cost-centers"></a>So transferieren Sie Dimensionswerte im Sachkonto zum Kostenstellenplan  
1.  Richten Sie eine Dimension als Kostenstellendimension im Fenster **Kostenstellendimension aktualisieren** ein. Nur die Werte aus dieser Dimension werden übertragen.  
2.  Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Symbol Nach Seite oder Bericht suchen"), geben Sie **Kostenstellen** ein, und wählen Sie dann den zugehörigen Link aus.  
3.  Klicken Sie auf der Registerkarte **Aktionen** in der Gruppe **Funktion** auf **Kostenstellen aus Dimension abrufen**, um Dimensionswerte zum Kostenstellenplan zu übertragen. Die Funktion überträgt die Dimensionswerte, die Sie in Schritt 1 definiert haben.  

    > [!NOTE]  
    >  Sie können das Feld **Kostenstellendimension ausrichten** so einrichten, dass eine unidirektionale Synchronisierung von Dimensionswerten aus dem Sachkonto zum Kostenstellenplan definiert wird. Sie können keine Synchronisierung des Kostenstellenplans mit Dimensionswerten aus dem Sachkonto definieren.  

Der Kostenstellenplan enthält jetzt alle angegebenen Dimensionswerte aus dem Sachkonto und umfasst Titel und Zwischensummen.  

## <a name="to-create-new-cost-centers-in-the-chart-of-cost-centers-window"></a>So richten Sie im Fenster Kostenstellenplan neue Kostenstellen ein  
Sie können Kostenkarten im Fenster **Kostenstellen** oder im Fenster **Kostenstellenkarte** einrichten und verwalten. So richten Sie im Fenster **Kostenstellenplan** neue Kostenstellen ein.  

1. Öffnen Sie das Fenster **Kostenstellenplan** im Bearbeitungsmodus.  
2. Geben Sie im Feld **Code** den Kostenstellencode ein. Alle Kostenstellen müssen einen Code aufweisen.  
3. Geben Sie im Feld **Namen** den Kostenstellennamen ein.  
4. Wählen Sie den Dropdownpfeil im Feld **Positionstyp** aus, um den Zweck der Kostenstelle anzugeben.  

    - Für Kostenstellen der Art **Summe** müssen Sie das Feld **Zusammenzählung** ausfüllen. Verwenden Sie den **Oder**-Operator, der eine vertikale Zeile (**&#124;**) ist, um Bereiche von Kostenstellen festzulegen.  
    - Für Kostenstellen der **Bis-Summe**-Zeilenart wird dieses Feld automatisch ausgefüllt, wenn Sie die Einzugsfunktion verwenden.  
5.  Füllen Sie die Felder **Sortierreihenfolge** und **Kostenunterart** aus.  
6.  Wählen Sie die nächste leere Zeile aus, um eine neue Kostenstelle zu erstellen. Wiederholen Sie dann die Schritte 2 bis 5.  
7.  Nachdem Sie alle Kostenstellen eingerichtet haben, wählen Sie die Aktion **Kostenstellen einrücken** aus. Wählen Sie die Schaltfläche **Ja** aus.  

> [!IMPORTANT]  
>  Wenn Sie Definitionen in den **Zusammenzählung**-Feldern für **Bis-Summe**-Kostenstellen eingegeben haben, bevor Sie die Einzugsfunktion ausführen, müssen Sie sie noch einmal eingeben. Die Funktion überschreibt die Werte in allen **Bis-Summe**-Feldern.  

## <a name="see-also"></a>Siehe auch  
[Kostenrechnung](finance-manage-cost-accounting.md)  
[Einrichten der Kostenrechnung](finance-set-up-cost-accounting.md)   
[Terminologie der Kostenrechnung](finance-terminology-in-cost-accounting.md)   
[Informationen zur Kostenrechnung](finance-about-cost-accounting.md)  
[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

