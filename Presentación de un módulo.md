
## Enunciado

Un $A$-[[Módulo]], $M$, es presentado por $r:A^{(I)}\to A^{(J)}$ si tenemos la [[Sucesión exacta]]

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A^{(I)} & A^{(J)} & M & 0 \\
\arrow["r", from=1-1, to=1-2]
\arrow["\pi", from=1-2, to=1-3]
\arrow["", from=1-3, to=1-4]
\end{tikzcd}
\end{document}
```

o sea,

- $\pi$ es epi
- $\text{im}(r)=\text{ker}(\pi)$

($M\cong A^{(J)}/\text{im}(r)$)

## Observaciones

Si $I$ y $J$ son finitos, $r$ queda determinado por

$$r(e_{i}) = r_{i} = (r_{ij})_{j\in J}$$

con lo cual $\text{im}(r) = <(r_{ij})_{j\in J}, i \in I>$ Es decir $\text{im}(r)$ es generado por 'las filas de r'.

Con esta misma óptica, si $I = J$, $r(e_{i})= a_{i} e_{i}$ entonces decimos que $r$ es una matriz diagonal, $r_{ij}=a_{i}\delta_{ij}$. En este caso tenemos la siguiente cadena de isomorfimos

$$
\begin{align}
M &= \frac{A^{(I)}}{<a_{i}e_{i},i \in I>} \\
	&= \frac{\oplus_{i \in I}(<e_{i}>)}{\oplus_{i \in I}<a_{i}e_{i}>} \\
	& \cong \bigoplus_{i \in I} \frac{<e_{i}>}{<a_{i}e_{i}>}  \\
	& \cong \bigoplus_{i\in I} \frac{A}{Aa_{i}}
\end{align}
$$

