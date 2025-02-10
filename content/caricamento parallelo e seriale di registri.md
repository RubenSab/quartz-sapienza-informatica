# Caricamento parallelo
## con i [[flip-flop delay (D)]]

Un'array di FF D da sola non può caricarsi parallelamente perché non dispone di una linea di LOAD, cioè un segnale di ENABLE condiviso tra tutti i flip-flop che fa passare tutti i bit nelle loro rispettive celle di memoria allo stesso momento.
![[caricamento parallelo.svg]]
Tuttavia, aggiungendo una linea di LOAD e una serie di circuiti di controllo abbinati ai flip flop, ognuno composto da 2 [[AND gate con funzione di controllo]] che confluiscono in una porta OR, avremo che:
- quando LOAD = 0, tutti i flip-flop conserveranno il valore corrente (memorizzazione)
- quando LOAD = 1, tutti i flip-flop assumeranno il valore dell'entrata corrispondente alla loro posizione del registro ($Q_{n}\to n$).
![[registro D.svg]]
## con i [[flip-flop set-reset (SR)]] e [[flip flop JK.svg]]

Se non si considera la linea di LOAD, la procedura è identica alla precedente in entrambi i casi perché negando il segnale che entra in S (o J) e facendolo entrare in R (o K) otteniamo un FF D.  

![[caricamento e memorizzazione con FFSR.svg]]

Considerando la linea di LOAD, il circuito invece cambia perché:
- **S** deve essere uguale a 1 se LOAD = 1 e l'entrata corrispondente = 1
- **R** deve essere uguale a 0 se LOAD = 1 e l'entrata corrispondente = 0

![[caricamento con FFSR.svg]]
# Caricamento seriale
![[caricamento seriale.svg]]
Questa configurazione di flip-flop può caricarsi serialmente ma è ancora incapace di memorizzare.

```
Esempio:

input seriale = 1011

t0: ----
t1: 1---
t2: 11--
t3: 011-
t4: 1011 > l'input seriale viene caricato completamente
t5: -101
t6: --10
t7: ---1
t8: ---- > l'input seriale viene perso
```