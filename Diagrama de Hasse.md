## Definición
Dado un [[Poset]] $X$, un diagrama de Hasse, $\mathscr{H}(X)$, es un digrafo con $x\to y$ si $x \prec y$. Lo dibujamos como.  
```tikz
\usepackage{amsfonts}
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	y \\
	. & y \\
	x 
	\arrow[no head, from=1-1, to=3-1]
	\arrow[" " , from=2-1, to=2-2]
\end{tikzcd}
\end{document}
```
## Ejemplo

```tikz
\usepackage{amsfonts}
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	& a &\\
	b & & c \\
	d & & d 
	\arrow[no head, from=1-2, to=2-1]
	\arrow[no head, from=1-2, to=2-3]
	\arrow[no head, from=2-1, to=3-1]
	\arrow[no head, from=2-3, to=3-3]
	\arrow[no head, from=2-1, to=3-3]
	\arrow[no head, from=2-3, to=3-1]
\end{tikzcd}
\end{document}
```
