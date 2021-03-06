---
title: "Benutzeraktivität in einem Änderungsprotokoll nachverfolgen"
Description: "Sie können ein Benutzerprotokoll aktivieren, sodass Sie Aufzeichnungen über sämtliche Änderungen haben, die an den Daten in verfolgten Tabellen vorgenommen werden."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: user log, user activity, tracking
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 74d70c9929cfa29909281b964488319be7a9f127
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="logging-changes-in-dynamics-nav"></a>Änderungen in Dynamics NAV protokollieren
Sie können die Änderungsanmeldung aktivieren, sodass [!INCLUDE[d365fin](includes/d365fin_md.md)] Sie den Verlauf der Aktivitäten sehen. Das Protokoll basiert auf Änderungen, die an den Daten in den von Ihnen verfolgten Tabellen vorgenommen werden. Im Änderungsprotokoll sind Posten chronologisch bestellt und zeigt Änderungen an, die in den Feldern der angegebenen Tabellen vorgenommen wurden. Das Änderungsprotokoll erfasst alle Änderungen, die auf der Tabelle vorgenommen wurden.  

## <a name="working-with-the-change-log"></a>Arbeiten mit dem Änderungsprotokoll
Ein verbreitetes Problem in einem Finanzsystem ist die Lokalisierung von Fehlern und Änderungen von Daten. Es könnte alles sein – von einer falschen Kundentelefonnummer bis hin zu einer falschen Buchung in der Finanzbuchhaltung. Die Änderungsprotokollfunktion ermöglicht die Verfolgung aller direkten Änderungen, die von einem Benutzer an den Daten in der Datenbank vorgenommen werden. Sie müssen jede Tabelle und jedes Feld festlegen, die/das die Anwendung protokollieren soll, und dann das Änderungsprotokoll aktivieren.  

Sie verwenden das Fenster **Änderungsprotokoll einrichten** zum Aktivieren bzw. Deaktivieren des Änderungsprotokolls. Wenn Sie das Änderungsprotokoll aktivieren bzw. deaktivieren, wird diese Aktivität protokolliert, sodass Sie immer sehen, welcher Anwender die Protokollierung an- bzw. abgeschaltet hat. Dies kann nicht abgeschaltet werden.  

Wenn Sie im Fenster **Änderungsprotokoll Einrichtung** die Aktion **Tabellen** wählen, können Sie angeben, welche Tabellen auf Änderungen verfolgt werden sollen, und welche Änderungen verfolgt werden sollen. [!INCLUDE[d365fin](includes/d365fin_md.md)] verfolgt auch mehrere Systemtabellen.

Wenn Sie das Änderungsprotokoll eingerichtet und aktiviert haben und jemand Daten verändert hat, protokolliert die Anwendung die Änderung in einem **Änderungsprotokollposten**. Wenn Sie Posten löschen möchten, können Sie die im Fenster **Änderungsprotokollposten löschen** tun, an dem Sie Filter auf Basis Datum und Zeit festlegen können.  

## <a name="see-also"></a>Siehe auch
[Ändern von grundlegenden Einstellungen](ui-change-basic-settings.md)  
[Sortieren](ui-sorting.md)  
[Seite oder Bericht suchen verwenden](ui-search.md)  
[Vorgehensweise: Verwalten Sie Benutzer und Berechtigungen](ui-how-users-permissions.md)    
[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

