Bei diesem Aufgabentyp können natürlich auch andere Eigenschaften von Histogrammen gefragt sein. Eine andere Variante besteht darin, aus einem gegebenen Histo- gramm Eigenschaften zu definieren. Weiterer Aufgabentyp: Histogramm aus Bild errechnen oder Histogrammebnung berechnung, siehe Beispiele aus der Vorlesung
- Punktoperationen
	- Operationen wo der neue Farbwert eines Bildpunkts nur von ursprünglichen Wert und evtl. Position abhängt. Also keine Infos von benachbarten Bildpunkten
	- homogene transformation
		- unabhängig von Lage im Bild
	- inhomogene transformation
		- hängt auch von Lage in Bild ab
- Grauwerthistogramm
	- ![[Pasted image 20250205140636.png]]
	- Eine Häufigkeitsverteilung der Grauwerte im Bild
	- zeichnen können anhand Tabelle h(x)
		- ![[Pasted image 20250205134601.png]]
	- Kummulative Verteilungsfunktion H(x)
		- ![[Pasted image 20250205134706.png]]
- kummulatives Histogramm
	- ![[Pasted image 20250205140655.png]]
- Dynamik 
	- ist die anzahl verschiedener Grauwerte im Bild
	- hohe dynamik -> viele unterschiedliche farben, ist besser
	- ![[Pasted image 20250205131915.png]]
- Kontrast
	- is der effektiv genutzte Bereich von Grauwerten
	- ![[Pasted image 20250205131926.png]]
- Belichtung
	- Fehler: Ende der Grauwertskala ungenutzte bereiche während am anderen ende eine Häufung auftritt
	- ![[Pasted image 20250205132048.png]]
- was tun wenn zu wenig kontrast?
	- Histogrammanpassung
- schwellwert-operation, wofür eingesetzt
	- Segmentierung, z.B. Binarisierung
	- Werte oberhalb eines Schwellwerts werden auf 1 gesetzt, andere 0
- shading korrektur, wie wird durchgeführt
	- Ortsabhängige Grauwerttransformation
	- Kompensation örtlich Inhomogener Beleuchtungseinflüsse
	- Durchführung
		- Referenzbild mit konstanter Reflektion aufnehmen (fref)
		- Original mit hilfe des Referenzbild korrigieren
- Auto-Kontrast Erläutern
	- Vorgehen erläutern
	- Vor und Nachteile
- Histogrammebnung erläutern
	- Grauwerte möglichst gleichmäßig über gesamten zur verfügung stehenden Wertebereich verteilen
	- Grauwerte wo cumm Verteilungsfunktion stark ansteigt werden auseinander gezogen
	- Annähernd Gleichverteilung herstellen, klassischer Ausgleich
		- ![[Pasted image 20250205140519.png]]
	- Grauwerte entsprechend kumm. Verteilungsfunktion ausdehnen. 0 wird auf 0 abgebildet
		- ![[Pasted image 20250205140614.png]]
- transformationskennlinien
	- Ortsunabhängige Grauwerttransformation
	- geht auch als LUT
	- Invertierung umsetzbar, unterbelichtung korrigierbar, ...
	- ![[Pasted image 20250205133645.png]]
	- Korrektur unterbelichtung
		- ![[Pasted image 20250205133707.png]]
	- Kontrastverstärkung
		- ![[Pasted image 20250205134225.png]]
	- um Bereich hervorzuheben
		- ![[Pasted image 20250205135512.png]]
- XOR zweier binärer Bilder
	- Erkennen von Unterschieden, gleiche pixel werden ausgeblendet.
	- Kann für Bewegungserkennung und Bildmaskierung eingesetzt werden
- Subtraktion zweier Bilder
	- Änderungsdetektion
	- Betragsbildung für Erhalt des Wertebereichs 
	- Verstärkt Grauwertdifferenzen
!! Immer Achsenbeschriftungen angeben, sonst ist es ein fehler !!

![[Pasted image 20250205115921.png]]
- ergänzt

![[Pasted image 20250205115939.png]]
- ergänzt

![[Pasted image 20250205115950.png]]
- ergänzt

![[Pasted image 20250205120003.png]]
- ergänzt

![[Pasted image 20250205120014.png]]
- ergänzt 

![[Pasted image 20250205120026.png]]
- ergänzt

![[Pasted image 20250205120037.png]]
- ergänzt

![[Pasted image 20250205120047.png]]
- ergänzt
![[Pasted image 20250205120442.png]]
- ergänzt