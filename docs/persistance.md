# Persistance
Die Grundeunstellungen der Stellwerksblöcke und Anlagemodule ist auch ohne Stromversorger jeweils lokal dauerhaft gespeichert. Die Betriebsdaten, wie die Zuordnung von Zugnummern oder die Position von Zügen, liegen nur für, wenn sie Anlage mit Strom versorgt wird.

Alle Anlagenmodule senden ihren Status, sobald sich etwas verändert. Mindestens alle zehn Sekunden wird der Status auch ohne Änderung übertragen. Der gesamte Anlagenstatus wird si in der Zentrale abgelegt.

Die Zentrale verfügt über einen Pufferakku, der sie für eine Minuten versorgen kann, wenn die Netzversorgung ausfällt. Wird das System ausgeschaltet, wird der aktuell Status von der Zentrale in einem nichtflüchtigen Speicher geschrieben. Das erfolgt auch bei einem Stromausfall.

Sobald die Anlage wieder einschalten wird, überträgt die Zentrale den letzten gespeicherten Status auf die Module. Die Freimelder liefern in jedem Fall den aktuellen Zustand eines Gleisabschnitts. Die Fahrspannung bleiben alle auf Null und müssen erst durch eine Nullstellung am Fahrpult aktiviert werden.

Wenn sich im ausgeschalteten Zustand die Belegung der Gleise nicht verändert hat, kann der Betrieb ohne zusätzliche Handlung einfach wieder aufgenommen werden.

Hat sich etwas verändert, müssen die Zugnummern neu vergeben werden. Über einen zentralen Reset können alle Zugnummernzuornungen gelöscht werden.
