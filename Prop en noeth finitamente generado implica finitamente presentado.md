
## Enunciado

Sea $A$ un [[Anillo noetheriano]], entonces todo $A$-[[Módulo]] finitamente [[Submódulo generado|generado]] es finitamente [[Presentación de un módulo|presentado]].

## Demostración

Tomemos generadores de $M$, $\{ m_{1},m_{2},\dots m_{r} \} \subset M$ entonces tenemos un epimorfismo:

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A^r & M & 0 \\
\arrow["\varphi", from=1-1, to=1-2]
\arrow["", from=1-2, to=1-3]
\end{tikzcd}
\end{document}
```
con $\varphi(e_{i})=m_{i}$.

Sea $S=\text{ker}(\varphi)\subset A^{r}$ como $A$ es noetheriano, $S$ es finitamente generado, eligiendo $\sigma_{1},\sigma_{2},\dots,\sigma_{s} \in S$ generadores entonces tenemos

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A^s & S & 0 \\
\arrow["\psi", from=1-1, to=1-2]
\arrow["", from=1-2, to=1-3]
\end{tikzcd}
\end{document}
```
con $\psi(b_{1},\dots, b_{s})= \sum_{i=1}^{d}b_{i}\sigma_{}{i}$. Esto nos da

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A^s & A^r & M & 0 \\
\arrow["\psi", from=1-1, to=1-2]
\arrow["\varphi", from=1-2, to=1-3]
\arrow["", from=1-3, to=1-4]
\end{tikzcd}
\end{document}
```
como [[Presentación de un módulo|presentación]].

