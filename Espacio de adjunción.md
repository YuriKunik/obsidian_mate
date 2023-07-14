## Idea
Se busca pegar un espacio $X$ con otro $B$ mediante la imagen de una función continua que sale de un subespacio, $A$, de $X$.

## Definición

### Construcción
Sean $X$ y $B$ espacios topológicos, sea $A$ un subespacio cerrado de $X$ y $f: A \to B$ una función continua. El **espacio de adjunción** $B \cup_f X$ se define a partir de la unión disjunta $B \coprod X$ identificando los puntos $a \in A$ con los puntos $f(a)\in B$. Concretamente $B\cup_f X = B\coprod X / \sim$ con $\sim$ la relación de equivalencia generada por la relación $a \sim f(a)$ para todo $a\in A$. A la función $f: A \to B$ se la denomina función de adjunción. 

### Propiedad Universal

El espacio de adjunción es un [[pushout]] con las funciones $f : A \to B$ e $i: A \to X$,
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A & B\\
X & B \cup_f X\\
&& Z
\arrow["f", from=1-1, to=1-2]
\arrow["\bar{f}", from=2-1, to=2-2]
\arrow["i", from=1-1, to=2-1]
\arrow["\bar{i}", from=1-2, to=2-2]
\arrow["g_X",bend right, from=2-1, to=3-3]
\arrow["g_Y",bend left, from=1-2, to=3-3]
\arrow["\exists! g", dotted, from=2-2, to=3-3]
\end{tikzcd}
\end{document}
```
### Notación
Si tenemos un espacio de adjunción, notamos al diagrama:
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A && B\\
& ADJ &\\
X && B \cup_f X\\
\arrow["f", from=1-1, to=1-3]
\arrow["\bar{f}", from=3-1, to=3-3]
\arrow["i", from=1-1, to=3-1]
\arrow["\bar{i}", from=1-3, to=3-3]
\end{tikzcd}
\end{document}
```
