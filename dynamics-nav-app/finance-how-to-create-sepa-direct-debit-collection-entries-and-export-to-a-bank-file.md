---
title: SEPA-Lastschrift
description: "Speichert die Posten für die Lastschrift in einer XML-Datei, die Sie zur Verarbeitung an die elektronische Bank senden oder hochladen."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct-debit, collection, payment, sepa
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6071991197182b13894bd5b0cb5be3d06e967a29
ms.contentlocale: de-de
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-sepa-direct-debit-collection-entries-and-export-to-a-bank-file"></a>Vorgehensweise: SEPA-Lastschrifteinzugsposten erstellen und in eine Bankdatei exportieren
Um die Bank anzuweisen, den Zahlungsbetrag vom Bankkonto des Debitors auf das Bankkonto Ihres Unternehmens zu überweisen, erstellen Sie einen Lastschrifteinzug mit Informationen zum Bankkonto des Debitors, den betroffenen Verkaufsrechnungen und dem Lastschrift-Mandat. Aus dem resultierenden Lastschrifteinzugsposten können Sie dann eine XML-Datei exportieren, die Sie dann zur Verarbeitung an Ihre elektronische Bank senden oder hochladen. Alle Zahlungen, die von der Bank nicht verarbeitet werden konnten, werden Ihnen von Ihrer Bank mitgeteilt, und Sie müssen dann die jeweiligen Lastschrifteinzugsposten manuell ablehnen.  

> [!NOTE]  
>  Um Zahlungen mithilfe von SEPA-Lastschrift zu erfassen, muss die Währung der Verkaufsrechnung EURO sein.  

### <a name="to-create-a-direct-debit-collection"></a>Erstellen eines Lastschrifteinzugs  
1. Wählen Sie ![Nach Seite oder Bericht suchen](media/ui-search/search_small.png "Nach Seite oder Berichtsymbol suchen") und geben **Lastschriften** ein und wählen dann den zugehörigen Link aus.  
2. Wählen Sie im Fenster **Lastschriften** auf der Registerkarte **Start** in der Gruppe **Neu** die Option **Lastschrifteinzug erstellen** aus.  
3. Füllen Sie im Fenster **Lastschrift erstellen** die Felder gemäß der Beschreibung in der folgenden Tabelle aus.  

    |Feld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Ab Fälligkeitsdatum**|Geben Sie das früheste Zahlungsfälligkeitsdatum auf Verkaufsrechnungen an, für das Sie einen Lastschrifteinzug erstellen wollen.|  
    |**Bis Fälligkeitsdatum**|Geben Sie das späteste Zahlungsfälligkeitsdatum auf Verkaufsrechnungen an, für das Sie einen Lastschrifteinzug erstellen wollen.|  
    |**Partnerart**|Geben Sie an, ob der Lastschrifteinzug für Debitoren des Typs **Unternehmen** oder **Person** erfolgt.|  
    |**Nur Debitoren mit gültiger Einzugsermächtigung**|Geben Sie an, ob ein Lastschrifteinzug für Debitoren erstellt wird, die über ein gültiges Lastschrift-Mandat verfügen. **Hinweis:** Eine Lastschrift wird auch erstellt, wenn das Feld **Lastschrift-Unternehmens-ID** auf der Vertriebsrechnung nicht ausgefüllt ist.|  
    |**Nur Rechnungen mit gültigem Lastschrift-Mandat**|Legt fest, ob ein Lastschrifteinzug nur dann für Verkaufsrechnungen erstellt wird, wenn im Feld **Lastschrift-Mandat-ID** auf der Verkaufsrechnung ein gültiges Lastschrift-Mandat ausgewählt ist.|  
    |**Bankkontonr.**|Geben Sie an, auf welches der Bankkonten Ihres Unternehmens die Eingangszahlung vom Bankkonto des Debitors überwiesen werden soll.|  
    |**Bankkontoname**|Gibt den Namen des Bankkontos an, das Sie im Feld **Bankkontonr.** auswählen. Dieses Feld wird automatisch ausgefüllt.|  

