> Un **registro** è un componente che memorizza temporaneamente e gestisce informazioni binarie (bit) su un numero di posizioni, cioè un insieme di celle di memoria ([[flip-flop]]), per poter trasferire i bit tra i circuiti. Possono operare in parallelo o in serie.

Ogni flip-flop contenuto in un registro ha i seguenti ingressi:
# Ingressi sincroni
Cioè dipendenti dal clock: questi ingressi operano solo quando il clock è attivo (ad esempio, al fronte di salita o discesa). I due ingressi sincroni tipici di un flip-flop sono:

- **SET**: Imposta l'uscita del flip-flop a 1, quando il clock è attivo.
- **RESET**: Imposta l'uscita del flip-flop a 0, quando il clock è attivo.

# ingressi asincroni
Cioè indipendenti dal clock: sono usati per forzare il flip-flop in uno stato specifico, senza aspettare il ciclo di clock. I due ingressi asincroni più comuni sono:
    
- **PRESET**: Imposta (pone a 1) l'uscita del flip-flop in modo immediato, senza bisogno del clock.
- **CLEAR** (o RESET): Resetta (pone a 0) l'uscita del flip-flop in modo immediato, senza bisogno del clock.

> N.B.: PRESET si attiva quando è 1 (si dice ***active-high***) e CLEAR si attiva quando è 0 (si dice ***active-low***).

![[Pasted image 20250210173934 1.png]]

# tipi di registri

- [[registri di memorizzazione]]
- [[registro contatore]]