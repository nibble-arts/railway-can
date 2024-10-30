# Spurplanstellwerk Siemens SP Dr S60
## Aufbau
Das Stellwerk gibt das Vorbild weitgehend Original wieder. Es besteht aus Blöcken, die auf einer Grundplatine aufgesteckt werden. Die Gehäuse der Blöcke bestehen aus farblich unterschiedlich gedruckten 3D-Teilen, die zusammengesteckt, bzw. verklebt werden. Damit ist es möglich die graue (ider farbige) Grundplatte und die schwarzen Gleise robust und ohne Aufdruck zu realisieren.

Es gibt aktive Blöcke mit Tasten und LEDs, passive Blöcke nur mit einer Ausleuchtung und Blindplatten. Die aktiven Blöcke sind über einen CAN-Bus mit der Zentrale verbunden.

Die Blöcke haben an der Unterseite zwei Pfostenstecker, mit denen alle nötigen elektrischen Verbindungen hergestellt werden. Jeder Block wird mit +5 Volt versorgt und hängt an der gemeinsamen Busleitung.

Blöcke, die nur eine Ausleuchtung bieten, werden über Jumper auf der Grundplatine mit dem entsprechenden Block verbunden.

Die Grundplatten sind für einen Raster von fünf Blöcken horizontal und drei Blöcken vertikal vorgesehen und können beliebig nebeneinander angeordnet werden. Die elektrische Verbindung zwischen den Grundplatten wird durch Steckverbindungen hergestellte.

Für den Aufbau des Stellpultes sind keine Lötarbeiten nötig.

## Programmierung
Die Stellwerkblöcke und die entsprechenden Anlagenmodule werden über den CAN-Bus miteinander verbunden. Das beschränkt die Verkabelung auf je ein Buskabel zum Stellpult und zur Anlage.

Bevor die Blöcke im Stellwerk konfiguriert werden, sollten sie Anlagenmodule programmiert werden. Jedem Modul wird dabei eine anlagenweit einmalige Nummer zugewiesen.

Die Stellwerksblöcke müssen einmalig mit dem entsprechenden Anlagenmodul verbunden werden. Dazu muss im Block lediglich die entsprechende Modulnummer eingetragen werden.

Die Anlagenmodule und Stellwerkblöcke werden programmiert, indem sie in den Programmierplatz des Stellwerks gesteckt werden.

Zum Test wird das Anlagenmodul installiert und der Stellwerksblock in das Stellpult gesteckt. Sind die Module korrekt verbunden, leuchten nach dem Einschalten am Block alle LEDs für zwei Sekunde auf. Sollte keine Verbindung gefunden werden, blinken die LEDs in Sekundentakt. Dieser Test läuft bei jedem Einschaltvorgang der Anlage ab und signalisiert so mögliche Fehlfunktionen.
