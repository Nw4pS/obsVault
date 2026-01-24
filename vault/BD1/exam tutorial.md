
# primo esercizio
## Dipendenze funzionali
### trovare le chiavi in uno schema
- **Trova i "Must-Have"**: Guarda tutti gli attributi. Quelli che **non compaiono MAI a destra** di una freccia `→` devono per forza far parte di **ogni chiave**. Iniziamo da loro.
    
- **Calcola la Chiusura Iniziale**: Prendi gli attributi "Must-Have" e calcola la loro chiusura. Per calcolare la chiusura `X+` , parti con `Z=X` e continua ad aggiungere attributi finché non puoi più aggiungerne, usando le dipendenze `Y→V` dove `Y` è già contenuto in `Z`.
- **Verifica e Aggiungi**:
    
    - Se la chiusura è già tutto lo schema `R`, hai trovato l'unica chiave. Finito!
        
    - Se no, aggiungi ai "Must-Have" uno alla volta gli altri attributi (parti da quelli che compaiono più spesso a sinistra) e ricalcola la chiusura.
        
- **Raggiunto `R`? Minimizza!**: Quando trovi un insieme `K` tale che `K+ = R`, controlla che sia minimo. Prova a togliere un attributo da `K` e vedi se la chiusura è ancora `R`. Se non lo è, allora `K` è una chiave.
### controllare se F è in 3NF
- **Prerequisiti**: Devi conoscere **tutte le chiavi** dello schema (esercizio E.1.1).
    
- **Identifica gli Attributi "Primi"**: Fai un elenco di tutti gli attributi che compongono le chiavi. Questi sono gli attributi "primi" o "pregiati". Tutti gli altri sono "non primi".
    
- **Analizza ogni Dipendenza**: Prendi ogni dipendenza `X → Y` dall'insieme `F`. Se `Y` ha più attributi, spezzettala (es. `A → BC` diventa `A → B` e `A → C`).
    
- **Applica il "Test 3NF"**: Per ogni dipendenza `X → A` (con `A` singolo attributo), poniti due domande:
	- **Domanda 1**: `X` è una superchiave? (Cioè, contiene una delle chiavi che hai trovato al punto 1?). Se sì, **OK!** 👍 Passa alla prossima dipendenza.
    
	- **Domanda 2 (solo se la 1 è NO)**: `A` (l'attributo a destra) è un attributo "primo"? (È nella lista che hai fatto al punto 2?). Se sì, **OK!** 👍 Passa alla prossima.
- **Conclusioni**:

	- Se hai risposto **NO a entrambe le domande** anche per una sola dipendenza, lo schema **NON È in 3NF**. Puoi fermarti.
    
	- Se tutte le dipendenze superano almeno una delle due domande, lo schema **È in 3NF**.

### controllare se la decomposizione preserva F
![[Pasted image 20251012200202.png]]
### controllare se la decomposizione ha un join senza perdita
![[Pasted image 20251021231900.png]]
![[Pasted image 20251021231913.png]]
in caso contrario si tiene la tabella modificata e si ricomincia con le dipendenze funzionali
### trovare una copertura minimale e decomposizione ottimale
![[Pasted image 20251015230814.png]]
1. quindi nella prima parte si dividono le dipendenze con due attributi a destra
2. nella seconda si cerca un sottoinsieme degli attributi X che se esteso contiene Y
3. nel terzo si controlla se esistono dipendenze che trovano Y senza utilizzare la dipendenza $X\rightarrow Y$
![[Pasted image 20251015230835.png]]
4. c'è almeno un sottoschema che contiene una chiave quindi ha un join senza perdita

### Organizzazione fisica
#### HDD
![[Pasted image 20251102023024.png]]
$\frac{ROT}{2}$ poiché ROT equivale al tempo impiegato dal disco per effettuare una rotazione completa, poiché il caso migliore è che sia 0 ovvero il blocco si trova esattamente dove si deve trovare per la lettura e il caso peggiore sia quello in cui il blocco sia appena passato, si divide per 2 per creare una media 
![[Pasted image 20251102023231.png]] 
$\frac{60000}{velA}$ poiché nel caso di 7200 rpm, ovvero 7200 rotazioni per minuto, viene trascorso un tempo di $\frac{1}{7200}$ e per tradurre questo tempo da minuti a millisecondi, è necessario tradurre il minuto in millisicendi $1min=60000ms$ 

Nel calcolo del transfer time viene moltiplicato il **transfer rate** per $2^{20}$ perché va tradotto in bytes poiché il valore è in megabyte e si sta utilizzando come dividendo un valore in bytes. infine il risultato della divisione deve essere moltiplicato per 1000 poiché va tradotto da secondi a millisecondi.
#### file heap e file sequenziali
![[Pasted image 20251102154909.png]]
![[Pasted image 20251102154931.png]]
per calcolare il tempo impiegato si deve prendere il numero degli accessi (NA) e moltiplicarlo per il tempo impiegato dagli algoritmi, RBA nel caso di una ricerca binaria, SBA nel caso di una ricerca sequenziale

#### hash
in hash, ogni blocco ha un puntatore per il blocco successivo, quindi lo spazio per il record è $\frac{BS-PS}{RS}$
#### ISAM
![[Pasted image 20251102182602.png]]

in isam il puntatore si trova nel file index
![[Pasted image 20251102182622.png]]
![[Pasted image 20251102182651.png]]
$(\log_2{NB_{FI}})+1 * RBA$ , in cui il +1 accesso si riferisce all'accesso all'effettivo blocco del file principale, poiché la ricerca viene effettuata nel file index.
![[Pasted image 20251102183125.png]]
in cui con "entrate per blocco" si intende quante key/index possono essere contenute in un blocco del file index, è il corrispettivo di "quanti record possono essere contenuti in un blocco"