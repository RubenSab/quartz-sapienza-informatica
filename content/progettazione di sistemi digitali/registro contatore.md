> Servono per cadenzare le attività di altri moduli. Non hanno un input perché i [[flip-flop]] reagiscono solo al fronte d'onda del clock.

Possono essere **sincroni** o **asincroni**.

# asincroni o a cascata

## caratteristiche

- Il **primo flip-flop** è attivato direttamente dal segnale di clock.
- Gli altri flip-flop sono attivati dall'uscita del flip-flop precedente, creando un effetto "**a cascata**" (ripple).
- Più lento rispetto al contatore sincrono, perché ogni flip-flop introduce un ritardo di propagazione.

## tipi

- [[contatore asincrono modulo 2 alla n]]
- [[contatore asincrono preselezionabile]]
- [[contatore asincrono con reset]]

# sincroni

## caratteristiche
- Tutti i flip-flop ricevono il clock in **modo simultaneo**.
- Non c'è effetto di propagazione del ritardo tra i flip-flop.
- Più veloce rispetto al contatore asincrono.
- Circuito più complesso perché richiede una logica combinatoria per aggiornare gli stati.

> N.B.: nei contatori sincroni il LSB è sempre memorizzato primo flip flop (il più vicino al clock), mentre il MSB è memorizzato nell'ultimo.

## tipi
- [[contatore sincrono modulo 2 alla n]]
- [[contatore sincrono bidirezionale]]
- [[contatore con abilitazione al conteggio]]
- [[contatore di eventi]]