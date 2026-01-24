dato uno spazio vettoriale V ed un sottospazio $W \subseteq V$.
La struttura $(V/W,+,\cdot)$ è l'insieme quoziente, dove la somma è definita come $[v]+[w]=[v+w]$ e il prodotto come $\lambda [v] = [\lambda v]$

immaginiamo uno spazio vettoriale che rappresenta un edificio tridimensionale, un vettore che rappresenta un punto di questo edificio sarà  composto da $$\begin{pmatrix} \mathbb{R} \\ \mathbb{R} \\ \mathbb{R} \end{pmatrix}$$
se si volesse raggruppare i punti nell'edificio in base al piano, si dovrebbe agire sul terzo elemento $$\begin{pmatrix} \mathbb{R} \\ \mathbb{R} \\ 0 \end{pmatrix}$$
in questo modo, prendendo 2 punti nello spazio, e facendone la sottrazione, se il terzo elemento è 0, saranno in relazione e quindi nella stessa classe.

# dimensione di uno spazio quoziente
la dimensione di uno spazio quoziente sarà $$dim(V/W)= dim(V)-dim(W)$$
esempio:
riprendendo il vettore di prima $$\begin{pmatrix} x \\ y \\ 0 \end{pmatrix}$$
esso è formato da una base (rappresentata canonicamente) del tipo: $$\text{base}(W)=\set{\begin{pmatrix}1 \\ 0 \\ 0 \end{pmatrix},\begin{pmatrix} 0 \\ 1 \\ 0 \end{pmatrix}}$$
invece $$\text{base}(V)=\set{\begin{pmatrix}1 \\ 0 \\ 0 \end{pmatrix},\begin{pmatrix} 0 \\ 1 \\ 0 \end{pmatrix},\begin{pmatrix} 0 \\ 0 \\ 1 \end{pmatrix}}$$
l'insieme quoziente $V/W$, viene suddiviso in base alla terza riga, immaginiamola come asse Z, quindi la base dell'insieme quoziente sarà $$\set{[\begin{pmatrix} 0 \\ 0 \\ 1 \end{pmatrix}]}$$