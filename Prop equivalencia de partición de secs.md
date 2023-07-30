
## Enunciado

Dada una [[sucesión exacta corta]] de $A$-[[Módulo|modulos]]
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
0 & N & M & P & 0 \\
\arrow["", from=1-1, to=1-2]
\arrow["f", from=1-2, to=1-3]
\arrow["g", from=1-3, to=1-4]
\arrow["", from=1-4, to=1-5]
\end{tikzcd}
\end{document}
```
tenemos que son equivalentes

1. $f$ es una [[sección]].
2. $g$ es una [[retracción]].
3. La [[Partición de sucesiones exactas cortas|sucesión exacta corta se parte]].