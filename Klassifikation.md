- Objekte kann man durch verschiedene Merkmale/attribute/features beschreiben
- Workflow Klassifikation mit ML
	- Design
		- Definition, Datenquellen
	- Implementation
		- Datenanalyse, Vorverarbeitung, Merkmalselektion, Training
		- Vorverarbeitung: aus bildern werden merkmale extrahiert
	- Evaluation
		- Parameteroptimierung, Modellauswahl
	- Application
- k nächster nachbar
	- für testpunkt die Klasseninfo von k nächstem Punkten in Trainingsmenge, mehrheit antwortet
- Support-Vektor Maschine
	- Bei SVMs findet eine Eingabetransformation mit einer Kernfunktion statt
	- Kernfunktion
		- Radiale Basisfunktionen
		- Polynomfunktionen
		- Identität
		- Problemangepasste Kernfkt (String Kernels)
	- Maximum Margin
		- Breiter rand gut weil höheres Rauschen zulässig
	- Soft Margin
		- Erlaubt fehlklassifikation innerhalb margin
	- Workflow biomedizinische bilder
- Valisierung von Ergebnissen
	- Bootstrapping
		- stichprobe mit zurücklegen ziehen, ca. 30% validierungsmenge, k bootstrapläufe durchgeführt
		- viele replikate durchführbar und aussagekräftige statistiken
	- Kreuzvalidierung
		- Mustermenge in k gleich große teile einteilen
		- wenn k sehr groß, validierungsmenge klein
- Objekterkennung
	- Durch Bildsegmentierung (Features der Segmente)
	- gleitendes Fenster und berechnung der Features
- Attributeigenschaften (gewünscht)
	- Translationsinvariant, Rotationsinvariant, Skaleninvariant
- Features für Objektklassifikation
	- Flächeninhalt
		- TIV, RIV
	- Umfang
		- TIV, RIV
	- Kompaktheit
		- TIV, SIV, RIV
	- Zirkularität
		- Rundheit
	- Bounding Box
		- x-Eck um Punkte
	- Kettencodes
		- Beschreibung von Konturen mithilfe von Codes
		- Invariant gegenüber Startpunktwahl
	- zentrale Momente
		- Verschiebung Ursprung an Schwerpunkt
	- Orientierung
		- Richtung Hauptachse
	- Exzentrizität
		- Größenverhältnis Hauptachse
	-  Hu Momente
		- 7 invariante Merkmale zur Formbeschreibung basierend auf zentrale Momente
	- Projektionen
		- ![[Pasted image 20250209091322.png]]
- Fluch der Dimensionne
	- Steigende Zahl Merkmale -> notwendige trainingsmuster überproportional

![[Pasted image 20250205123325.png]]![[Pasted image 20250205123337.png]]
![[Pasted image 20250205123346.png]]
![[Pasted image 20250205123401.png]]
![[Pasted image 20250205123411.png]]
![[Pasted image 20250205123429.png]]
![[Pasted image 20250205123438.png]]
