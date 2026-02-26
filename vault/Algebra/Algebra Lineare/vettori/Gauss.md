è possibile trasformare un insieme di vettori in una matrice per sapere se esso è linearmente indipendente
$$\set{\begin{pmatrix}1 \\ -3 \\ 3\end{pmatrix},\begin{pmatrix}0 \\ 2 \\ 2\end{pmatrix},\begin{pmatrix} 1 \\ 3 \\ -3\end{pmatrix},\begin{pmatrix} 0 \\ 1 \\ 0\end{pmatrix}} \to \begin{pmatrix}1,0,1,0 \\ -3,2,3,1 \\ 3,2,-3,0\end{pmatrix}$$
per sapere se questo insieme di vettori è linearmente indipendente, bisogna trasformarlo in modo tale da avere dei pivot che vanno in diagonale dall'angolo sinistro superiore  fino a toccare la base e sotto di essi degli 0
## operazioni
per modificare la matrice si possono utilizzare le seguenti operazioni:
- **scambio**: è possibile scambiare due righe tra loro, è comodo avere quella con il pivot di valore più alto sopra l'altra 
- **addizione**: è possibile addizionare e quindi sottrarre una riga ad un altra per un valore k
	  es: $R_2 \to R_2+k\cdot R_1 = -3231+(3\cdot 1010)=0261$
- **moltiplicazione per se stesso**: $R_1 \to k \cdot R_1$
# gauss per trovare matrice inversa
si accostano la matrice di cui si vuole trovare l'inverso e la matrice d'identità e si utilizza gauss per ottenere a sinistra la matrice di identità (quindi trasformare la matrice originale in matrice di identità) e a destra la sua inversa