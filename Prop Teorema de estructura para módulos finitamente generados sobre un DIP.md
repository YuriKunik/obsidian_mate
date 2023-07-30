
## Enunciado

Sea $A$ un [[Dominio de ideales principales]], $M$ un $A$-[[Módulo]] [[finitamente generado]]. Entonces existen $n \in \mathbb{N}$ y $d_{1},d_{2},\dots,d_{n} \in A$ tales que 

$$
M \cong \bigoplus_{i=1}^{n}\frac{A}{<d_{i}>} 
$$
además $d_{1}|d_{2}, d_{2}|d_{3}, \dots, d_{n-1}|d_{n}$

## Demostración

Sean $A$ y $m$ como en el enunciado, $M$ es finitamente presentado (por [[Prop en noeth finitamente generado implica finitamente presentado|prop nfgifp]]) entonces $\exists \alpha \in A^{r\times s}$, [[Matriz en anillos]], tal que $M \cong \text{coker}(\bar{\alpha})$:
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A^s & A^r & M & 0 \\
\arrow["\bar{\alpha}", from=1-1, to=1-2]
\arrow["\pi", from=1-2, to=1-3]
\arrow["", from=1-3, to=1-4]
\end{tikzcd}
\end{document}
```
Por [[Prop diagonalización sobre DIPs|prop dsdip]] $\exists \beta=\text{diag}(d_{1},\dots,d_{N})$, $<d_{1}> \supset<d_{2}> \supset\dots\supset<d_{N}>$  tal que $\alpha \equiv \beta$, entonces, por [[Prop equivalencia de matrices implica isomorfismo de cokers]] y [[Ejemplo básico de matriz diagonal en módulos]]:

$$
M \cong \text{coker}(\bar{\beta}) \cong \bigoplus_{i=1}^{N} \frac{A}{<d_{i}>}
$$