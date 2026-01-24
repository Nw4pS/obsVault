
un database è un insieme strutturato di dati, immagina un database come un insieme di tabelle ("studenti", "professori", "esami"), ogni ennupla di una tabella rappresenta dei dati collegati tra di loro:

| nome  | cognome | matricola | nascita    |
| ----- | ------- | --------- | ---------- |
| paolo | brosio  | 321321    | 16/03/1999 |
| mario | moro    | 432432    | 12/08/2000 |
in questo caso rappresentano uno studente.
Le tabelle sono create e modificate tramite delle query SQL che possono anche utili per delle operazioni.
## transazioni
È importante tenere a mente il concetto di roll-back, ovvero se un operazione viene annullata si deve poter tornare indietro, questo è possibile tramite un transaction log. Si devono anche gestire le competizioni allo stesso dato
## DBMS
Un dbms è un sistema di management per gestire i database, che in questo corso vedremo quello relazionale.
## Modello Relazionale
### definizioni
 ![[Pasted image 20250923150457.png]]
 ![[Pasted image 20250923150610.png]]
 ![[Pasted image 20250923150649.png]]
 ![[Pasted image 20250923150749.png]]
 ![[Pasted image 20250923151400.png]]
 quindi uno schema di un database è l'insieme di schemi, il database è l'istanza dello schema.
 ![[Pasted image 20250923151737.png]]
![[Pasted image 20250923153624.png]]
![[Pasted image 20250923153737.png]]
![[Pasted image 20250923154504.png]]
![[Pasted image 20250923155313.png]]
### riferimenti e valori nulli
 i riferimenti ad altre tabelle del database vengono effettuati tramite i valori, es:
 ![[Pasted image 20250923152930.png]]
 questo viene effettuato tramite key, ovvero chiavi univoche che rappresentano una relazione, in questo caso la matricola e il codice del corso. Le chiavi, al contrario di altri campi, non possono essere Null

### vincoli di integrità
i vincoli di integrità servono a risolvere eventuali ambiguità:
![[Pasted image 20250923153639.png]]
### chiavi primarie e secondarie
![[Pasted image 20250923154237.png]]
![[Pasted image 20250923154507.png]]
![[Pasted image 20250923154526.png]]
### anomalie
![[Pasted image 20250923155305.png]]
