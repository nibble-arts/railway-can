# Persistance
Die Grundeinstellungen der Stellwerksblöcke und Anlagemodule ist auch ohne Stromversorger jeweils lokal dauerhaft gespeichert. Die Betriebsdaten, wie die Zuordnung von Zugnummern oder die Position von Zügen, liegen nur vor, wenn die Anlage mit Strom versorgt wird.

Alle Anlagenmodule senden ihren Status, sobald sich etwas verändert, an die Zentrale und damit das Stellwerk. Mindestens alle zehn Sekunden wird der Status auch ohne Änderung übertragen. Der gesamte Anlagenstatus wird damit laufend in der Zentrale gesammelt.

Die Zentrale verfügt über einen Pufferakku, der sie für eine Minuten versorgen kann, wenn die Netzversorgung ausfällt. Sie erkennt eine Stromunterbrechung und schreibt den aktuell Status in einen nichtflüchtigen Speicher. Das erfolgt auch bei einem Stromausfall.

Sobald die Anlage wieder einschalten wird, überträgt die Zentrale den letzten gespeicherten Status auf die Module. Die Freimelder liefern zusätzlich den aktuellen Zustand eines Gleisabschnitts. 

Die Fahrspannungen bleiben auf Null und müssen erst durch eine Nullstellung am Fahrpult aktiviert werden. Gestellte und teilweise abgefahrene Fahrstraßen bleiben verschlossen. Fahrstraßen, die nur beantragt wurden, werden nicht wiederhergestellt.

Wenn sich im ausgeschalteten Zustand die Belegung der Gleise nicht verändert hat, kann der Betrieb ohne zusätzliche Handlung einfach wieder aufgenommen werden.

Hat sich etwas verändert, müssen die Zugnummern neu vergeben werden. Über einen zentralen Reset können alle Zugnummernzuornungen gelöscht werden.
