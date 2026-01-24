dato uno spazio vettoriale $(V,+, \cdot)$, definiamo come spazio affine a V la struttura $(A,V,\phi)$ dove:
- gli elementi di A sono punti
- la funzione $\phi: A\times V \to A$ prende un punto in A, un vettore (direzioni del tipo, vai su, giù, destra, sinistra) e tira fuori un altro punto.
	- associatività mista: $$\forall p \in A, \forall v,w \in V, \phi(\phi(p,v),w)=\phi(p,v+w)$$ poiché preso un punto e sommandogli un vettore(indicazione) e sommando un vettore (indicazione) al risultato, si ha come risultato il punto che si ottiene con la somma dei due vettori (somma delle istruzioni, ad es. dicendo "parti da questo punto e vai a destra, ora vai in alto" si ottiene lo stesso risultato di "parti da questo punto e vai in diagonale verso l'alto e a destra".
	- elemento nullo: $a \in A, 0_v \in V, \phi(p,0_v)=0_v$ ovvero, se prendi un punto a e non gli dai indicazioni, si resta nel punto a
	- azione libera e transitiva: $\phi_p: V \to A: v\to \phi(p,v)$ è biettiva.
	  Ovvero fissando il punto di partenza p e dandogli un solo vettore, ottengo un punto d'arrivo e viceversa, se ho un punto di arrivo  è possibile dargli un solo vettore e tornare al punto di partenza, poiché è biettiva e tutti i punti sono nello stesso insieme, allora da un punto è possibile arrivare a tutti gli altri punti 
## sottospazio affine e giacitura
preso un sottospazio $W \subseteq V$ e $v \in V$, un sottospazio affine è l'insieme di punti generato da: $$U=v+W :=\set{v+w | w \in W}$$
dove U viene definito giacitura di W e dove:
$dim(U)=dim(giac(W))=dim(W)$

>ogni sottospazio affine può essere visto come classe laterale di un sottospazio

**se si prendesse un sottospazio di dimensione differente dallo spazio?**
![[Pasted image 20260116004038.png]]
poiché i due vettori  hanno entrambi 3 componenti, non ci sarà alcun problema con la somma