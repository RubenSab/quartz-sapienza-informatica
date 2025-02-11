> Un **registro** è un componente che memorizza temporaneamente e gestisce informazioni binarie (bit) su un numero di posizioni, cioè un insieme di celle di memoria ([[flip-flop]]), per poter trasferire i bit tra i circuiti. Possono operare in parallelo o in serie.

- **Ingressi sincroni** (dipendenti dal clock): Questi ingressi operano solo quando il clock è attivo (ad esempio, al fronte di salita o discesa). I due ingressi sincroni tipici di un flip-flop sono:

    - **Set**: Imposta l'uscita del flip-flop a 1, quando il clock è attivo.
    - **Reset**: Imposta l'uscita del flip-flop a 0, quando il clock è attivo.

- **Ingressi asincroni** (indipendenti dal clock): Sono usati per forzare il flip-flop in uno stato specifico, senza aspettare il ciclo di clock. I due ingressi asincroni più comuni sono:
    
    - **Preset (o Set)**: Imposta (pone a 1) l'uscita del flip-flop in modo immediato, senza bisogno del clock.
    - **Clear (o Reset)**: Resetta (pone a 0) l'uscita del flip-flop in modo immediato, senza bisogno del clock.

![[Pasted image 20250210173934 1.png]]

- [[registri di memorizzazione]]
- [[registri contatori]]