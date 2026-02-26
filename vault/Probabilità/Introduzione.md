# Eventi
dato un insieme ambiente:
- carte:= {1,2,3,4,5,6,7,...}
- meteo:={pioggia, nevicata,soleggiato,...}
un evento è un sottoinsieme dell'ambiente al quale viene assegnata una certa probabilità che accada, ad esempio che escano 5 carte di fila con lo stesso seme.
Si dice che l'evento ha successo se si verifica

La probabilità di un evento si misura con il valore $p=r | r\in \mathbb{R}, 0\leq r \leq 1$, più grande è p, più l'evento è probabile.
## operatori logici
Dati degli eventi 
- A= il punteggio ottenuto dal primo dado è minore o uguale al punteggio del secondo dado
- B= la somma dei punteggi ottenuti è pari
- C= il punteggio ottenuto dal primo dado è strattamente maggiore di 3
possono essere scritti come 
- $A= \set{X_1 \leq X_2}$
- $B=\set{X_1+X_2 \space \text{pari}}$
- $C= \set{X_1 \gt 3}$
possono essere utilizzati gli operatori logici:
- OR: $A \lor B=\set{\text{si è verificato almeno uno dei due eventi}}$
- AND: $A \land B=\set{\text{si sono verificati entrambi gli eventi}}$
- NOT: $\lnot A=\set{\text{non si è verificato l'evento}}$
# evento composto
un evento si dice composto quando $E= E_1 \lor E_2, E\neq E_1, E \neq E_2$, altrimenti si dice evento semplice (o elementare).
es: l'evento "esce una faccia del dado superiore a 3" è un evento composto, poiché $\set {X_1\gt 3}= \set{X_1=4}\lor \set{X_1=5} \lor \set{X_1=6}$.
Un esempio di evento naturale è uno di quelli che compongono l'elemento composto, ad es $\set{X_1=4}$

# probabilità classica (uniforme)
con probabilità classica si intende quando i casi possibili sono in un insieme finito e la probabilità di un evento è definita come il numero di casi favorevoli su tutti i casi possibili.
es: evento {esce l'asso di bastoni} tale proababilità sarà 1/40 ovvero la probabilità che esca la carta selezionata tra le complessive 40 carte.
# probabilità condizionata
La probabilità cambia in base alle informazioni che si hanno, se uno spettatore estraesse una carta dalle 40 carte e dicesse "è uscito un asso", le probabilità che sia uscito l'asso di bastoni, non è più 1/40, ma 1/4.