La funzione di Eulero trova la cardinalità dei numeri coprimi ad n
$$\phi(n)=x :(x \in \mathbb{N} \land 0 \lt x \leq n \land MCD(n,x)=1)$$
# numeri primi
dato $p \in P$ si ha che $$\phi (p) = p-1$$
e dato $p^k$ si ha che:
$\phi(p^k)=p^k - p^{k-1}$
# numeri non primi
dato $n=p_1 * p_2$ si ha che 
$$\phi (n)= \phi(p_1)*\phi(p_2) \implies \phi(n)= (p_1 -1)(p_2 -1)$$

es:
	1. $\phi(40) = \phi(5) * \phi(2^3) = (5-1)*(2^3 - 2^2)= 4*4=16$  