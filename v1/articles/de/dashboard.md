## Dashboard



Das Dashboard bietet einen Überblick über Ihre Produktvarianten und die zugehörigen GTINs sowie Tools für deren effiziente Verwaltung. Von dieser zentralen Stelle aus können Sie GTINs zuweisen, verfolgen und verwalten, ihren Status einsehen und Massenaktionen durchführen.

**GTIN-Status und -Verwaltung**

Die Seite **GTIN-Status** bietet Ihnen eine detaillierte Übersicht über die Ihren Produktvarianten zugewiesenen GTINs. Sie können Varianten nach GTIN-Status filtern, um Ihren Bestand einfach zu verwalten und die Einhaltung der GS1-Standards sicherzustellen.

 **Statusfilter:** Nutzen Sie die Filteroptionen, um zwischen verschiedenen Status zu navigieren:

&nbsp;&nbsp; **Zugewiesen:** Zeigt Produkte an, denen gültige GTINs zugewiesen sind.

**Nicht zugewiesen:** Zeigt Produkte an, denen noch keine GTIN zugewiesen ist.

 **Gültig:** Zeigt GTINs an, die das erforderliche Format aufweisen und den GS1-Standards entsprechen, sodass sie auf allen unterstützten Plattformen verwendet werden können.

**Ungültig:** Hebt alle GTINs hervor, die nicht dem erforderlichen Format oder den GS1-Standards entsprechen.

**Duplikate:** Zeigt alle GTINs an, die in verschiedenen Varianten dupliziert sind.

**GTIN-Sperrstatus:** Zusätzlich zum Produktstatus.

 **Verfügbar:** Zeigt die Gesamtzahl der verbleibenden GTINs im konfigurierten Firmenpräfixblock an, sodass Sie den Überblick darüber behalten, wie viele GTINs noch zugewiesen werden können.

&nbsp;&nbsp;**Ausstehend Shopify:** GTINs, die zugewiesen wurden, sich aber noch im Prozess der Synchronisierung oder Annahme durch Shopify befinden.

 &nbsp;&nbsp; **Ausstehend GS1:** Zur Validierung übermittelte GTINs, die auf Bestätigung oder Verifizierung durch GS1 warten.

 &nbsp;&nbsp;**Downloads:** GTINs, die zur Verwendung in externen Systemen oder Aufzeichnungen exportiert oder heruntergeladen wurden.

**Manuelle und automatische Aktualisierung**

Das Dashboard zeigt den Zeitpunkt der letzten Aktualisierung der GTIN-Daten an, sodass Sie die letzten Änderungen verfolgen können. Eine manuelle Aktualisierung kann über die Schaltfläche „Aktualisieren“ oben im Dashboard ausgelöst werden.

 &nbsp;&nbsp;**Automatische Aktualisierung:** Nach jeder Aktion, z. B. dem Zuweisen oder Aufheben der Zuweisung von GTINs, wird das Dashboard automatisch aktualisiert, um den aktualisierten Produktstatus anzuzeigen.

&nbsp;&nbsp;**Manuelle Aktualisierung:** Bei Bedarf können Sie die Seite jederzeit manuell über die Schaltfläche „Aktualisieren“ aktualisieren, um den Status und die Produktliste zu aktualisieren.

**Hinweis:** Bei Geschäften mit einer großen Anzahl von Produkten kann der Aktualisierungsvorgang je nach Größe Ihres Katalogs einige Zeit in Anspruch nehmen.

**Katalogstatus:**

&nbsp;&nbsp;Die Spalte „Status“ zeigt an, ob die GTIN des Produkts im GS1-Katalog vorhanden ist.

&nbsp;&nbsp;**GTIN-Status:** Gibt den Validierungsstatus der GTIN (Global Trade Item Number) gegenüber dem GS1 Global Data Synchronization Network an (GDSN)

&nbsp;&nbsp;**Verifiziert:** Gibt an, ob die GTIN des Produkts und die zugehörigen Attribute (Marke, Beschreibung usw.) durch den Dienst „Verified by GS1“ validiert wurden

![screenshot:Dashboard](Dashboard.png)

**GTINs zuweisen und aufheben**

Das Dashboard ermöglicht Ihnen die Zuweisung und Aufhebung von GTINs direkt aus der Variantenliste. Sie können dies einzeln oder in großen Mengen tun, was die Verwaltung großer Produktkataloge erleichtert.

**1. Individuelle GTIN-Zuweisung:**

&nbsp;&nbsp;Neben jeder Produktvariante sehen Sie die Schaltfläche „GTIN zuweisen“. Klicken Sie auf diese Schaltfläche, um dieser Variante manuell eine GTIN zuzuweisen.

![screenshot:GTINS zuweisen](AssignGTINs.png)

**2. Massenzuweisung und -aufhebung von GTINs:**

&nbsp;&nbsp;Sie können GTINs für mehrere Produkte gleichzeitig zuweisen oder deren Zuweisung aufheben:

&nbsp;&nbsp;Wählen Sie mehrere Produktvarianten aus, indem Sie die Kontrollkästchen daneben aktivieren.

&nbsp;&nbsp;Klicken Sie oben in der Liste auf die Schaltfläche **Zuweisen**, um allen ausgewählten Varianten automatisch verfügbare GTINs zuzuweisen.

&nbsp;&nbsp;Um GTINs zu entfernen, verwenden Sie die Schaltfläche **Aufheben**, um die Zuweisung von GTINs zu den ausgewählten Varianten aufzuheben.

![screenshot:Massen-GTINS](BulkAction.png)

**Filtern und Suchen nach Varianten**

Das Dashboard enthält erweiterte Filter- und Suchoptionen, mit denen Sie schnell bestimmte Produktvarianten finden:

&nbsp;&nbsp;**Suchleiste (Varianten filtern):** Sie können das Suchfeld verwenden, um Schlüsselwörter, Produkttitel oder GTINs einzugeben Variantenliste. Mit dieser Funktion können Sie Produkte schnell nach Name, Beschreibung oder anderen relevanten Daten filtern. Wenn Sie beispielsweise „neu“ in die Suchleiste eingeben, wird die Liste so gefiltert, dass nur Produkte angezeigt werden, deren Titel oder Details „neu“ enthalten.

**Statusfilter:**Verwenden Sie die Statusfilter (Zugewiesen, Nicht zugewiesen, Duplikate, Gültig, Ungültig), um die Liste der auf dem Dashboard angezeigten Produkte zu verfeinern.

![screenshot:Filters GTINS](SearchingFilters.png)

**Synchronisierung mit Ihrem GS1-Katalog**

Sie können Ihre Produkte auf zwei Arten mit Ihrem GS1-Katalog synchronisieren:

&nbsp;&nbsp;**1. Direktverbindung:** 

&nbsp;&nbsp; Wenn Sie eine Direktverbindung mit Ihrer GS1-Einheit (z. B. GS1 Deutschland) konfiguriert haben, werden Ihre Produkte automatisch mit dem GS1-Katalog synchronisiert.

&nbsp;&nbsp;**2. Exportieren und Importieren:** 

&nbsp;&nbsp; Sie können Produktdaten auch aus dem GS1 Assistant exportieren und manuell in Ihren GS1-Katalog importieren. Die App unterstützt derzeit Exportformate für **GS1 USA** und **GS1 Deutschland**.

&nbsp;&nbsp;Wenn Ihre Region noch nicht unterstützt wird und Sie bei der Erweiterung der Funktionalität auf zusätzliche GS1-Einheiten helfen können, wenden Sie sich bitte an uns.

![screenshot:GTINS herunterladen](DownloadModel.png)
