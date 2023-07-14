## Enunciado
Si $i: A\to X$ es una [[Cofibración]] cerrada tal que tenemos el siguiente [[Espacio de adjunción]]
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A && Y\\
& ADJ &\\
X && Y \cup_f X\\
\arrow["f", from=1-1, to=1-3]
\arrow["\bar{f}", from=3-1, to=3-3]
\arrow["i", from=1-1, to=3-1]
\arrow["\bar{i}", from=1-3, to=3-3]
\end{tikzcd}
\end{document}
```
entonces; si $f$ es una equivalencia homotópica, también lo es $\bar{f}$.
