# Railway-CAN
Ziel des Projekts ist es eine analog betriebene Modelleisenbahn sie zu steuern, dass ein weitgehend vorbildlicher Betrieb erreicht wird. Weichen, Signale und Fahrstraßen bedient das Stellwerk, Einer Lokomotive wird von einem Lokführer gesteuert. Die befahrenen Gleisabschnitte werden dabei vom System geschalten.

Um nicht von zukünftigen Updates und Betriebssystemwechseln auf Computern anhängig zu sein, soll die gesamte Steuerung mit den Bausteinen von Teilen-CAN abgedeckt sein. Ich greife dabei auf die Erfahrungen aus dem Loco-CAN Projekt zurück, dass eine ähnliche Hardware verwendet.

Der Aufbau und die Verkabelung der Anlage, sowie die nötigen Programmierschritte sollten für jeden Modellbahner umsetzbar sein, ohne Programmierkenntnisse. Da das gesamte Projekt, Hard- wie Software, open source ist, können jederzeit Module für Erweiterungen nachgefertigt werden. 

## Aufbau
Das System besteht aus dem Anlagenmodulen, dem Stellpult, Fahrpultenund der Zentrale.

Je nach existierender Verkabelung können die Anlagenodule direkt auf der Anlage verlegt werden oder beim bisherigen Stellpult. Wichtig ist, dass Kabel zu den Schienen, den Weichen und Signalen mit den Modulen verbunden werden müssen. Bei einer Neuverkabelung ist es ratsam die Module unter der Anlage anzubringen. Alle Module Museum an eine Versorgung-Ringleitung angeschlossen werden, die von einem Netzteil für die gesamte Anlage gespeist wird. Es ist auch möglich bei großen Anlagen mehrere Netzteile für Anlagenteile zu verwenden, es muss dann der Minuspol aller Netzteile verbinden werden.

Das Stellpult ist ein physisch aufgebautes Spurplanstellwerk der Type Siemens SP Dr S60. Es beinhaltet alle Bedienelemente zum Stellen der Weichen, Signale, Schranken und Fahrstraßen. Die Verkabelung der einzelnen Blöcke ist ganz einfach, werden sie lediglich mit einem vierpoligen Kabel untereinander verbunden. Die letzte Verbindung läuft zur Zentrale.

