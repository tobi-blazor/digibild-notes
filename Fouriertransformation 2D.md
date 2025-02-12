- (Amplituden und Phasenspektrum aus Bild ableiten)
- (Parameter der Kosinus funktion ermitteln aus Bild)
	- Gleichanteil, Frequenzm Amplitude, Phasenverschiebung
- 3 Anwendungen der Fouriertransformatin
	- synthese, analyse, filtern von signalen, kompression von signalen, analyse der fq eines signals
	- (hochpass,tiefpass, bandpass sind keine anwendungen)
- struktur des fourierspektrums
	- ![[Pasted image 20250208145431.png]]
	- 4f ist hälfte
- zweidimensionale diskrete fourier transformation ist separierbare transformation - warum?
	- weil es umgeformt werden kann
- was bedeutet separierbarkeit in praxis? (programmieren)
	- durch separierbarkeit kann leicht eine mehrdimensionale DFT implementiert werden
- faltungstheorem 
	- was passiert bei xxx des bildes im fourierraum?
		- roatation: rotiert mit
		- translation: unverändert
	- als konzept erklären können
		- lohnt sich bei großen operatorenfenstern
	- für 2 dimensionale fouriertransformation
		- zentriert weil mittlerer punkt sehr wichtig
		- wellenfront farbverlauf
- Artefakte von Manipulation in Fourier Spektrum, wie verhindern
	- Aliasing effekt
		- zu geringe abtast fq, führen zu moire mustern die im bild nicht waren
	- welligkeit/ringing
		- wegen zeitbegrenzung eines signals, wellen um objekt herum
	- leck-effekt
		- wenn beobachtungsintervall nicht ganzzahligen vielfachen der periodenlänge entspricht
- bei zentrierten spektrum skizzieren wo einfluss hohe frequenzen /niedrige am höchsten ist
	- niedrige in mitte
- Asymptotischer Zeitaufwand 2D-FFT  für rechteckige bilder der DImension MxN, M>N
	- DFT: Gesamt: O(M * N^2 + N * M^2 )
	- FFT: Gesamt: O(M * N (logM + logN ))


![[Pasted image 20250205122312.png]]
y

![[Pasted image 20250205122340.png]]
y
![[Pasted image 20250205122405.png]]
y
![[Pasted image 20250205122418.png]]
y
![[Pasted image 20250205122428.png]]
y
![[Pasted image 20250205122437.png]]
y
![[Pasted image 20250205122445.png]]
y
![[Pasted image 20250205122455.png]]
y
![[Pasted image 20250205122509.png]]
y
![[Pasted image 20250205122519.png]]
y