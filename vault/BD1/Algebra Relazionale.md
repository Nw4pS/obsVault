![[Pasted image 20250923163426.png]]
![[Pasted image 20250923164647.png]]
![[Pasted image 20250923165127.png]]
**nota bene** che nella tabella di output c'è solo un "Rossi", questo perché le relazioni seguono le regole dell'insiemistica, quindi ogni elemento deve essere diverso, in questo caso ci basta effettuare una "proiezione" anche il codice $C\#$ con $\pi_{Name,C\#}(Customers)$ .

![[Pasted image 20250923170444.png]]
![[Pasted image 20250923171454.png]]![[Pasted image 20250923171506.png]]
![[Pasted image 20250923172438.png]]
![[Pasted image 20250923172551.png]]
**COMBO** 
è possibile effettuare delle combo, ad esempio:
![[Pasted image 20250923172635.png]]![[Pasted image 20250923172711.png]]
![[Pasted image 20250923173141.png]]![[Pasted image 20250923173243.png]]
![[Pasted image 20250923175606.png]]
![[Pasted image 20250923175844.png]]
cambiamo nome a C# di una delle due tabelle per evitare ambiguità
![[Pasted image 20250923175901.png]]
effettuiamo il prodotto cartesiano
![[Pasted image 20250923175913.png]]
selezioniamo le tuple che hanno C# e CC# identico, in questo modo stiamo selezionando le tuple dei reali ordini
![[Pasted image 20250923180112.png]]
![[Pasted image 20250923181721.png]]
![[Pasted image 20250923182500.png]]
![[Pasted image 20250923182526.png]]
![[Pasted image 20250923182609.png]]
![[Pasted image 20250923182746.png]]
![[Pasted image 20250923183011.png]]
![[Pasted image 20250925163051.png]]
![[Pasted image 20250925163127.png]]
![[Pasted image 20250925163143.png]]

![[Pasted image 20250925174235.png]]
ESEMPIO
![[Pasted image 20250925174359.png]]
![[Pasted image 20250925174811.png]]
quindi, per selezionare una condizione sempre vera, ci basta creare una tabella in cui sono presenti le tuple in cui è falsa, e rimuovere dalla tabella originale, quelle che compaiono in quella falsa, ad esempio controllando nome e cognome, oppure con un id