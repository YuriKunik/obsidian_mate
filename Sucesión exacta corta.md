
## Definición

Una sucesión exacta corta es una [[Sucesión exacta]] con la siguiente forma

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
