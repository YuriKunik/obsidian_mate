#construcciones #categorias #definiciones 
# Definición

Dado un [[diagrama]] $F$, la categoría de [[cono|conos]] tiene:
1. Conos hacia $F$ como objetos.
2. Morfismos tales que el siguiente diagrama conmuta $\forall X, Y\in J$ 
```tikz
\usepackage{amsfonts}
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	 & N & \\
		&L&	\\
	 F(X) & & F(Y)
	\arrow ["u", from=1-2, to=2-2]
	\arrow[swap, "\phi_X", from=2-2, to=3-1]
	\arrow["\phi_Y", from=2-2, to=3-3]
	\arrow[bend right, swap, "\psi_X", from=1-2, to=3-1]
	\arrow[bend left, "\psi_Y", from=1-2, to=3-3]
	\arrow["F(f)", from=3-1, to=3-3]
\end{tikzcd}
\end{document}
```
