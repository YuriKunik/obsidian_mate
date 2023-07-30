
## Enunciado

Sea $N$ un $A$-[[Módulo]], sean $v_{j}:M_{j}\to N$ morfismos de $A$-módulos. Entonces existe un único morfismo $v:\oplus_{i\in I} M_{i}\to N$ que sale de la [[Suma directa de módulos|suma directa]] tal que conmuta

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
\bigoplus_{i\in I} M_i & N\\
M_j
\arrow["v", from=1-1, to=1-2]
\arrow["u_j", from=2-1, to=1-1]
\arrow["v_j", swap, from=2-1, to=1-2]
\end{tikzcd}
$\forall j \in I$
\end{document}
```
