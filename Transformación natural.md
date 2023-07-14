#matemática  #categorias #definiciones 
## Definición
Dados dos [[Funtor|funtores ]]$F,G : \mathscr{C} \to \mathscr{D}$, una transformación natural $\nu: F \Rightarrow G$ es una colección de flechas tal que
1. Para todo objeto, $X$ en la [[Categoría|categoría ]] $\mathscr{C}$ tiene asociada un morfismo $\nu_X: F(X) \to G(X)$. Este morfismo es llamado componente de $\nu$ en $X$.
2. Los componentes deben hacer que, dada una flecha, el siguiente diagrama conmute:
```tikz
\usepackage{tikz-cd}
\usepackage{amsfonts}
\begin{document}
\begin{tikzcd}
	F(X) & G(X) \\ 
	F(Y) & G(Y)
	\arrow["\nu_X", from=1-1, to=1-2]
	\arrow["F(f)", from=1-1, to=2-1]
	\arrow["G(f)", from=1-2, to=2-2]
	\arrow["\nu_Y", from=2-1, to=2-2]
\end{tikzcd}
\end{document}
```
Lo notamos con el siguiente diagrama

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}[]
C & \nu \Downarrow & D\\
\arrow[bend right,"F", from=1-1, to=1-3]
\arrow[bend left,"G", from=1-1, to=1-3]
\end{tikzcd}
\end{document}
```

