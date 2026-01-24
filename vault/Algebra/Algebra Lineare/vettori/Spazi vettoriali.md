Uno spazio vettoriale V su un campo K è una struttura algebrica $(V,+,\cdot)$ dove:
- $+:V\times V \to V$
- $\cdot: K\times V \to V$ 
in cui V è il gruppo dei vettori e K il campo degli scalari
	
**proprietà**:
- chiuso
- associatività scalare: $s,t \in K, v \in V \implies s \cdot (v\cdot t) = (s \cdot v) \cdot t$
- elemento neutro: $1 \in K, v \in V \implies 1\cdot v = v$
- distributività vettoriale: $s,t \in K, v \in V \implies v(s + t)= vs + vt$ 
- distributività scalare: $s \in K, v,w \in V \implies s(v+w)=sv+sw$
- vettore nullo: $0_v$ significa un vettore di elementi nulli (0,0,0,0)
	- $0_v \in V, \lambda \in K \implies \lambda \cdot 0_v = 0_v$ 
	- $0 \in K, v \in V \implies 0 \cdot v = 0_v$
## sottospazio vettoriale
un sottospazio vettoriale è una struttura con le stesse proprietà dello spazio vettoriale, ma su un insieme più piccolo
## spazio di coordinate
uno spazio di coordinate è uno spazio vettoriale in cui l'addizione tra vettori e il prodotto scalare sono definite come:

- addizione: presi...
	  $v:=(t_1,...,t_n) \in K^n$ 
	  $w:= (s_1,...s_n) \in K^n$ 
	  $v+w:= (t_1+s_1,...,t_n+s_n) \in K$
- moltiplicazione: presi ...
	  $v:=(t_1,...,t_n) \in K^n$
	  $\lambda \in K$
	  $\lambda \cdot v = (\lambda \cdot t_1,..., \lambda \cdot t_n) \in K^n$
