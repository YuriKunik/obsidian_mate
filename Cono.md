#categorias #definiciones #matemática 
## Definición

Dado un [[Diagrama]] $D: J \to \mathscr{C}$, $N$ un objeto de $\mathscr{C}$. Un cono de $N$ a $D$ es una familia de morfismos $\psi:N \to D(X)$ para cada $X\in ob(J)$ tal que el siguiente diagrama conmuta:
```tikz
\usepackage{amsfonts}
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	 & N & \\
			\\
	 D(X) & & D(Y)
	\arrow[swap, "\psi_X", from=1-2, to=3-1]
	\arrow["\psi_Y", from=1-2, to=3-3]
	\arrow["D(f)", from=3-1, to=3-3]
\end{tikzcd}
\end{document}
```
A $N$ se le dice vértice y a $D$ base.

## Intuición

Se tiene un objeto que está por arriba de todos los objetos que vienen como imagen del funtor $D$. La idea es que $N$ tiene flechas copadas a cada par de la imagen del funtor.