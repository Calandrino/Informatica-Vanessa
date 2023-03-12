# Verifica di un numero di carta di credito
L'ultima cifra di un numero di carta di credito è la **cifra di controllo**, che protegge il sistema da errori di trascrizione, come un errore che riguardi una singola cifra o lo scambio di due cifre.
Il metodo seguente è quello effettivamente utilizzato per verificare la validità dei numeri di carta di credito, ma, per semplicità, lo descriveremo nel caso di numeri di 8 cifre anziché 16.

Ipotizziamo che il numero da verificare di carta di credito sia: 43589795

* Partendo dalla cifra più a destra, sommate **tutte le cifre in posizione dispari** (l'indice 0 indica la posizione 1!) (quindi 5 + 7 + 8 + 3 = 23);
* **Raddoppiate tutte le cifre** che NON hanno fatto parte della somma precendente, poi, **sommate tutte le cifre dei numeri** così generati.
Nell'esempio precedente, il raddoppio dei numeri che non hanno fatto parte della somma sono: 18 18 10 8 (da 9 9 5 4); la somma quindi sarà: 1 + 8 + 1 + 8 + 1 + 0 + 8 = 27
* **Sommate le due somme** ottenute ai punti precedenti. Se l'**ultima cifra** del risultato è **0**, allora il numero della carta è **valido** (nell'esempio proposto si ha 23 + 27 = 50, quindi il numero della carta è valido).

Scrivete un programma che implementi questo algoritmo. L'utente deve fornire un numero di 8 cifre e il programma deve visualizzare un messaggio che dica se il numero della carta è valido o no.

Nel caso in cui il numero della carta non sia valido, il programma deve anche stampare a video il numero che la cifra di controllo dovrebbe avere per far sì che il numero sia valido.

#### Esempio di output 1
```
> Inseire un numero di 8 cifre: 43589795

Numero della carta valido
```

#### Esempio di output 2
```
> Inseire un numero di 8 cifre: 12345678

Numero della carta NON valido
Cifra di controllo valida: 4
```



