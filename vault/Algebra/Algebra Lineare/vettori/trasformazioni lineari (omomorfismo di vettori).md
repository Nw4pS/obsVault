una trasformazione lineare è un omomorfismo tra spazi vettoriali:
- $\forall v,v' \in V, f(v+v')=f(v)+f(v')$
- $\forall \lambda \in K, v \in V, f(\lambda v)= \lambda f(v)$ 

per immaginare meglio, si può pensare ad una trasformazione lineare come la luce del sole, essa colpisce un oggetto $K^3$ e lo traduce in un oggetto $K^2$ mantenendone la struttura interna, è possibile prendere due penne v e v', la somma della loro ombra sarà la stessa dell'ombra della loro somma.
Le trasformazioni lineari possono anche mantenere la stessa dimensione o aumentarla
# nucleo e immagine
poiché una trasformazione lineare non è altro che un omomorfismo, data una funzione $f:V \to W$ si hanno:
- nucleo: $ker(f)= v \in V | f(v)= 0_w$
- immagine: $im(f) =w \in W : \exists v \in V | f(v)=w$ 
# teorema del Rango
ricordiamo il primo teorema dell' [[isomorfismo]] $$\frac{\text{A}}{\ker(f)}\cong \text{im}(f)$$
dati:
- W e V spazi vettoriali
- $f: V \to W$
- rango di f $rk(f)$ corrispondente alla dimensione dell'immagine
si ha che $$rk(f)=dim(im(f))$$
per il primo teorema dell'isomorfismo, possiamo scrivere
$$im(f)\cong\frac{V}{ker(f)}$$

e quindi affermare che
>$$rk(f)=dim(im(f))=dim(V)-dim(ker(f))$$
