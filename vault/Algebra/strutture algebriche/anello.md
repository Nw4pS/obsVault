Un anello è una struttura algebrica $(A,+,\cdot)$ con un insieme e due operazioni binarie in cui:
- $A \neq \emptyset$ 
- $(A,+)$ è un gruppo abeliano (vale la proprietà commutativa su $+$)
- $(A,\cdot)$ è un semi-gruppo (vale la proprietà associativa su $(A,\cdot)$) 
- l'operazione $\cdot$ è distributiva rispetto a $+$ es: $a \cdot (b+c)=a \cdot b + a \cdot c$ , $\forall a,b,c \in A$
**Esempi di anello:**
- $(\mathbb{Z}, +, \cdot)$ ovvero i numeri interi
- [[matrici]]
- $(\mathbb{r}[x],+,\cdot)$ ovvero l'anello dei polinomi a coefficenti reali in una indeterminata x
Un anello si dice **unitario** se ha un elemento neutro (unità)

# Ideale
un ideale I è un sottoinsieme di un anello A con la seguente proprietà:
- è sottogruppo rispetto alla somma
- proprietà dell'assorbimento:
  $$\text{presi }i \in I, a \in A\text{ si ha che }i*a \in I \text{ ed } a*i \in I $$
se l'ideale non è commutativo, si deve distinguere tra ideali destri e sinistri