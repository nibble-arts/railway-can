# Section controller
Es gibt keine zentralen Fahrregler, vielmehr wird die Fahrspannung für jeden Abschnitt der Anlage vom entsprechenden Anlagenmodul erzeugt. Man könnte sagen, es gibt so viele Fahrregler, wir isolierte Abschnitte in der Gleisanlage.

Der gewünschte Fahrstrom wird mit dem Fahrpult vorgegeben, das auf die Zugnummer eingestellt ist. Der Wert wird über den CAN-Bus an die Anlagenmodule gesendet, die den Fahrstrom einstellen.

Ist einem Abschnitt keine Zugnummer zugewiesen, ist er stromlos. Abschnitte, die die gleiche Zugnummer besitzen, werden auf das gleiche Niveau eingestellt. Damit ist gewährleistet, das z.B. vor einem Halt zeigenden Signal nicht nur der Signalabschnitt, sondern auch der gesamte Abschnitt davor herunter geregelt wird und selbst ein schiebender Zug an der korrekten Stelle anhält.

Der verwendete Motorregler-Baustein besitzt eine Stromüberwachung sowie einen internen Überlasschutz. Im Falle eines Kurzschlusses wird das betroffene Modul abgeschalten, sowie alle Abschnitte mit der gleichen Zugnummer auf 0 gestellt.

motor driver: DRV8801PWPR
