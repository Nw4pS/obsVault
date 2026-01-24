# gruppo simmetrico di ordine n
prendiamo come esempio $(S_{n}, \circ)$, 
- $S_n =\{\mathcal{f}:[n]\rightarrow [n] | \mathcal{f}$ è bigettiva $\}$ è l'insieme delle funzioni bigettive che hanno $n$ come dominio e codominio.
- $\circ$ è un'operazione sull'insieme $S_n$ e $\tau \circ \alpha$ si legge come $\tau(\sigma(x))$    
Il gruppo simmetrico di ordine n ha le seguenti proprietà:
1. $\circ$ è **associativa**
2.  la **composizione** di funzioni bigettive è **bigettiva**, ovvero  $\forall \mathcal{g}, \mathcal{f} \in S_n$ , $\mathcal{g} \circ \mathcal{f} \in S_n$ 
3.  esiste l'**elemento neutro**: nel caso di $S_n$ abbiamo che la funzione $id(x)=x$. poiché in questo gruppo gli elementi sono funzioni allora si ha $id \circ \mathcal{f} = \mathcal{f} = \mathcal{f} \circ id$.
  L'ordine di un elemento è l'$r: a^r =e$ con a nell'insieme degli elt ed e elemento neutro
4. esiste l'**elemento inverso** di ogni elemento $\forall \mathcal{f} \in S_n, \mathcal{f}^-1 \in S_n$ con $\mathcal{f}^{-1}{(z)=x}:\mathcal{f}(x)=z$ 
- la cardinalità di $S_n$ è $n!$:
	è possibile rappresentare una funzione tramite una matrice $\begin{pmatrix} 1 & 2 & 3\\ \mathcal{f}(1) & \mathcal{f}(2) & \mathcal{f}(3) \end{pmatrix}$ , nella fila superiore sono presenti dei valori input alla funzione, nella fila inferiore sono presenti gli output.
	$S_n$ è l'insieme di tutte le funzioni bigettive che hanno come dominio e codominio l'insieme $\{0,1,2, ...,n\}$ ovvero tutti i modi per mappare un $n \in [n]$ in un altro $n \in [n]$ (il professore utilizza la notazione $X \rightarrow X$,quindi queste notazioni sono intercambiabili) e poiché in un insieme non possono esistere elementi identici (funzioni che effettuano la stessa mappatura), il numero di funzioni in $S_n$ è esattamente $n!$ 
	**esempio grafico:**
	$\begin{pmatrix} 1 & 2 & 3\\ \text{3 mappature possibili} & \text{2 mappature restanti} & \text{1 mappatura restante} \end{pmatrix}$ ovvero $3*2*1=3!$
# gruppo ciclico
Un gruppo ciclico è composto da un insieme ciclico, esso è dato da un elemento n detto **generatore** con il quale è possibile generare ogni altro numero dell'insieme ripetendo l'operazione del gruppo su se stesso e quindi su altri elementi del sottogruppo

esempio $(R,+)$
preso n=1 si crea un insieme $\set{1,2,3,...}$ formato da 1+1, 1+1+1, 1+1+1+1 ovvero da $$\set{n,2n,3n,4n}$$
dato che un gruppo ha anche l'elt inverso per ogni elemento, allora l'insieme conterà anche gli elementi $\set{-n,-2n,-3n}$ generati da $\set{1,1-1,1-1-1,\text{ecc...}}$

# sottogruppo
Un sottogruppo è un gruppo composto da un sottoinsieme degli elementi del gruppo.
Un sottogruppo di un gruppo ciclico sarà ciclico a sua volta, un sottogruppo ciclico generato da un elt a viene indicato come $<a>$

> NOTA: tutti i sottogruppi contenenti un numero $z \in \mathbb{Z}$ sono sottogruppi che hanno come generatore un divisore di $z$ poiché utilizzando l'operazione su $z$ ed un altro numero in $\mathbb{Z}$, si arriverà ad avere un generatore divis di z
> es: presi $\set{5,18}$ per chiusura, ogni risultato dell'operazione sui numeri nell'insieme è nell'insieme, quindi anche: 18-5= 15)  18-15=3,  5-3=2,  3-2=1 e quindi anche tutti i numeri generati da $<1>$ 

**proprietà**
- l'intersezione di due sottogruppi è un sottogruppo
- l'unione tra due sottogruppi è un sottogruppo? si, solo se uno è contenuto nell'altro
- un sottogruppo $H$ di un gruppo finito $G$ avrà cardinalità k che divide la cardinalità di G, ad esempio, un gruppo con 10 elementi, può avere sottogruppi di 2 o 5 elementi 
## sottogruppo normale
un sottogruppo normale è un sottogruppo $H \leq G$ in cui preso $x \in G$ , si ha che $$xH=Hx$$
questo significa che gli elementi di xH sono gli stessi di Hx, ma ad esempio $x*h$ e $h*x$ possono essere diversi e comunque essere nel gruppo xH o nel gruppo Hx
 # semigruppo
un semigruppo è una struttura algebrica composta da un insieme, un'operazione su cui vale l'associatività
