è essenziale leggere prima la pagina sulla [[congruenza lineare]]
il teorema cinese dei resti serve a risolvere sistemi di congruenze
$$\begin{cases}
a_1 x\equiv b_1 \mod{m_1} \\
a_2 x\equiv b_2 \mod{m_2}\\
a_n x \equiv b_n \mod{m_n}\end{cases}$$
condizione di esistenza:
- $\text{MCD }(a,m)=d$ con d che divide b

es:
$2x \equiv 7 \mod{10}$ non ammette soluzione perché $\text{MCD }(2,10)=2$ ed esso non è divisibile per 7.
>se in  $$\begin{cases}
a_1 x \equiv b_1 \mod{m_1} \\
a_2 x \equiv b_2 \mod{m_2}\\
a_n x \equiv b_n \mod{m_n}\end{cases}$$ le m sono a due a due coprimi tra loro, ovvero il loro MCD è 1 allora il sistema può essere scritto in maniera ridotta $$\begin{cases}
a_1 x\equiv b_1 \mod{m_1} \\
a_2 x\equiv b_2 \mod{m_2}\\
a_n x\equiv b_n \mod{m_n}\end{cases} \implies
\begin{cases}
x \equiv c_1 \mod{m'_1} \\
x \equiv c_2 \mod{m'_2}\\
x \equiv c_n \mod{m'_n}\end{cases}$$
# algoritmo risolutivo
1. controllare che le congruenze rispettino la condizione di esistenza
2. controllare che le congruenze siano 2 a 2 con m coprimi
3. semplificare il sistema (con esempio $\begin{cases} 2x \equiv 7 \mod{5} \\ 3x \equiv 8 \mod{4} \end{cases}$):
	1.   trasformando la prima congruenza in equazione $2x=7+5k \implies x=\frac{7+5k}{2}$ 
	2. assegno iterativamente a k un valore intero da 0 a $\infty$ fino ad avere il numero x intero $k=1,x=\frac{7+5k}{2}=6$
	3. assegno il risultato a c
	4. effettuo lo stesso procedimento alle prossime congruenze
4. trovato il nuovo sistema $\begin{cases} x \equiv 6 \mod{5} \\ x \equiv 4 \mod{4} \end{cases}$ se i moduli a due a due sono coprimi, allora posso riscrivere il sistema di congruenze come un'unica congruenza modulo al massimo $M=(m_1*m_2)$ se le m non sono coprime tra loro, saltare questo algoritmo e continua a leggere
5. trovare la nuova congruenza
	1. trasformo la prima congruenza in equazione $x=6+5k$
	2. sostituisco la x trovata alla seconda congruenza $6+5k \equiv 4 \mod{4}$
	3. isolo k a sinistra $k=1(4-6)$, per spostare una moltiplicazione a destra o sinistra, va trovato il numero che moltiplicato per il numero da spostare, dia come resto 1 se diviso per il modulo, ad esempio $5*1$ diviso 4 da resto 1
	4. trovato il valore di k, in questo caso $k=-2$
	5. sostituire k all'equazione della prima congruenza per trovare il valore di x, il risultato del sistema dato dalle prime 2 congruenze sarà la x trovata modulo $(m_1*m_2)$ in questo caso $\mod 20$
nel caso in cui le due m non siano coprimi, esiste comunque soluzione se:
- $\text{MCD}(m_1,m_2)|(c_1-c_2)$ , la soluzione è unica in $\mod({\text{mcm}(m_1,m_2))}$ 