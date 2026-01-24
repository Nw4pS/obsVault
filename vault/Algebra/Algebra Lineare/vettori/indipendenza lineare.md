dato uno spazio vettoriale V su K, un insieme di vettori viene detto linearmente indipendente se e solo se:
$$\lambda_1v_1+...+\lambda_n v_n=0 \iff \lambda_1,...,\lambda_n=0$$
ovvero che per far si che la combinazione lineare di questo insieme di vettori dia un vettore nullo, ogni scalare deve essere 0, altrimenti l'insieme verrebbe definito come linearmente indipendente.
Un altro modo di vederla è "un insieme si dice linearmente dipendente se posso scrivere un vettore dell'insieme come combinazione lineare di altri vettori dell'insieme"
## estensione a generatore
dati dei vettori linearmente indipendenti $v_1,...,v_n \in span(w_1,...,w_n)$ in cui $n\leq k$ (il numero di vettori linearmente indipendenti non può superare il numero dei vettori generatori, altrimenti si avrebbe per forza un vettore dipendente) allora: $$\exists (v_{k+1},...,v_n) | span(v_1,...,v_n)=span(w_1,...,w_n)$$
>ovvero che è possibile generare uno spazio vettoriale usando solamente vettori linearmente indipendenti, ma che questi vettori devono essere minori del numero di generatori originali