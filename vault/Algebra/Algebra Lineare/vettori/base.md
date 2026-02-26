dato uno spazio vettoriale V su K, una base è un insieme di vettori $(v_1,...,v_n)\neq 0_v \in V$ che sono sia un insieme di generatori che linearmente indipendenti
## base canonica
dato uno spazio di coordinate $K^n$ la base canonica è un insieme di vettori composto in questo modo:
$$e_i=(a_1,...,a_n) | \begin{cases}a_j=0 \iff i\neq j \\ a_j = 1 \iff i= j\end{cases}$$
per $K^3$ ne esce fuori:
$e_1 = \begin{pmatrix} 1 \\ 0 \\ 0 \end{pmatrix}, e_2 = \begin{pmatrix} 0 \\ 1 \\ 0 \end{pmatrix}, e_3 =\begin{pmatrix} 0 \\ 0 \\ 1 \end{pmatrix}$
questo ci permette di esplorare tutto il piano delle coordinate in maniera semplice, infatti un vettore del tipo $$\begin{pmatrix} 5 \\ -3 \\ 8 \end{pmatrix}$$ non sarà altro che $5 \cdot e_1, -3 \cdot e_2, 8 \cdot e_3$ 
# trovare una base
dati più matrici o vettori, si costruisce la matrice su cui utilizzare [[Gauss]].
La base di quell'insieme corrisponderà ai vettori/matrici corrispondenti alle matrici/vettori utilizzati.
Per trasformare un insieme di vettori/matrici per utilizzare Gauss, si prende un vettore/matrice e lo si scrive come colonna della matrice, es:
$$t_1=\begin{pmatrix}
1\space 1 \\
2 \space 1
\end{pmatrix}, t_2=\begin{pmatrix}
1\space 2 \\
1 \space 1
\end{pmatrix},t_3= \begin{pmatrix}
0\space 1 \\
-1 \space 0
\end{pmatrix} \to M= \begin{pmatrix}
1\space 1 \space 0\\
1 \space 2 \space 1\\
2 \space 1 \space -1\\
1 \space 1 \space 0
\end{pmatrix}$$

