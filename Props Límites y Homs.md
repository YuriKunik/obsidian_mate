## Enunciado
El [[Límite]] de una colección de objetos $\{ A_{i} \}$ sale del Hom de la siguiente forma:
$$
[X, \lim_{  \leftarrow_{i\in I} } A_{i}] \equiv \lim_{  \leftarrow_{i\in I}} [X,A_{i}]
$$
## Demostración

Primero observemos que un [[Funtor]] $F: X \to Y$ manda [[cono|conos]] en conos. Dado un cono de $X$ a $A$,
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	X \\
	A_i
	\arrow["\pi_i", from=1-1, to=2-1]
\end{tikzcd}
\end{document}
```
Aplicar el funtor nos da la siguiente colección de flechas:
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	FX \\
	FA_i
	\arrow["F\pi_i", from=1-1, to=2-1]
\end{tikzcd}
\end{document}
```
que es un cono de $FX$ a $FA: I \to FX$ ya que el siguiente diagrama conmuta:
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
FX \\
FA_i & FA_j
\arrow["f", from=1-1, to=2-1]
\arrow["F", from=1-1, to=2-2]
\arrow["f", from=2-1, to=2-2]
\end{tikzcd}
\end{document}
```

Terminar.
