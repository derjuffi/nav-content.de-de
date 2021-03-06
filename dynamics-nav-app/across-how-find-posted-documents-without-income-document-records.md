---
title: "Suche nach Belegen ohne Dateianhänge"
Description: "Sie können nach Sachposten für gebuchte Einkaufs- und Verkaufsbelege suchen, die keine eingehenden elektronische Belege haben, wie importierte Rechnungen."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 515026b4da842afeda1759f50313dc26bcfd3350
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-find-posted-documents-without-incoming-document-records"></a>So wird's gemacht: Gebuchte Belege ohne Eingangsbelege finden
In den Fenstern **Kontenplan** und **Sachposten** können Sie eine Suchfunktion verwenden, um Sachposten für gebuchte Einkaufs- und Verkaufsbelege zu finden, für die keine eingehende Belegdatensätze vorhanden sind, und dann zentral eine Verknüpfung zu vorhandenen Datensätzen herstellen oder neue mit angefügten Belegdateien erstellen.

## <a name="to-find-posted-documents-without-incoming-document-records"></a>So finden Sie gebuchte Belege ohne zugehörige Eingangsbelege
1. Wählen Sie das Symbol ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Bericht suchen") aus und geben **Kontenplan** ein. Wählen Sie dann den zugehörigen Link aus.
2. Wählen Sie eine Zeile für ein Sachkonto aus, für dessen Sachposten Sie gebuchte Einkaufs- und Verkaufsbelege abrufen möchten, zu denen keine Eingangsbelege vorhanden sind, und wählen Sie dann die Aktion **Gebuchte Belege ohne Eingangsbeleg**.
3. Wählen Sie die Aktion **Ledger Entries** aus.
4. Wählen Sie im Fenster **Sachposten** die Aktion **Gebuchte Belege ohne Eingangsbelege** aus.

Daraufhin wird das Fenster **Gebuchte Belege ohne Eingangsbeleg** geöffnet, das die gebuchten Einkaufs- und Verkaufsbelege ohne zugehörige Eingangsbelege enthält, die von Sachposten auf dem Sachkonto dargestellt werden, für das Sie das Fenster geöffnet haben. Das Fenster kann maximal 1000 Zeilen anzeigen. Standardmäßig enthält das Feld **Datumsfilter** daher einen Filter, der die Anzeige auf Einträge beschränkt, deren Buchungsdatum zwischen dem Beginn der Buchhaltungsperiode und dem Arbeitsdatum liegt.

## <a name="to-connect-found-documents-to-existing-incoming-document-records"></a>So verknüpfen Sie gefundene Dokumente mit vorhandenen Eingangsbelegen
1. Wählen Sie im Fenster **Gebuchte Belege ohne Eingangsbeleg** die Zeile für einen gebuchten Beleg aus, den Sie mit einem vorhandenen Eingangsbeleg verknüpfen möchten, und wählen Sie dann die Aktion **Eingehenden Beleg auswählen** aus.
2. Wählen Sie im Fenster **Eingehende Belege** den Eingangsbeleg aus, den Sie der gefundenen Buchung zuordnen möchten, und klicken Sie anschließend auf die Schaltfläche **OK**.
3. Im Fenster **Gebuchte Belege ohne Eingangsbeleg** wird der gewählte Eingangsbeleg nun mit dem gebuchten Beleg verknüpft und in der InfoBox **Eingehende Belegdateien** angezeigt.

Wenn das Fenster **Eingehende Belege** keinen relevanten Eingangsbeleg-Datensatz enthält, können Sie einen erstellen. Weitere Informationen finden Sie unter [So gehts: Eingehende Dokumente erstellen](across-how-create-income-document-records.md).

## <a name="see-also"></a>Siehe auch
[Eingehende Dokumente verarbeiten](across-process-income-documents.md)  
[Eingehende Belege](across-income-documents.md)  
[Einkauf](purchasing-manage-purchasing.md)  
[Arbeiten mit [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

