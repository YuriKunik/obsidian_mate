
## Enunciado

Seas $M$ y $M'$ $A$-[[Módulo|módulos]], $N$ un [[Sub-módulo]] de $M$ y $f:M\to M'$ un [[Morfismo de módulos]] tal que $f(N)=0$ ($N \subset \text{ker}(f)$), entonces el siguiente diagrama conmuta

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
M & M'\\
M / N
\arrow["f", from=1-1, to=1-2]
\arrow["\pi", swap,from=1-1, to=2-1]
\arrow["\bar{f}", swap, from=2-1, to=1-2]
\end{tikzcd}
\end{document}
```
