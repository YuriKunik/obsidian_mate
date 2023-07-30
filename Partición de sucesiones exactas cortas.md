
## Definición

Decimos que una [[Sucesión exacta corta]] de $A$-[[Módulo|módulos ]]se parte si existe $\theta:M \to N\oplus P$ tal que

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
0 & N & M & P & 0 \\
0 & N & N\oplus P & P & 0
\arrow[" ", from=1-1, to=1-2]
\arrow["f", from=1-2, to=1-3]
\arrow["g", from=1-3, to=1-4]
\arrow[" ", from=1-4, to=1-5]
\arrow[" ", from=2-1, to=2-2]
\arrow["i", from=2-2, to=2-3]
\arrow["\pi", from=2-3, to=2-4]
\arrow[" ", from=2-4, to=2-5]
\arrow["id", from=1-2, to=2-2]
\arrow["\theta", from=1-3, to=2-3]
\arrow["id", from=1-4, to=2-4]
\end{tikzcd}
\end{document}
```
