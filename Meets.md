
## Definición

Sea $(P, \leq)$ un [[Preorden|preorden]] y $A \subseteq P$ un subconjunto. Decimos que un elemento $p \in P$ es un meet de $A$ si
1. $\forall a \in A$ tenemos $p\leq a$ y
2. $\forall q$ tal que $q\leq a$, $\forall a \in A$, tenemos $q\leq p$ .
Lo notamos $p=\wedge A$

## Observación

### Un meet es un límite

#### Cono con base la inclusión

Dado un subconjunto $A \subseteq P$,  tomamos el funtor inclusión $i: A\to P$ como base de la [[Categoría|categoría]] de [[Cono|conos]]. Con esto, un cono es un elemento $p \in P$ , tal que $\forall a,b \in A$

```tikz
\usepackage{amsfonts}
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	 & p & \\
			\\
	 a & & b
	\arrow[swap, "", from=1-2, to=3-1]
	\arrow["", from=1-2, to=3-3]
	\arrow["", from=3-1, to=3-3]
\end{tikzcd}
\end{document}
```
Esto nos viene a decir que, dado un par comparable, p es menor a ambos. Tomando $a \rightarrow a$ tenemos que p es menor igual a todos los elementos de $A$. 

#### Cono terminal

Un [[límite]] en esta [[categoría]] va a ser un [[cono]] terminal. Es decir que, para todo vértice $q$ de un cono, el cono terminal con vértice $p$ es más chico que $q$. Esto más lo anterior juntan claramente la noción de meet. i.e
$$
\lim_{\leftarrow} i = \wedge A
$$