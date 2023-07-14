## Definición
Dadas dos transformaciones naturales entre [[Funtor|funtores]] $\nu: F\Rightarrow G$ y $\mu:F^{'} \Rightarrow G^{'}$ 

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}[]
C & \nu \Downarrow & D & \mu \Downarrow & E\\
\arrow[bend right,"G", from=1-1, to=1-3]
\arrow[bend left,"F", from=1-1, to=1-3]
\arrow[bend right,"G^{'}", from=1-3, to=1-5]
\arrow[bend left,"F^{'}", from=1-3, to=1-5]
\end{tikzcd}
\end{document}
```
tenemos la composición horizontal


```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}[]
C & \nu \Downarrow & E \\
\arrow[bend right,"G^{'}G", from=1-1, to=1-3]
\arrow[bend left,"F^{'}F", from=1-1, to=1-3]
\end{tikzcd}
\end{document}
```
que vienen de los cuadrados

```tikz
\usepackage{tikz-cd}
\usepackage{amsfonts}
\begin{document}
\begin{tikzcd}
	F(X) & G(X) \\ 
	F^{'}F(Y) & G^{'}G(Y)
	\arrow["\nu_X", from=1-1, to=1-2]
	\arrow["F^{'}F(f)", from=1-1, to=2-1]
	\arrow["G^{'}G(f)", from=1-2, to=2-2]
	\arrow["\nu_Y", from=2-1, to=2-2]
\end{tikzcd}
\end{document}
```
