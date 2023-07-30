
## Enunciado
Sea $M$ un $A$-[[Módulo]], entonces $M$ es [[Módulo Noetheriano|noetheriano]] sii todo [[Sub-módulo]] de $M$ es finitamente generado

## Demostración

### $\implies$
Dado un submódulo $S$, tomemos $C$ el conjunto de submódulos de $S$ que son finitamente generados. Por ser $M$ noetheriano $C$ va a tener un elemento maximal, $T$. Para demostrar la ida nos alcanza ver que $T=S$. Si existiera un $s\in S-T$, entonces $T \oplus s$ sigue siendo un submódulo de $S$ y es finitamente generado, por lo tanto $T=S$ lo que nos dice que $S$ es finitamente generado.

### $\Leftarrow$

Sea $(S_{i})_{i \in \mathbb{N}}$ una cadena creciente de submódulos de $M$. Sea $S=\cup S_{i}$ entonces $S$ es submódulo de $M$ y por lo tanto finitamente generado, $S = <s_{1},\dots, s_{n}>$ con $s_{j}\in S$ entonces $\exists N \in \mathbb{N}$ tal que $s_{i}\in S_{N}$ para todo $i$. por lo tanto la cadena $(S_{i})_{i \in \mathbb{N}}$ se estaciona en $S_{N}$.



