un isomorfismo è un [[omomorfismo]] su cui vale la biettività, quindi applicando la funzione inversa a destra, si ottiene l'elemento originale $$\mathcal{f}^{-1}(\mathcal{f}(x))=x$$
es:
preso $g \in G$ e l'isomorfismo $\mathcal{f}(x)\to ghg^{-1}$
$\mathcal{f}(x\cdot y) = \mathcal{f}(x)\cdot \mathcal{f}(y)$

$gxyg^{-1}_G = (g(x)g^{-1}g(y)g^{-1})_G$  
risolviamo a destra:
$$gxg^{-1}gyg^{-1} \to gxeyg^{-1} \to gxyg^{-1}$$ in questo modo abbiamo dimostrato la biettività dell'isomorfismo

# primo teorema dell'isomorfismo
se $\mathcal{f}:A\to B$ è un isomorfismo tra anelli, allora 
$$\frac{\text{A}}{\ker(f)}\cong \text{im}(f)$$
esempio:
$\mathbb{Z}_4 \cong \mathbb{Z}_5^*$ quando $\mathbb{Z}_4=\frac{\text{A}}{\ker(f)}$ e $\mathbb{Z}_5^*=\text{im}(f)$

l'immagine viene data quando si partiziona l'anello per il kernel, quindi, se abbiamo già l'immagine e l'anello, noi troviamo la funzione dall'anello all'immagine, una volta trovata la funzione, abbiamo il kernel e possiamo scrivere la formula
# isomorfismo di due gruppi ciclici
seguire l'algoritmo:
1. elimina i casi ovvi:
	1. hanno la stessa cardinalità (numero di elementi)? se si, procedi
	2. sono entrambi commutativi o non commutativi? se si, procedi
	3. esiste un generatore? se si, procedi
2. controlla l'ordine:
	1. quanti elementi di ordine 1 ci sono?
	2. quanti elementi di ordine 2 ci sono?
	3. quanti elementi di ordine n ci sono? se la quantità di elementi ordine n è la stessa in entrambi i gruppi /anelli/... allora va avanti
3. trova il generatore del primo gruppo
4. trova il generatore del secondo gruppo
5. manda il primo nel secondo![[Pasted image 20260111203528.png]]