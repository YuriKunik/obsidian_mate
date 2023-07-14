#ejemplos #categorias #matemática #topo 

## Funtor olvido (topo)

Sea el espacio topológico $1$, tenemos funciones continuas que agarran un punto de $X$. Nos dice que tenemos una biyección 
$$
U(X) \cong [1,X]
$$
y  es [[Transformación natural|natural]] en X. Para ver que es natural, analizamos el siguiente diagrama:

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
U(X) & 1 X\\
U(X^\prime) & 1 X \\
\arrow["u", from=1-1, to=1-2]
\arrow["Uf", from=1-1, to=2-1]
\arrow["f", from=2-1, to=2-2]
\arrow["f", from=1-2, to=2-2]
\end{tikzcd}
\end{document}
```

