#definiciones #categorias #propiedades_universales
## Definición
Dada una [[categoría]] $\mathscr{C}$  y dos flechas

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A & Y\\
X 

\arrow["f", from=1-1, to=1-2]
\arrow["g", from=1-1, to=2-1]
\end{tikzcd}
\end{document}
```

Un **pushout** es un objeto $Z$ junto con dos pares de flechas $\hat{f}, \hat{g}$  tal que el siguiente diagrama conmuta

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A & Y\\
X & Y \cup_f X\\
\arrow["f", from=1-1, to=1-2]
\arrow["\bar{f}", from=2-1, to=2-2]
\arrow["g", from=1-1, to=2-1]
\arrow["\bar{g}", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```
 y cumple la propiedad universal:

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A & Y\\
X & Y \cup_f X\\
&& Z
\arrow["f", from=1-1, to=1-2]
\arrow["\bar{f}", from=2-1, to=2-2]
\arrow["g", from=1-1, to=2-1]
\arrow["\bar{g}", from=1-2, to=2-2]
\arrow["h_X",bend right, from=2-1, to=3-3]
\arrow["h_Y",bend left, from=1-2, to=3-3]
\arrow["\exists! h", dotted, from=2-2, to=3-3]
\end{tikzcd}
\end{document}
```