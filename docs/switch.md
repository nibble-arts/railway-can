# Weiche
Weichen bilden ein eigenen Abschnitt und müssen auf allen Seiten elektrisch isoliert sein. Für Fahrspannung wird durch das Weichenmodul erzeugt.

Ein Freimeldesensor dient dazu ein Umstellen unter Fahrzeugen zu verhindern und Fahrstraßen, nachdem sie durchfahren wurden, automatisch auflösen zu können. 

Werden zwei zusätzliche Sensoren in den zulaufenden Gleisen installiert, kann ein Aufschneiden erkannt und gemeldet werden.

Das Modul kann sowohl Weichenantriebe mit Magneten, als auch mit Modebauservos ansteuern. Im zweiten Fall können die Endlagen und die Umstellzeit programmiert werden.

## Switch status
- valid: in correct end position
- running: moving to new positions
- timeout: end position not reached in time
- split: switch was split, can be solved by confirm, switching position or timeout (depends on setting)

## Hardware
- Section controller (see RC-section)
- occupation sensor (area of switch rails)
- split sensors (on incoming tracks)
- solenoid driver (2x FET)
- servo driver (5V supply)
- frog polarization (2x FET)
