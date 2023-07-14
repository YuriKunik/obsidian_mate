#definiciones #topoalg #matemática 

## Definición
La homología simplicial reducida de un espacio $X$ viene dada por los grupos de homología dados por la [[Cadena de Complejos]]

```tikz
\usepackage{amsfonts}
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	 \dots & C_2(X) & C_1(X) & C_0(X) & \mathbb{Z} & 0
	\arrow["\partial_{2}", from=1-1, to=1-2]
	\arrow["\partial_{1}", from=1-2, to=1-3]
	\arrow["\partial_{0}", from=1-3, to=1-4]
	\arrow["\varepsilon", from=1-4, to=1-5]
	\arrow["", from=1-5, to=1-6]
\end{tikzcd}
\end{document}
```
 con $\varepsilon$ la misma que en la demostración de [[Homología singular, caso base]], $\varepsilon(\sum_i n_i \sigma_i)= \sum_i n_i$.
## Observación
Los grupos de homología reducidos $\tilde{H_n}$  coinciden para todo $n \leq 1$ y en $\tilde{H_n}$ vale $H_n \oplus \mathbb{Z}$ 
