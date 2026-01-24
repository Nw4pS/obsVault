il piccolo teorema di Fermat afferma che $$a^{\phi(m)} \equiv 1 \mod{m}$$
se $a$ ed $m$ sono coprimi tra loro.
# dim informale
utilizziamo modulo n,
preso un insieme di numeri coprimi a m
es: m=10 $\set{1,3,7,9}$
preso un numero coprimo ad m, es: n=3

moltiplicando ogni elemento dell'insieme per il numero m si ottiene 
$\set{3*1,3*3,3*7,3*9}=\set{3,9,21,27}$ che in modulo 10 è $\set{3,9,1,7}$  che è lo stesso insieme iniziale modulo 10 quindi il prodotto degli elementi all'interno del set è lo stesso, in questo caso $189=T$
e quindi:
$$(3*1)(3*3)(3*7)(3*9)\equiv 1*3*7*9 \mod{10}$$
è possibile mettere da parte il 3 per rendersi conto di una cosa:
$$3^4*(1*3*7*9)\equiv 1*3*7*9 \mod{10}$$
$$3^4*T \equiv 1*T \mod{10}$$
poiché $T$ è una somma di numeri coprimi a 10, allora anche T è coprimo a 10, questo significa che ha un inverso ed è possibile quindi dividere sia a inistra che a destra per l'inverso, ottenendo:
$$3^4 \equiv 1 \mod{10}$$
> notare che si è utilizzato 3, ma si sarebbe potuto utilizzare qualsiasi altro numero coprimo con 10 (coprimo perché altrimenti si modificherebbe l'insieme e quindi non si avrebbe più $T\equiv T$)

> notare anche che l'esponente a cui viene elevata la base per essere congrua a 1 è il numero di numeri coprimi con il modulo che si calcola tramite la funzione di eulero

si torna quindi alla forma 
$$a^{\phi(m)} \equiv 1 \mod{m}$$
# ulteriore forma
$$a^n \equiv a^{n \mod{\phi(m)}} \mod{m}$$
si vuole trasformare m in elementi più piccoli:
$3^{31}\mod{10}$, si prende $\phi(10)=4$
e si trasforma il 31 in $$31=(4*7)+3$$
ovvero il "ritmo" ogni quanto si ottiene 1 come resto (la cardinalità dei numeri coprimi ad m) moltiplicato per quante volte viene eseguito, più il resto, quindi a quanto è congruo il 31 $\mod{\phi(10)=4}$

quindi $3^{31}\equiv 3^{(4*7)+3}\mod{10}$ 
manipolando la congruenza si ottiene:
1. $3^{31}\equiv 3^{(4*7)}*3^{3}\mod{10}$ 
2. $3^{31}\equiv (3^4)^7 ** 3^{3}\mod{10}$
3. poiché $3^4 \mod 10$ è congruo ad 1, è possibile sostituirlo
4. $3^{31}\equiv 1^7*3^{3}\mod{10}$
5. $3^{31}\equiv 3^{3}\mod{10}$
in questo modo è stato ridotto $3^{31}$ in una potenza facilmente calcolabile

> nota bene, utilizzando la formula originale si ottiene $$3^{31} \equiv 3^{31 \mod{4}} \mod{10}$$ in cui $31 \mod 4$ significa "il resto di $\frac{31}{4}=7$ ovvero $3=31-4*7$ ovvero $31=3+4*7$"