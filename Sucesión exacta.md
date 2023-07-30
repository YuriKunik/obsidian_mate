
## Definición

Una sucesión exacta es una cadena de morfismos

```tikz
\usepackage{amsfonts}
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	 \dots & M_{n+1} & M_n \dots & \dots M_1 & M_0
	\arrow["f_{n+1}", from=1-1, to=1-2]
	\arrow["f_{n}", from=1-2, to=1-3]
	\arrow["f_{0}", from=1-4, to=1-5]
\end{tikzcd}
\end{document}
```

tales que $\text{ker}(f_{i-1}) = \text{im}(f_{i})$
