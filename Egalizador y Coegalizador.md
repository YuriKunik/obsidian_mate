#categorias #definiciones 
## Definiciones

### Egalizador
Dada una [[categoría]] $C$ decimos que el Egalizador de $f,g:X\rightarrow Y$ es una flecha $\lambda: E \rightarrow X$ tal que cumple la siguiente propiedad universal.
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	E & X & Y \\
	Z
	\arrow["\lambda", from=1-1, to=1-2]
	\arrow["f", shift left=1, from=1-2, to=1-3]
	\arrow["g"', shift right=1, from=1-2, to=1-3]
	\arrow["{\exists! h}", dashed, from=2-1, to=1-1]
	\arrow["{\tilde{h}}"', from=2-1, to=1-2]
\end{tikzcd}
\end{document}
```


### Coegalizador
Dada una categoría $C$ decimos que el Coegalizador de $f,g:X\rightarrow Y$ es una flecha $\lambda: E \rightarrow X$ tal que cumple la siguiente propiedad universal.
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	X & Y & E \\
	&& Z
	\arrow["\lambda", from=1-2, to=1-3]
	\arrow["f", shift left=1, from=1-1, to=1-2]
	\arrow["g"', shift right=1, from=1-1, to=1-2]
	\arrow["{\exists! h}", dashed, from=1-3, to=2-3]
	\arrow["{\tilde{h}}"', from=1-2, to=2-3]
\end{tikzcd}
\end{document}
```
## Observaciones
Estas definiciones son duales. 