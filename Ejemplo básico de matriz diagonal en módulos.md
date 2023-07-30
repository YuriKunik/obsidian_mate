
## Ejemplo

Sea el $A$-[[Módulo]] $M=\oplus_{i=1}^{r}A / <d_{i}>$, entonces $M$ tiene la [[Presentación de un módulo|presentación]]

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A^r & A^r & M & 0 \\
\arrow["\psi", from=1-1, to=1-2]
\arrow["\varphi", from=1-2, to=1-3]
\arrow["", from=1-3, to=1-4]
\end{tikzcd}
\end{document}
```
con $\varphi=\oplus \pi_{i}$ y $\psi(e_{i})=d_{i}e_{i}$