L'algoritmo di Euclide viene utilizzato per trovare l'MCD di tra due numeri troppo grandi per la scomposizione in fattori primi
**algoritmo**:
1. si assegnano $a$ e $b$ in modo tale che $0\lt a \leq b$
2. si effettua $\frac{a}{b}$ e si salva il resto in r
3. si assegna $a=b$ e $b=r$
4. si continua fino ad avere resto 0. L'MCD sarà l'ultimo resto diverso da 0

**esempio**:
 1. $\frac{14743}{8915}=1 \text{ resto } 5828$
 2. $\frac{8915}{5828}= 1 \text{ resto } 3087$
 3. $\frac{5828}{3087}= 1 \text{ resto } 2741$
 4. $\frac{3087}{2741}= 1\text{ resto } 346$
 5. $\frac{2741}{346}=7 \text{ resto }319$
 6. $\frac{346}{319}= 1\text{ resto } 27$
 7. $\frac{319}{27}= 11 \text{ resto } 22$
 8. $\frac{27}{22}= 1 \text{ resto } 5$
 9. $\frac{22}{5}= 4\text{ resto } 2$
 10. $\frac{5}{2}= 2 \text{ resto } 1$
 11. $\frac{2}{1}= 2\text{ resto } 0$
 12. controllo quale sia il resto precedente a 0, ovvero $\text{MCD }(14743,8915)=1$
# trovare gli inversi

l'algoritmo può essere utilizzato anche per trovare gli inversi ovvero quei numeri che moltiplicati tra loro e divisi per il modulo, hanno resto 1
es:
per trovare l'inverso di 3 modulo 7
1. $\frac{7}{3}=2$ resto 1 ovvero $1= 7-3*2$
2. $\frac{3}{1}=3$ resto 0 
 abbiamo l'$MCD(7,3)=1$ quindi esiste l'inverso e possiamo identificarlo dall'identità di Bézout appena svolta $1= 7+ 3*(-2)$ in questo caso il numero è negativo quindi si prende il modulo e si sottrae il negativo $7-2=5$ infatti $\frac{3*5}{7}=2$ con resto 1
