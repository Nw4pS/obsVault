# dimostrazione per induzione:
La dimostrazione per induzione è utile quando si deve dimostrare che una condizione è vera per tutti gli elementi in un insieme.
1. si controlla se la condizione è vera per un valore n, ad esempio 1
2. si controlla se è vera per un valore generico k=n+1
poiché generico, se è vero per un valore, sarà vero per il successivo, come un effetto domino
# mostrare che qualcosa sia un anello o gruppo o relazione o altro
basta dimostrare le proprietà una per una
# tecniche usate nelle dimostrazioni
## 1. trucco dell'elemento neutro (ninja)
**quando usarlo:** quando hai un elemento z complesso e si deve dimosrare una certa struttura complessa.
Se si ha che 1= qualcosa, in una dimostrazione può essere utile moltiplicare per 1 (si può fare sempre se è l'elemento neutro) e sostituirlo con qualcosa  date le ipotesi per vedere se si riesce ad andare avanti
es:
dati $z=z*1$ e $1= u*v$, sostituendo abbiamo che $z= z(u+v)=zu+zv$
# 2. traduci tutto subito (dizionario)
tradurre il testo in matematichese o scrivere delle proprietà dovute dalle ipotesi per avere le traduzioni davanti agli occhi e rendere tutto più intuitivo, nel caso di 
- "siano I J degli ideali" si traduce in $\text{se }x \in I \text{ e } r \in A \implies xr\in I$ ovvero la proprietà assorbente, in questo modo quando la vediamo possiamo riconoscerla
- "$I+J=A$" significa che i valori in A sono composti da $i+j$ ad esempio $i+j=1$ e ci ricolleghiamo al trucco del ninja
- "$z\in I\cap J$" significa che $z \in I \text{ e } z \in J$
# 3. doppia inclusione
**quando usarlo:** quando si deve dimostrare che $A=B$ 
**come:** dimostrare che:
- $A \subseteq B$ 
- $B \subseteq A$ 
spesso una è ovvia e l'altra no
# 4. lavorare indietro (reverse engineering)
se non sai come partire dall'ipotesi, parti dalla tesi e smontala fino ad arrivare all'ipotesi
1. voglio dimostrare che $z \in IJ$
2. come è fatto un elemento di $IJ$
3. è una somma di cose tipo $x*y$?
4. posso usare la tecnica ninja?2w

# $\iff$ se e solo se
quando si presenta se e solo se, dobbiamo dividerlo in due esercizi
1. andata ($\implies$): in cui si prende per vero ciò che è a sinistra e si dimostra ciò che è a destra
2. ritorno ($\impliedby$): in cui si prende per vero ciò che è a destra e si dimostra ciò che è a sinistra