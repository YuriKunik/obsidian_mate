## Enunciado

Sea $A$ un [[Anillo]] conmutativo, $a \in A$ [[Elementos primos en A| elemento primo]] entonces es [[Elemento irreducible|irreducible]].
## Demostración

Buscamos demostrar que; si tenemos un elemento $b$ tal que $b | a \implies b\in A^{*}$ o $b\sim a$. Como $b|a$, $a=b\cdot x$ en particular $a|b\cdot x$ con lo que $a|b$ o $a|x$. Esto da lugar a la siguiente cadena de implicaciones
$$
\begin{align}
	a|b\cdot x &\implies a|b \text{ o } a|x \\
&\implies a\sim b \text{ o } x=aj \\
&\implies a\sim b \text{ o } a=baj \\
&\implies a\sim b \text{ o } b\in A^{*}
\end{align}
$$
