## Konfiguration



Der erste Schritt bei der Verwendung der GS1 Assistant App ist die Konfiguration der Einstellungen, die bestimmen, wie Ihre GTINs zugewiesen und verwaltet werden.

Dieser Abschnitt führt Sie durch die Verwaltung des Firmenpräfixes und die Konfiguration der App-Sprache.

![screenshot:Erste Schritte](GetStarted.png)

 **Firmenpräfix verwalten**

 Verwenden Sie Ihr eigenes, von GS1 zugewiesenes globales Firmenpräfix (GPC), um GTINs zu generieren.

Ein Firmenpräfix wird zugewiesen, wenn Sie Barcodes über GS1 kaufen.

Dazu müssen Sie Ihr GCP eingeben, das GTIN-Format (UPC/EAN/GTIN-14) angeben und den Bereich der zu verwendenden GTINs konfigurieren.

![screenshot:Firmenpräfix verwalten](ManageCompanyPrefix.png)

![screenshot:Neues Firmenpräfix](NewCompanyPrefix.png)

 **GS1-Firmenpräfix aktualisieren**

Sie können ein vorhandenes Firmenpräfix, um bestimmte Bereiche für GTINs festzulegen, die Ihren Produkten zugewiesen werden sollen

1. Öffnen Sie den GS1-Konfigurationsbildschirm:**

 Klicken Sie in der Liste neben dem Firmenpräfix, das Sie aktualisieren möchten, auf die Schaltfläche „Bearbeiten“. 

 **2. Firmenpräfix und Blockgröße:**
Die Felder „Firmenpräfix“ und „Blockgröße“ sind vorausgefüllt und schreibgeschützt. Diese Felder zeigen das Präfix und die Größe des zugewiesenen Blocks an und können nach der Erstkonfiguration nicht mehr geändert werden. 

 **3. Sequenzbereiche:** Sie können optional Sequenzbereiche für GTIN-Zuweisungen definieren. Diese Bereiche geben die Reihenfolge oder Sequenz an, in der GTINs den Produktvarianten aus Ihrem Firmenpräfixblock zugewiesen werden. Beachten Sie, dass die Sequenzbereiche nicht die eigentlichen GTIN-Nummern, sondern die internen Sequenzpositionen innerhalb des Blocks darstellen. 

&nbsp;&nbsp; **Start:** Geben Sie die Startsequenznummer ein. Dies ist die erste Position im Firmenpräfixblock, ab der mit der GTIN-Zuweisung begonnen wird. 

&nbsp;&nbsp; **Ende:** Geben Sie die Endsequenznummer ein. Dies ist die letzte Sequenzposition, die für GTIN-Zuweisungen verwendet wird.

![screenshot:Präfix wird aktualisiert](UpdatingPrefix.png)

 **Verbindung zu GS1 wird hergestellt**

Sie können die App mit Ihrem GS1-Konto verbinden, um Firmenpräfixe und GTIN-Zuweisungen zu synchronisieren. Nach der Verbindung werden die in Ihrem GS1-Konto gespeicherten Präfixe automatisch in die App übernommen.

**1. Mit GS1 verbinden:**

Klicken Sie auf die Schaltfläche „Mit GS1 verbinden“, um den Vorgang zu starten. Sie müssen ein API-Token von Ihrer GS1-Einheit generieren, um die Verbindung herzustellen.

**2. Firmenpräfixe synchronisieren:**

Nach der Verbindung werden Ihre Firmenpräfixe mit Ihrem GS1-Konto synchronisiert. In der Statusspalte wird angezeigt, ob jedes Präfix im GS1-Katalog vorhanden ist.

 **Hinweis:** Der Synchronisierungsvorgang überschreibt nicht Ihre lokalen Konfigurationen, sondern synchronisiert nur neue Daten von GS1.

![screenshot:PrefixGrid](PrefixGrid.png)

![screenshot:Connect GS1](ConnectGS1.png)

**GS1-Standardeinstellungen**

 In diesem Abschnitt können Sie Standardproduktinformationen für die Zuweisung von GTINs (Global Trade Item Numbers) festlegen. Diese Werte helfen dabei, Ihre Produktlisten in GS1-kompatiblen Systemen und Marktplätzen zu standardisieren.

![screenshot:GS1-Standardwerte](GS1Defaults.png)
