```tikz
\usepackage{amsfonts}
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	 & N & \\
			\\
	 F(X) & & F(Y)
	\arrow[swap, "\psi_X", from=1-2, to=3-1]
	\arrow["\psi_Y", from=1-2, to=3-3]
	\arrow["F(f)", from=3-1, to=3-3]
\end{tikzcd}
\end{document}
```