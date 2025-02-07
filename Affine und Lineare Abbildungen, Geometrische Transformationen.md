- unten immer 0,0,1 für 2D Transformationen
$$\begin{matrix}
a & b & tx \\
c & d & ty \\
0 & 0 & 1
\end{matrix}$$
- Scherung/Streckung
$$\begin{matrix}
1 & kx & 0 \\
ky & 1 & 0 \\
0 & 0 & 1
\end{matrix}$$
	- a und d = 1 bzw. Faktor für vergrößerung
	- kx > 0 => Bild nach rechts verzerrt
	- ky > 0 => Bild nach oben verzerrt
- Rotation
	- Allgemein:
$$	\begin{matrix}
cos(\alpha) & -sin(\alpha) & 0 \\
sin(\alpha) & cos(\alpha) & 0 \\
0 & 0 & 1
\end{matrix}$$
	- Dabei ist $\alpha$ der Winkel gegne Uhrzeigersinn
	- Dreht 90° (im) Uhrzeigersinn:
$$
\begin{matrix}
0 & 1 & 0 \\
-1 & 0 & 0 \\
0 & 0 & 1
\end{matrix}
$$
	- Dreht 180°:
$$
\begin{matrix}
-1 & 0 & 0 \\
0 & -1 & 0 \\
0 & 0 & 1
\end{matrix}
$$
- Skalierung
	- a und d ändern sich
	- a=d: gleichmäßige Skalierung
- Spiegelung
	- An X achse
$$\begin{matrix}
1 & 0 & 0 \\
0 & -1 & 0 \\
0 & 0 & 1
\end{matrix}$$
	- An Y Achse
$$\begin{matrix}
-1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{matrix}$$
	- Punktspiegelung
$$
\begin{matrix}
-1 & 0 & 0 \\
0 & -1 & 0 \\
0 & 0 & 1
\end{matrix}$$
- Translation (Verschiebung)
	- tx und ty
	- wird als $(t_x,t_y)^T$ angegeben
- Source to target erklären
- target to source erklären
- Affine Abbildungen sind $A*x$
	- das hoch T nicht vergessen
	- für Homogene Koordinate eine 1 in 3. Zeile ergänzen
- ! Invarianz gegenüber geometrischen EIgenschaften mit Transformationen
- Interpolationsverfahren
	- nearest neighbor
		- nächster Pixel, sehr schnell
		- eckige/scharfe kanten
	- lineare
		- Zwei abtastpunkte, durchschnitt
	- bilinear
		- vier nachbarn, durchschnitt
		- flüssiger übergang der kanten
- Vorwärtstransformation, vorundnachteile
- Rückwärtstransformation, vorundnachteile
- Homogene Koordinate
- 
![[Pasted image 20250205121905.png]]
ye
![[Pasted image 20250205121939.png]]
ye
![[Pasted image 20250205121812.png]]
ye
![[Pasted image 20250205121954.png]]
ye
![[Pasted image 20250205122002.png]]
ye
![[Pasted image 20250205122012.png]]
ya
![[Pasted image 20250205122020.png]]

![[Pasted image 20250205122028.png]]

![[Pasted image 20250205122042.png]]

![[Pasted image 20250205122051.png]]

