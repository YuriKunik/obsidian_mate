## Definición
Dado $A \subseteq X$, decimos que $i:A\to X$ es una cofibración si cumple la siguiente propiedad: $\forall Y$ espacio topológico, $f: X\to Y$, $H: A \times I \to Y$ continua
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A & X\\
A \times I & X \times I\\
&& Y
\arrow["i", from=1-1, to=1-2]
\arrow["i \times 1_I", from=2-1, to=2-2]
\arrow["i_0", from=1-1, to=2-1]
\arrow["i_0", from=1-2, to=2-2]
\arrow["H",bend right, from=2-1, to=3-3]
\arrow["f",bend left, from=1-2, to=3-3]
\arrow["\exists G", dotted, from=2-2, to=3-3]
\end{tikzcd}
\end{document}
```

A esta propiedad se la denomina propiedad de extensión de homotopías (PEH).

## Observaciones
1. El uso principal que se le da es el siguiente: Si $i: A\to X$ es una cofibración y $A$ es contráctil, entonces $f :X \to X/A$ es una equivalencia topológica.
2. La PEH es casi un [[pushout]], le falta la unicidad de la G.