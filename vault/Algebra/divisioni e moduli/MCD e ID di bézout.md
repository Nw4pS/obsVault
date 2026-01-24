dati $a_1,...,a_k \in \mathbb{Z}$ definiamo $d \in N$ come massimo comun' divisore degli elementi a, se dato $k \in \mathbb{z}$ 
$$k|a_1\land...\land k|a_n\iff k|d$$
a parole "esiste un k che divide ogni elemento di a, se e solo se k divide d" non risulta molto intuitivo, ma d è il massimo comune divisore, infatti $k=d$ divide d ed essendo il k massimo (poiché il valore k più alto che divide d) allora è anche il massimo valore che divide gli elementi di a
**numeri coprimi:**
	due numeri si dicono coprimi se tra di loro hanno 1 come MCD
# Identità di Bézout
il MCD(a,b) con a b non entrambi nulli, si può trovare tramite:
$$ax+by=d$$
ad esempio a=12, b=18
$$12x+18y=6$$ se $x=-1$ ed $y=1$

 **come trovare l'identità:**
 per trovare l'identità di Bézout si può utilizzare l'[[Algoritmo di Euclide]] e riscrivere le divisioni come $$\text{resto}= \text{dividendo} + \text{divisore}*\text{quoziente}$$
partendo dalla divisione con $\text{resto} = d$ dato il seguente esempio con $d=1$:
![[Pasted image 20251210190015.png]]
si prende il divisore (il resto della divisione precedente) e si sostituisce con la parte destra dell'equazione che ha quel divisore come resto, si deve cercare di tenere una moltiplicazione tra due numeri in modo tale da arrivare ad avere un'identità di Bézout ovvero $1=14743*x + 8915*y$
si procede a mostrare i passaggi:
1. $1=5-2*2 \implies 1=5-(22-5*4)*2 \implies 1=5-22$
2. $1=5-22 \implies 1=(27-22*1)-22$
3. $1=27-22*2$
4. ... si continua fino ad avere $1=14743*x + 8915*y$

**utilità:**
- **trovare l'inverso modulo n**: si vuole risolvere l'equazione $5x\equiv (\text{mod }17)$ ovvero l'inverso di 5 nel mondo modulo 17. 
  1. si traduce in equazione $$5x \equiv 1(\text{mod }17) \implies 5x -1 =17y$$ ovvero che esiste un numero y che indica quante volte 17 ci sta in 5x-1, riordinando i termini si ha che $$5x-17y=1$$ che è come l'identità di Bézout
Bézout dice che poiché $MCD(5,17)=1$ allora $5x+17y=1$
- **risolvere equazioni Diofantee**: Equazioni del tipo 3x+5y=100 (dove cerchi soluzioni intere)
- **algoritmo RSA**: cifratura, non si guarderà nel corso
