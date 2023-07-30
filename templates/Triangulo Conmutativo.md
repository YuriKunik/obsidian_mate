```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A & B\\
C
\arrow["f", from=1-1, to=1-2]
\arrow["g", swap,from=1-1, to=2-1]
\arrow["h", swap, from=2-1, to=1-2]
\end{tikzcd}
\end{document}
```