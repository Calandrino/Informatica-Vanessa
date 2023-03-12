# Numeri romani
Scrivete un programma che converta un numero intero positivo nel corrispondente valore espresso nel sistema di numerazione romano.

I numeri romani sono costituite da 6 diverse cifre:

```
I     1
V     5
X     10
L     50
C     100
D     500
M     1000
```
I numeri romani vengono composti seguendo queste regole:

* Si possono rappresentare soltanto numeri fino a **3999**;
* Come nel sistema decimale, le migliaia, le centinaia, le decine e le unità vengono espresse separatamente;
* I numeri da 1 a 9 sono rappresentati, in ordine crescente, da I, II, III, IV, V, VI, VII, VIII, IX: 
* Come si può notare, una lettera che precede la lettera V o X rappresenta una unità che deve essere **sottratta** dal valore;
* Non si posso avere più di tre I consecutive;
* Le decine e le centinaia sono gestite allo stesso modo, tranne per il fatto che, al posto delle lettere I, V, X, si usano le lettere X, L, C e, rispettivamente, le lettere C, D, M.

#### Esempio di output
```
> Inserire un numero intero: 1978

Numero romano corrispondente: MCMLXXVIII
```
