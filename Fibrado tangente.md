Un **fibrado** sobre una [[Variedad topologíca diferenciable]] $M$ es una terna $(X, M, \pi)$ con $\pi :X\to M$ tal que, para cada $p \in M$ exista un entorno de $p$, $U$ tal que existe una variedad diferencial $Z$ y un [[difeomorfismo]] $h:\pi^{-1}(U)\to U \times Z$, tales que $\pi = pr_{1} \circ h$.

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
\pi^{-1}(U) & U \times Z\\
M
\arrow["h", from=1-1, to=1-2]
\arrow["\pi", swap,from=1-1, to=2-1]
\arrow["pr_1", swap, from=1-2, to=2-1]
\end{tikzcd}
\end{document}
```
