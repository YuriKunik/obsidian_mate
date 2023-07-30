
## Enunciado

Sea $A$ un [[Dominio de ideales principales]], $M$ un $A$-[[Módulo]], que, por el [[Prop Teorema de estructura para módulos finitamente generados sobre un DIP| teorema 1 de estructura]] se escribe como: 
$$
M \cong \bigoplus_{i=1}^{N}A / <d_{i}>,
$$
con $<d_{1}> \supset <d_{2}> \supset \dots \supset <d_{N}>$. Tomando $m$ tal que 
$$
\begin{align}
d_{i}\neq 0  &\quad \text{para} \quad i\leq m \\

d_{i}= 0  &\quad \text{para} \quad i > m \\
\end{align}
$$
entonces
$$
M \cong \bigoplus_{i=1}^{m}A / <d_{i}> \oplus A^{N-m}.
$$
## Observación

Con esto, el [[Módulo de torsión]] cumple
$$
t(M) \cong \bigoplus_{i=1}^{m} \frac{A}{<d_{i}>}
$$
y, por lo tanto

$$
M / t(M) \cong A^{N-m}
$$
en particular, $M / t(M)$ es un [[Módulo libre]].