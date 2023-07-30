
## Enunciado

Sea $A$ un anillo, entonces son equivalentes

1. $A$ es un [[Anillo noetheriano]].
2. Todo $A$-[[Módulo]] finitamente generado es noetheriano.

## Demostración

### 1 $\implies$ 2

$A$ es un $A$-módulo finitamente generado por lo que es noetheriano como $A$-módulo, y esto es la definición de ser un anillo noetheriano.

### 2 $\implies$ 1

Dado $M$ un $A$-módulo finitamente generado, $M = <x_{1},x_{2},\dots,x_{n}>$ tenemos un morfismo epi $f:A^{n}\to M$. Por [[Prop Yoga de Noetherianos-Artinianos|Yoga de Noetherianos]] nos alcanza con ver que $A^{n}$ es Noetheriano. Veamos esto por inducción en $n$. El caso base lo tenemos por hipótesis. Para el paso inductivo, si $A^{n}$ es Noetheriano, tenemos la [[Sucesión exacta corta]]

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
0 & A^{n} & A^{n+1} & A & 0 \\
\arrow["", from=1-1, to=1-2]
\arrow["i", from=1-2, to=1-3]
\arrow["\pi", from=1-3, to=1-4]
\arrow["", from=1-4, to=1-5]
\end{tikzcd}
\end{document}
```
Como $A^{n}$ y $A$ son Noetherianos, volviendo a usar yoga, $A^{n+1}$ también lo es.