4. Wählen Sie die Schaltfläche **OK** aus.  

     Eine Einzugserfassung wird dem **Lastschrift**-Fenster hinzugefügt, und ein oder mehrere Lastschrifteinzugsposten werden erstellt.  

### <a name="to-export-a-direct-debit-collection-entry-to-a-bank-file"></a>Export eines Lastschrifteinzugpostens in eine Bankdatei  
1. Wählen Sie im Fenster **Lastschriften** auf der Registerkarte **Start** in der Gruppe **Verarbeiten** die Option **Lastschrifteinzug-Eintrag erstellen** aus.  
2. Wählen Sie im Fenster **Lastschrifteinzug-Eintrag** den Eintrag aus, den Sie exportieren möchten, und wählen Sie dann auf der Registerkarte **Start**, in der Gruppe **Verarbeiten**, **Lastschrift erstellen** aus.  
3. Speichern Sie die Exportdatei an dem Speicherort, von dem aus Sie sie an Ihre elektronische Bank senden oder hochladen.  

     Im Fenster **Lastschrifteinzug-Eintrag** wird das Feld **Status Lastschrift** zur erstellten Datei geändert. Im Fenster **SEPA-Lastschrift-Mandate** wird das Feld **Sollzähler** mit einer Anzahl aktualisiert.  

Wenn die exportierte Datei nicht verarbeitet werden kann, etwa weil der Kunde nicht mehr zahlungsfähig ist, können Sie den Lastschrifteinzugsposten ablehnen. Wenn die exportierte Datei von der Bank erfolgreich verarbeitet wird, werden die fälligen Zahlungen der beteiligten Verkaufsrechnungen von den beteiligten Kunden automatisch eingezogen. In diesem Fall können Sie die Erfassung schließen.  

### <a name="to-reject-a-direct-debit-collection-entry"></a>Ablehnen eines Lastschrifteinzugpostens  
* Wählen Sie im Fenster **Lastschrifteinzug-Eintrag** den Eintrag aus, der nicht erfolgreich verarbeitet wurde, und wählen Sie dann auf der Registerkarte **Start**, in der Gruppe **Verarbeiten**, **Eintrag ablehnen** aus.  

     Der Wert im Feld **Status**im Fenster **Lastschrifteinzug-Eintrag** wird auf **zurückgewiesen** geändert.  

### <a name="to-close-a-direct-debit-collection"></a>Schließen eines Lastschrifteinzugs  
* Wählen Sie im Fenster **Lastschrifteinzug-Eintrag** den Eintrag aus, der nicht erfolgreich verarbeitet wurde, und wählen Sie dann auf der Registerkarte **Start**, in der Gruppe **Verarbeiten**, **Lastschrift beenden** aus.  

     Der zugehörige Lastschrifteinzug wird geschlossen.  

Sie können jetzt Zahlungseingänge für die betreffenden Verkaufsrechnungen buchen. Sie können dies tun, wie Sie normalerweise Zahlungseingänge buchen, etwa im Fenster **Zahlungserfassung** oder Sie können die zugehörigen Zahlungseingänge direkt aus dem Fenster **Lastschrifteinzug-Eintrag** buchen. Weitere Informationen finden Sie unter [Vorgehensweise:  SEPA-Lastschrifteinzug-Zahlungseingänge buchen](finance-how-to-post-sepa-direct-debit-payment-receipts.md).  

## <a name="see-also"></a>Siehe auch  
[Vorgehensweise: Einrichten von SEPA-Lastschriften](finance-how-to-set-up-sepa-direct-debit.md)   
[Vorgehensweise: SEPA-Lastschrifteinzug-Zahlungseingänge buchen](finance-how-to-post-sepa-direct-debit-payment-receipts.md)   
[Einziehen von Zahlungen per Lastschriftverfahren SEPA](finance-collect-payments-with-sepa-direct-debit.md)   

