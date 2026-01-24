
| comando        | significato                                                           |
| -------------- | --------------------------------------------------------------------- |
| .global  start | indica dove il programma ha inizio                                    |
| .text          | dove è scritto il codice                                              |
| .data          | sezione dove vanno inseriti i dati (credo sia dove si inizializzano ) |
|                |                                                                       |
|                |                                                                       |
|                |                                                                       |
|                |                                                                       |
# tipi di dato
- word: una word è un insieme di 32bit, i registri sono composti da word di n lunghezza. Per inizializzare una word si utilizza 
  ```RISC-V
  v1: .word 10 
  v2: .word 12
  v3: .word 14
  ...
  ```
# etichette
- start: inizio del codice scritto in text
- end: fine del codice scritto in text, verrà chiamata una syscall, ad esempio per uscire dal programma

è possibile aggiungere etichette a cui saltare, ad esempio per creare dei blocchi di codice da eseguire una volta verificata una condizione
# comandi
- la: load address, salva in un indirizzo di memoria un indirizzo di memoria es: `la t0, v1`
- li: load immidiate, salva in un indirizzo di memoria il valore scritto, es: `li t0, 10`
- lw: load word, salva una word in un indirizzo di memoria (salva il valore non l'indirizzo di memoria in cui il valore è salvato, come nel caso di la), 
  es: `lw t1, 0(t0)` in questo caso salva in t1, la word (quindi il valore) presente in t0+0, per salvare il valore presente nella word successiva, avrei utilizzato lw t1, 4(t0) poiché una word equivalgono a 4byte (32bit)
- sw: store word, immagazzina il valore contenuto in un indirizzo di memoria, in una word alla posizione offset(pos_origin), 
  esempio: `sw t5, 16(t0)` prende il valore contenuto in t5 e lo copia alla sedicesima word partendo da t0
- j per saltare da un'etichetta all'altra, 
  es: `j ciclo1`
## operazioni
- add: addizione tra variabili già inizializzate es: add t0, t0, t1
- addi: add immidiate, addiziona un valore alla variabile
  es: `addi t0, t0, 10`
  in cui la prima variabile è quella in cui andrà salvato il risultato e le altre due vanno sommate
- srai: shift right arithmetic immidiate, effettua una divisione con fattore 2, ad esempio
  `srai t5, t5, 2` effettua una divisione per 4, `srai t5, t5, 1` effettuerebbe la divisione per 2
# blocchi
per implementare i cicli, si utilizzano le condizioni branch che indirizzano a delle etichette e alla fine del blocco dell'etichetta, si utilizza un jump al controllo:
![[Pasted image 20251018190935.png]]

- bge: branch if greater than or equal, se la variabile è maggiore o uguale ad un valore, vai alla targhetta specificata
  ```RISC-V assembly language
  bge t0, zero, maggioreDiZero
  addi t0, t0, t1
  
  maggioreDiZero:
  addi t1, t1, 1
  ```
- ble: branch if less than or equal, se la variabile è minore o uguale ad un valore, vai alla targhetta specificata
- beq: branch if equal: se la variabile è uguale ad un valore
# creare ciclo for
per creare un ciclo for serve una condizione ed un jump ad una etichetta ciclo situata prima della condizione
```RISC-V
li t0, 0
li t1, 5
ciclo:
addi t0, t0, 1
beq t0, t1 end
j ciclo
end:

```
# syscall
1. si inserisce in a7, il valore corrispondente alla syscall che si vuole chiamare
2. si caricano valori da restituire (a0,a1,a2,a3,fa0,...)
3. si chiama la funzione ECALL