
## Enunciado

Sea $A$ un [[Anillo]] conmutativo, si $P\subset A$ es [[Ideal maximal|maximal]] entonces $P$ es [[Ideal Primo|primo]].

## Demostración

Sabiendo que, sea $J$ [[Ideal]] tal que $P \subset J \subsetneq A \implies P=J$ queremos ver que, si $a\cdot b\in P \implies a\in P \text{ o } b \in P$. Si $a\in A,~ a\notin P$ entonces $J = P + Aa$ es ideal, $P\subsetneq J$. Entonces $J=A$, esto nos dice que $e=p+r\cdot a$. Multiplicando a ambos lados por $b$ obtenemos$b=b\cdot p + b\cdot r\cdot a = b\cdot p+ r \cdot b\cdot a$, que, al ser suma de elementos de $P$ un ideal, está en $P$. Con esto demostramos que $b\in P$ asumiendo que $a\notin P$ lo cual nos da lo deseado.
