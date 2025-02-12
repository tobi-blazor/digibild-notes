- Zweck Segmentierung
	- Trennung von räumlichen/homogenen Bereichen eines Bildes, Klassifikation
- Wie Kantenbilder erzeugt
	- Canny Algorithmus
		- 1. Glättungsfilter 2. Gradientenfilter 3. Non-Maxima-Unterdrückung 4. Doppelter Schwellwert 5. Verkettung
- Zweck und Funktion OTSU
- Konturpunktverkettung
	- ![[Pasted image 20250207165204.png]]
	- einfach, schnell, kette kann in mehrere teile zerfallen, entspricht ggf. nicht Gradientenrichtung +pi/2
- Wie Konturpunktdetektion für Segmentierung funktioniert
- ! Ablauf Kontursegmentierung von Ursprungsbild zu Repräsentation der Objektränder durch Liste von Strecken
	- Hervorhebung von Grauwertdifferenzen in horizontaler und vertikaler Richtung (kartesische Darstellung) durch Gradientenoperation.
	- Wandlung der kartesischen Darstellung des Ergebnisses in polare Darstellung ergibt Betrag und die Richtung der jeweils größten Grauwertänderung.
	- Gradientenoperatoren „verschmieren“ die Kontur aufgrund ihres Tiefpassverhaltens.
	- Aufbesserung der Kontur erreicht man durch ihre Verdünnung, so dass ein Gradientenbild mit 1 Pixel breiten Linien entsteht.
	- Verkettungsverfahren sammelt benachbarte Konturpunkte auf und bildet daraus eine Kette.
	- Die Verkettung von Konturpunkten realisiert die Zusammenhangsanalyse für die Kontursegmentierung.
	- Das Verkettungsverfahren liefert Listen der Koordinaten der verketteten Konturpunkte.
	- Der letzte Verfahrensschritt approximiert die durch die Konturpunktketten repräsentierten Konturen durch Strecken. 
	- Am Ende des Verfahrens steht also eine Liste von Strecken in Form der Koordinaten ihrer Endpunkte.
- Region Growing bei Segmentierung vorteile, nachteile
	- Aufteilung des Bildes in Zonen maximaler Homogenität (z.B. ähnliche Intensitäten)
	- ausgehend von n-Ursprungspixel werden andere Pixel die Homogenitätskriterium erfüllen aggregiert
	- nachbarschaftsinfo mit einbezogen, robus tbei verrauschung, Umsetzung in 3D einfach
	- Modellwissen schwerer mit einzubeziehen, startpunkt/region ist vorzugeben, auslaufen ist möglich
- 

![[Pasted image 20250205122828.png]]
j
![[Pasted image 20250205122843.png]]
j
![[Pasted image 20250205122913.png]]
j
![[Pasted image 20250205122933.png]]
j
![[Pasted image 20250205122941.png]]
j
![[Pasted image 20250205122948.png]]
j
![[Pasted image 20250205123009.png]]
j
![[Pasted image 20250205123018.png]]
y
![[Pasted image 20250205123027.png]]
y