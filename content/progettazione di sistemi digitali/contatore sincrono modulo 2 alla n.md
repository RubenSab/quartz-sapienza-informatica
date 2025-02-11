# esempio mod 8 ($2^3$ bit)

Realizzazione con i [[flip-flop (JK)]]

![[Pasted image 20250211204411.png]]

Realizzazione con i [[flip-flop toggle (T)]]

![[Pasted image 20250211204436.png]]

Osserviamo che il primo flip-flop (quello del LSB) commuta sempre ad ogni fronte di salita del clock. Il secondo flip-flop commuta solo quando l'uscita del primo è a 1, mentre il terzo commuta quando le uscite dei primi due sono a 1.

> N.B.: Nei contatori sincroni, ogni flip flop dal terzo incluso in poi commuta solo quando l'uscita degli ultimi due flip-flip sono a 1. Ciò permette di raddoppiare il tempo di commutazione di ogni cifra dalla meno significante alla più significante.

![[Pasted image 20250211210239.png]]

*(foto e descrizioni da [elemania.altervista.org](https://www.elemania.altervista.org/digitale/contatori/cont5.html))*

> N.B.: Volendo costruire un contatore che conta alla rovescia, basterebbe semplicemente usare le uscite complementate dei flip-flop invece che le uscite normali.