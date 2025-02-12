### Was ist eine Segementierung:
- Trennung von räumlichen oder homogenen Bereichen innerhalb eines Bildes, Zuordnung zu einer Klasse (Klassifikation)

### Bereichorientierte Verfahren
- versucht Bildpunkte zu bestimmen, die zu den Bereichen gehören
- Region Growing
- Schwellenwertverfahren => OTSU

### Region Growing
Aufteilung des Bildes in Zonen max. homgenität
Startpunkt wählen -> Region wachsen durch nachbarpixel -> Stopp wenn keine weitern Pixel
- vorteil
	- nachbarschaftsinformation einbezogen
	- robust gegen rauschen
	- umsetzung 3d einfach
- nachteil
	- modellwissen schwerer mit einzubeziehen
	- startpunkt ist vorgegeben
	- auslaufen möglich => Barriere zur Vorbeugung

### Konturorientierte Verfahren
- versuchen Rand der Bereiche zu bestimmen
- Gradientenoperatoren
- Vorteile
	- datenreduktion
	- strukturelle Beschreibung

### Gradientenoperator
Gradient => Richtung des stärksten Grauwertanstiegs
Sobel/Prewitt wird benutzt um die partielle Ableitungen zu bilden (vertikal/horizontal) => Betrag und Winkel wird bestimmt => zweite Ableitung Laplace für Stärke der Kanten

| **Operator** | **Mathematische Grundlage** | **Vorteile**                             | **Nachteile**                  |
| ------------ | --------------------------- | ---------------------------------------- | ------------------------------ |
| **Sobel**    | Erste Ableitung             | Richtungssensitiv, robust gegen Rauschen | Kanten sind oft dick           |
| **Prewitt**  | Erste Ableitung             | Ähnlich wie Sobel, aber einfacher        | Weniger genau als Sobel        |
| **Laplace**  | Zweite Ableitung            | Findet Kanten unabhängig von Richtung    | Empfindlich gegenüber Rauschen |

### Ablauf Kontursegmentierung von Ursprungsbild zu Repräsentation der Objektränder durch Liste von Strecken
- Hervorhebung von Grauwertdifferenzen in horizontaler und vertikaler Richtung (kartesische Darstellung) durch Gradientenoperation.
- Wandlung der kartesischen Darstellung in polare Darstellung ergibt Betrag und die Richtung der jeweils größten Grauwertänderung.
- Aufbesserung der Kontur durch Verdünnung, so dass Gradientenbild mit 1 Pixel Linien entsteht => Non-Maxima Unterdrückung
- Verkettungsverfahren sammelt benachbarte Konturpunkte auf und bildet Kette.
- Zusammenhangsanalyse realisiert die Verkettung von Konturpunkten für die Kontursegmentierung.
- Verkettungsverfahren liefert Listen der Koordinaten der verketteten Konturpunkte.
- letzter Verfahrensschritt approximiert die Konturen durch Strecken. 
- Ende des Verfahrens steht Liste von Strecken in Form der Koordinaten ihrer Endpunkte.

### Non-Maxima-Unterdrückung
- Pixel links und rechts der lokalen Maxima muss entfernt werden
- Lage des linken und rechten Nachbarn orientiert sich an Gradientenrichtung des aktuellen Pixels

### Konturpunktverkettung
![[Pasted image 20250207165204.png]]
Problem: können in einzelne ketten zerfallen => Man geht ans Ende der Kette und geht Rückwärts

### Canny-Algorithmus
- detektiert Kanten in einem Bild
- Glättungsfilter mit Gauß
- Gradientenfilter mit Sobel (deshalb vorher glättung)
- Non-Maxima-Unterdrückung
- Doppelter Schwellwert => zwei Schwellenwerte um schwache und starke Kanten zu haben
- Verkettung (schwache Kanten verbunden mit starke über 8ter-Nachbar)
