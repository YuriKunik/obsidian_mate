
## Enunciado

Sea $H$ un [[Subgrupo Normal]] de un [[Grupo]] $G$. Entonces, para todo [[Morfismo de grupos]] $\varphi:G\to G'$ tal que $H \subseteq \text{ker}(\varphi)$ existe un único morfismo $\bar{\varphi}:G / H \to G'$ tal que el siguiente diagrama conmuta:
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
G & G'\\
G / H
\arrow["\varphi", from=1-1, to=1-2]
\arrow["\pi", swap,from=1-1, to=2-1]
\arrow["\exists! \bar{\varphi}", swap, from=2-1, to=1-2]
\end{tikzcd}
\end{document}
```

## Demostración

Tenemos la existencia de la función por [[Prop universal del cociente]] ya que la condición $H \subseteq \text{ker}(\varphi)$ nos dice que $\varphi$ es equivalente con la relación inducida por $H$. Nos falta ver que es compatible con la operación del grupo. pero eso vale por definición.