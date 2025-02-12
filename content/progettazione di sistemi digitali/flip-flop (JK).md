*J e K sono etichette arbitrarie per i due input del flip-flop*

> Un flip-flop JK differisce da un [[flip-flop set-reset (SR)]] solamente dal fatto che quando i due input sono a 1, l'output del flip-flop è il complemento dello stato memorizzato l'istante precedente.

# funzionamento

| J   | K   | y(t+1)            |
| --- | --- | ----------------- |
| 0   | 0   | $y(t)$            |
| 0   | 1   | 0                 |
| 1   | 0   | 1                 |
| 1   | 1   | $\overline{y(t)}$ |

## tabella di verità

| y(t) | J   | K   | y(t+1) |
| ---- | --- | --- | ------ |
| 0    | 0   | 0   | 0      |
| 0    | 0   | 1   | 0      |
| 0    | 1   | 0   | 1      |
| 0    | 1   | 1   | 1      |
| 1    | 0   | 0   | 1      |
| 1    | 0   | 1   | 0      |
| 1    | 1   | 0   | 1      |
| 1    | 1   | 1   | 0      |

## espressione booleana

espressione booleana di $y(t+1)$ in funzione di $y(t), J, K$:

$$y(t+1)=\overline{y(t)}\cdot J + y(t)\cdot\overline{K}$$
# realizzazione

Nel disegno sotto $y(t)=Q$ e $y(t+1)=y$, quindi vale che $y=\overline{Q}\cdot J + Q\cdot\overline{K}$

![[flip flop JK.svg]]