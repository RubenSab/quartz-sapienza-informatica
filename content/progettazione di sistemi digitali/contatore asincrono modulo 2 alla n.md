# esempio di contatore sincrono mod 8
Disegniamo lo schema dell'automa con il [[automi a stati finiti (finite state automata) con output|modello di Moore]].

![[automa contatore Moore.jpg]]

## Tavola degli stati futuri:

| $y_2 y_1 y_0$ | $Y_2 Y_1 Y_0$ | $j_2 k_2$  | $j_1 k_1$  | $j_0 k_0$  | $z_2 z_1 z_0$ |
| ------------- | ------------- | ---------- | ---------- | ---------- | ------------- |
| 000           | 001           | 0 $\delta$ | 0 $\delta$ | 1 $\delta$ | 000           |
| 001           | 010           | 0 $\delta$ | 1 $\delta$ | $\delta$ 1 | 001           |
| 010           | 011           | 0 $\delta$ | $\delta$ 0 | 1 $\delta$ | 010           |
| 011           | 100           | 1 $\delta$ | $\delta$ 1 | $\delta$ 1 | 011           |
| 100           | 101           | $\delta$ 0 | 0 $\delta$ | 1 $\delta$ | 100           |
| 101           | 110           | $\delta$ 0 | 1 $\delta$ | $\delta$ 1 | 101           |
| 110           | 111           | $\delta$ 0 | $\delta$ 0 | 1 $\delta$ | 110           |
| 111           | 000           | $\delta$ 1 | $\delta$ 0 | $\delta$ 1 | 111           |
## espressioni booleane

Ricaviamo le espressioni minimali delle [[rete sequenziale generica.canvas|funzioni di eccitazione]] dei [[flip-flop (JK)]].
$j_{0}=k_{0}=1$
$j_{1}=k_{1}=y_{1}\bullet y_{0}$ (ricavato dalla k-mappa di $y_{2}y_{1}y_{0}$)

## rappresentazione del circuito

![[contatore a cascata.jpg]]

> N.B.: Con un processo analogo si può progettare un contatore che usa dei [[flip-flop toggle (T)]] (tra l'altro molto più adatti per lo scopo) o uno in mod $n$ che conta al contrario da $n-1$ a $0$ (in quest'ultimo caso il circuito è uguale ma per ogni flip-flop si prende l'uscita con l'output negato piuttosto che l'output normale).

## diagramma temporale

> N.B.: I flip-flop cambiano stato sui fronti di salita del clock.

![[diagramma temporale contatore.jpg]]

