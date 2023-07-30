
## Enunciado

### Forma algebraica
Sea $N$ un $A$-[[Módulo]], sean $f_{j}:N\to M_{j}$ [[Morfismo de módulos]]. Entonces existe un único $f:N\to \times_{i \in I}M_{i}$ tal que el siguiente diagrama conmuta para todo $j \in I$

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
N & \times_{i 
\in I} M_i\\
& M_{j}
\arrow["f", from=1-1, to=1-2]
\arrow["f_j", swap,from=1-1, to=2-2]
\arrow["\pi_j", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

a $f$ la llamamos $\bigtimes f_{i}$.

### Forma categórica
El producto es un cono universal en la categoría de conos dados por el funtor identidad.

Esta categoría tiene como conos

```tikz
\usepackage{amsfonts}
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	 N & & M \\
			\\
	 & M_j & \\
	\arrow[swap, "\phi_j", from=1-1, to=3-2]
	\arrow["\psi_j", from=1-3, to=3-2]
	\arrow["f", from=1-1, to=1-3]
\end{tikzcd}
\end{document}
```
y que sea un límite, nos dice que 
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
\times_{j\in I} M_j \\
M_j
\arrow["\pi_j", from=1-1, to=2-1]
\end{tikzcd}
\end{document}
```
es un objeto final.