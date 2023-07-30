
## Enunciado

Sea $A$ un [[Anillo]] conmutativo, $S \subset A$ [[Subconjunto multiplicativo]]
1. $\varphi: A \to S^{-1}A$ es morfismo de anillos tal que $\forall s \in S$, $\varphi(s)\in S^{-1}A$ es inversible.
2. Si $\psi:A\to B$ es morfismo de anillos tal que $\psi(s)\subset B^{*}$.Entonces:

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A & B\\
S^{-1}A
\arrow["\psi", from=1-1, to=1-2]
\arrow["\varphi", swap,from=1-1, to=2-1]
\arrow["\bar{\psi}", swap, from=2-1, to=1-2]
\end{tikzcd}
\end{document}
```

## Idea Demostración

2. Definimos $\bar{\psi}\left( \frac{a}{s} \right)=\psi(a)\psi(s)^{-1}$. 

## Observación

Tenemos una proposición análoga para [[módulo|módulos]].