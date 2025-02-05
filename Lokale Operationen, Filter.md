- Glättungsfilter
	- Maske enthält nur werte >= 0
- Differenzfilter
	- Maske enthält mind. 1x Wert > 0 und Wert < 0
- Box
	- ![[Pasted image 20250205205142.png]]
	- Rauschen Redizieren
	- Steile Grauwertübergänge abgeflacht, Kanten unscharf
	-  Tiefpass Filterung
- Median
	- nicht linear, Rangordnungsoperatoren
	- Alle Werte werden sortiert, und der mittlere wird gewählt (median)
	- regelmäßiges rauschen entfernen
- Blur,
	- ![[Pasted image 20250205205220.png]]
	- 
- Laplace
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
- Prewitt
- Faltung: linear/nicht linear beachten
	- Linear
		- verknüpfung der Pixelwerte innerhalb des Operatorenfensters durch linearen ausdruck (gewichtete summe)
	- nichtlinear
		- verknüpfung der Pixelwerte innerhalb des Operatorenfensters durch nichtlinearen ausdruck (min, max, median, exp)

- Rangordnungsoperatoren
	- werte werden sortiert, gewichtet, aufsummiert. summe bildet neuen wert
	- nichtlinear

![[Pasted image 20250205120505.png]]
![[Pasted image 20250205120516.png]]
![[Pasted image 20250205120523.png]]
![[Pasted image 20250205120536.png]]
![[Pasted image 20250205120546.png]]
![[Pasted image 20250205120554.png]]
![[Pasted image 20250205120606.png]]![[Pasted image 20250205120823.png]]
![[Pasted image 20250205120837.png]]
![[Pasted image 20250205120849.png]]
![[Pasted image 20250205120916.png]]![[Pasted image 20250205120924.png]]
![[Pasted image 20250205120932.png]]
