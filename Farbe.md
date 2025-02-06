- Farbhistogramm
	- linker wert ist x, rechter wert ist y
	- alle werte durchgehen und als strichliste eintragen
- Medianschnitt
	- farbhistogramm bestimmen
	- Hülle erstellen (quader)
	- wiederholen bis die Liste k Quader enthält
		- quader mit meisten farben aussuchen
		- freie farben entlang längster kante in gleich große teilmengen
	- für jedes Quader $\frac{summeSpalte*xWert+summeSpalte_n*xWert_n}{summeDerWerte}$

- Octree
	- Datenstruktur ist ein Baum mit bis zu 8 Kindern
	- Definiert hierarchische Zerlegung des RGB Baums in Würfel abnehmender Größe
	- Jeder Knoten enthält RGB Wert und Zähler wie oft Wert aufgetreten ist.
	- Übersteigt die ANzahl der Blattknoten den Wert K, werden die Blattknoten zu neuem verschmolzen (RGB und und zähler addiert)
	- Am Ende enhält der Octree höchstens k Blattknoten
	- RGB Werte der Blattknoten werden in Farbtabelle übertragen
	- 
- CIE Normalvalenzsystem
- Modell der Farbwahrnehmung im menschl. Auge, stärken, schwächen
- Farbbild in Graustufe wandeln
	- HSI und den Intensitätskanal auswählen
	- oder R G und B Kanal mit Faktor multiplizieren und dann addieren
- Aufbau von HSI Farbraum, Einsatzzweck
	- Klassisches mischen von Farben
	- Hue (farbton)
	- Saturation (Sättigung)
		- weißanteil, reinheit der Farbe beeinflusst
	- Intensität (Helligkeit)
		- schwarzanteil
	- Ideal für Bildverbesserung Operationen, weil Helligkeit von Farbe entkoppelt ist
- Populatity Algorithmus
	- Häufigste auftretende Farben werden übernommen
	- schlechte quali wenn selten auftretende farben wichtig sind
	- zeitaufwendig
- Lookup Tables, Farbraumtabellen
	- zur Datenreduktion, Performance Gründe
	- Im Bild ist verweis auf LUT mit Index, welche Farbe benutzt werden soll
- Fehlfarben Darstellung
	- Schwarz weiß (ct, MRT) Bild einfärben, weil das intiutiver ist
	- Temperatur als Farbe Farstellen
![[Pasted image 20250205121432.png]]

![[Pasted image 20250205121850.png]]
check
![[Pasted image 20250205121439.png]]
check
![[Pasted image 20250205121558.png]]
check
![[Pasted image 20250205121617.png]]
check
![[Pasted image 20250205121625.png]]
check
![[Pasted image 20250205121635.png]]
ye

![[Pasted image 20250205121645.png]]
ye
![[Pasted image 20250205121657.png]]
ye
![[Pasted image 20250205121718.png]]
jo
![[Pasted image 20250205121728.png]]
ye