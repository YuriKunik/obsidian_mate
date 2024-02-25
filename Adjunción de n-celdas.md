#topoalg #definiciones #construcciones 

## Definición
Una adjunción de una $n$-celda es el siguiente [[Espacio de adjunción]] 
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
 S^{n-1 }&& B\\
& ADJ &\\
D^n && B \cup_\phi D^n

\arrow["\varphi", from=1-1, to=1-3]
\arrow["\bar{\varphi}", from=3-1, to=3-3]
\arrow["i", from=1-1, to=3-1]
\arrow["\bar{i}", from=1-3, to=3-3]
\end{tikzcd}
\end{document}
```

En este caso notamos $B\cup_f D^n = B\cup e^n$ y decimos que se obtiene de B adjuntando una $n$-celda. Una $n$-celda es la imagen de $\mathbb{D}^n$ por $\bar{f}$ y la función $\bar{f}$ se llama función característica de la celda.