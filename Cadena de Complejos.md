#definiciones #topoalg #matemática #álgebra
## Definición

Una cadena de complejos es una colección de morfismos $\{\varphi_n\}_{n_\in\mathbb{N}}$  tal que $im(\varphi_{n}) \subset ker(\varphi_{n+1})$. Diagramáticamente escribimos:
```tikz
\usepackage{amsfonts}
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	 \dots & C_{n+1}(X) & C_n(X) \dots & \dots C_1(X) & C_0(X) & 0
	\arrow["\partial_{n+1}", from=1-1, to=1-2]
	\arrow["\partial_{n}", from=1-2, to=1-3]
	\arrow["\partial_{0}", from=1-4, to=1-5]
	\arrow["", from=1-5, to=1-6]
\end{tikzcd}
\end{document}
```