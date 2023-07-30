
## Definición

Dado un [[Grupo]] $G$, tenemos la [[Categoría]] conformada por

1. $\text{Ob(G-Ens)}:=$ Conjuntos $A$ con una $G$ [[Acción de grupo|acción]] sobre ellos
2. $\text{Fl(G-Ens)}:=$ Funciones de conjuntos tales que conmuta
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
G \times A & G \times A'\\
A & A'
\arrow["id_G \times \varphi", from=1-1, to=1-2]
\arrow["\rho", swap,from=1-1, to=2-1]
\arrow["\rho'", from=1-2, to=2-2]
\arrow["\varphi", swap, from=2-1, to=2-2]
\end{tikzcd}
\end{document}
```
es decir, $\varphi$ saca afuera a los actuantes. a estos elementos se les dice equivariantes.
