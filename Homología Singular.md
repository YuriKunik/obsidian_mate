#construcciones #topoalg #matemática 
## Definición
La homología singular de un espacio $X$ es la homología dada por la [[Cadena de Complejos]]

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	\dots & C_{n+1}(X) & C_n(X) & \dots & C_1(X) & C_0(X) & 0
	\arrow["\partial_{n+1}", from=1-1, to=1-2]
	\arrow["\partial_{n}", from=1-2, to=1-3]
	\arrow["\partial_{2}", from=1-3, to=1-4]
	\arrow["\partial_{1}", from=1-4, to=1-5]
	\arrow["\partial_{0}", from=1-5, to=1-6]
	\arrow["", from=1-6, to=1-7]
\end{tikzcd}
\end{document}
```


Con $C_n(X)$ el grupo abeliano libre generado por las funciones continuas $\sigma : \Delta^n \rightarrow X$. Y morfismos $\partial_n : C_{n+1}(X) \rightarrow C_n(X)$  que mandan
$$
\partial_n(\sigma) = \sum_{i} (-1)^{i} \sigma|_{[v_0, \dots,    \hat{v_i}, \dots v_n]}
$$
Las funciones $\partial_n$ son llamadas **morfismos de borde** y las funciones $\sigma$ [[n simplex singular |n-simplices singulares]].
Finalmente, el n-ésimo grupo de homología simplicial lo podemos definir como $H_n(X) = ker(\partial_n)/Im(\partial_{n+1})$.