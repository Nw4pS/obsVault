Una matrice $M_{m,n}$ è una struttura algebrica $(\text{insieme}, +, \cdot)$ detta [[anello]] unitario e viene visualizzata tramite righe e colonne in cui:
- $M_{m,n}(\mathbb{R})$ denota che gli elementi della matrice sono nell'insieme dei numeri reali
- $m =$ numero di righe
- $n=$ numero di colonne
es:
$A = \begin{pmatrix} 1 & 2 & 3 \\ -5 & 6 & 7 \end{pmatrix}$ con $A \in M$ e con gli elementi $a_{i,j} \in \mathbb{R}$ e $1<=i<m, 1<=j<=n$
# operazioni
Siano $A,B \in M_{m,n}$

$A= \begin{pmatrix} 1 & 2 & 3 \\ 5 & 6 & 7 \end{pmatrix}, B= \begin{pmatrix} 7 & 8 & 11 \\ -3 & 4 & 0 \end{pmatrix}$

- somma:
	per sommare due matrici, es $A+B$ si somma l'elemento $a_{i,j}$ e l'elemento $b_{i,j}$ .
	$A \begin{pmatrix} 1 & 2 & 3 \\ 5 & 6 & 7 \end{pmatrix} + B \begin{pmatrix} 7 & 8 & 11 \\ -3 & 4 & 0 \end{pmatrix} = C\begin{pmatrix} 8 & 10 & 14 \\ 2 & 10 & 7 \end{pmatrix}$ 
- prodotto:
	supponendo una matrice quadrata, quindi con $m=n, A=(a_{i,j}), B=(b_{i,j})$ definiamo il prodotto della matrice quadrata con questa formula (poiché più facile di dirlo a parole):
	$\sum_{l=1}^{n}{(a_{i,l})\cdot(b_{l,j})}$  

# elemento neutro
l'elemento neutro della matrice è detto "matrice di identità" poiché ritorna la matrice per la quale viene moltiplicato.

$M_{m,n}\begin{pmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{pmatrix}$ con $m=n=3$ 

$M_{m,n}\begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}$ con $m=n=2$ 
