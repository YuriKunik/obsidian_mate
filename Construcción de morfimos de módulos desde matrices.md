
## Construcción

Sea $A$ un [[Anillo]], $\alpha \in A^{r\times s}$ entonces $\bar{\alpha}:A^{s} \to A^{r}$ es un morfismo de [[Módulo libre|módulos libres]] inducido por $\alpha$, $\bar{\alpha}(x)=\alpha x$, $x \in A^{s}=A^{s\times1}$. 
Con esto tenemos el módulo $M=\text{coker}(\bar{\alpha})=\frac{A^{r}}{\text{im}(\bar{\alpha})}$ que tiene la [[Presentación de un módulo|presentación]]:
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A^s & A^r & M & 0 \\
\arrow["\bar{\alpha}", from=1-1, to=1-2]
\arrow["\pi", from=1-2, to=1-3]
\arrow["", from=1-3, to=1-4]
\end{tikzcd}
\end{document}
```

