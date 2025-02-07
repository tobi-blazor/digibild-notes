- Glättungsfilter
	- Maske enthält nur werte >= 0
- Differenzfilter
	- Maske enthält mind. 1x Wert > 0 und Wert < 0
- Box
	- ![[Pasted image 20250205205142.png]]
	- Rauschen Redizieren
	- Steile Grauwertübergänge abgeflacht, Kanten unscharf
	- kann für glättung für segmentierung eingesetzt werden
	-  Tiefpass Filterung
	- "gewichtete summe der grauwerte"
- Median
	- nicht linear, Rangordnungsoperatoren
	- Alle Werte werden sortiert, und der mittlere wird gewählt (median)
	- rauschen reduzieren, steile grauwertübergänge bleiben erhalten, schnelle operation
	- 
- Blur,
	- ![[Pasted image 20250205205220.png]]
	- 
- Laplace
	- ![[Pasted image 20250205222528.png]]
	- linearer Filter
	- Grauwertsprünge zwischen dunklen und hellen Bildregionen hervorheben (hervorhebung grauwertdifferenzen)
	- Realisiert Approximation/abschätzung der zweiten ableitung
	- sensibel auf kleine störungen
	- Bei negativen drauf achten was in aufgabe steht, ganze zahlen sind auch negativ
- Min
	- Nicht linear, Rangordnungsoperatoren
	- Dunkle Regionen Säubern
	- Helle schrumpfen/zerstören
	- Ergebnis: kleinster wert im operatorenfenster (außerhalb rand ist 0)
- Max
	- Nicht linear, Rangordnungsoperatoren
	- Ergebnis: größter wert im operatorenfenster
	- Helle regionen säubern
	- Dunkle regionen schrumpfen/zerstören
- Closest-of-Min-Max
	- min und max bilden
	- wert wählen von beiden der am nächsten ist an original/hotspot. bei gleichstand ist egal, aber konsistent wählen
	- falls unbefriedigend, dann iterative anwendung oder vergrößerung von operatorfenster hilft
	- verstärkung von grauwertdifferenzen, hervorhebung von grauwertsprüngen
- Prewitt
	- ![[Pasted image 20250205221602.png]]
	- Hervorhebung von Grauwertdifferenzen
	- weniger empfindlich gegenüber Bildstörungen
	- realisieren approximation der 1. ableitung
- Faltung
	- wenn mit fenster darstellbar und filter linear ist. faltung kann man mit fourier darstellen
- Linear
	- verknüpfung der Pixelwerte innerhalb des Operatorenfensters durch linearen ausdruck (gewichtete summe)
- nichtlinear
	- verknüpfung der Pixelwerte innerhalb des Operatorenfensters durch nichtlinearen ausdruck (min, max, median, exp)
- Rangordnungsoperatoren
	- werte werden sortiert, gewichtet, aufsummiert. summe bildet neuen wert
	- nichtlinear
- absolute Differenz min und max für jedes pixel
	- ergibt hervorgehobenen wertübergänge zwischen dunklen und hellen regionen
- Separierbarkeit
	- zerteilung eines zweidimensionalen filters in zweii eindimensionale
	- geht wenn filterfunktion als (äußeres) produkt beschrieben werden kann
![[Pasted image 20250205120505.png]]
yes

![[Pasted image 20250205120516.png]]
check

![[Pasted image 20250205120523.png]]
check
![[Pasted image 20250205120536.png]]
ye
![[Pasted image 20250205120546.png]]
ye
![[Pasted image 20250205120554.png]]
jo
![[Pasted image 20250205120606.png]]
jo

![[Pasted image 20250205120916.png]]
ye
![[Pasted image 20250205120924.png]]
ye
![[Pasted image 20250205120932.png]]
check