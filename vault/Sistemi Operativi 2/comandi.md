Ogni comando è composto da
- comando
- opzioni
- argomenti obbligatori
detta sinossi del comando
es:
```Bash
obsidian@debian:~$ rm -r cartella2
```
in cui:
- comando: `rm`
- opzioni: `-r`
- argomento: `cartella2`
## opzioni
le opzioni possono solitamente essere scritte in due modi:
- breve: -carattere
- lunga: --parola
### argomenti di opzioni
le opzioni possono avere argomenti, ad esempio --key=1, -k1 o -k 1, mentre le opzioni senza argomenti possono essere raggruppabili, quindi:
`-b -r -c` = `-brc` 
# manuale dei comandi
se non si conosce l'utilizzo o il funzionamento di un comando, si può utilizzare il manuale dei comandi (e non solo) per conoscerne le funzionalità:
```Bash
man ls
```
da come output:
```
LS(1)                            User Commands                            LS(1)

NAME
       ls - list directory contents

SYNOPSIS
       ls [OPTION]... [FILE]...

DESCRIPTION
       List  information  about  the  FILEs (the current directory by default).
       Sort entries alphabetically if none of -cftuvSUX nor  --sort  is  speci‐
       fied.

       Mandatory arguments to long options are mandatory for short options too.

       -a, --all
              do not ignore entries starting with .

       -A, --almost-all
              do not list implied . and ..

       --author
              with -l, print the author of each file
 Manual page ls(1) line 1 (press h for help or q to quit)
```