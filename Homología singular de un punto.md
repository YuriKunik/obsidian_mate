## Proposición
Si $X$ es un punto, entonces su [[Homología Singular]] $H_n(X) = 0$ para $n>0$ y $H_0(X)\approx \mathbb{Z}$ 

## Demostración 
Cada $C_n(X)$ es $\mathbb{Z}$ ya que tenemos un único [[n simplex singular]] para cada n. Los morfismos de borde van a mandar $\sigma_n \mapsto \sum_i (-1)^i \sigma_{n-1}$ lo cual vale 0 si n es par y $\sigma_{n-1}$ si n es impar. Con esto nos queda la [[Cadena de Complejos]] 

```tikz
\usepackage{tikz-cd}
\usepackage{amsfonts}
\begin{document}
\begin{tikzcd}
	\dots & \mathbb{Z} & \mathbb{Z} & \mathbb{Z} & 0
	\arrow["0", from=1-1, to=1-2]
	\arrow["\approx", from=1-2, to=1-3]
	\arrow["0", from=1-3, to=1-4]
	\arrow["", from=1-4, to=1-5]
\end{tikzcd}
\end{document}
```

que, al pasar a la homología, nos da lo que queriamos.