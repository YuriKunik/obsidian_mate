
## Enunciado

### Constructivo

Sea $A$ un conjunto con una relación de equivalencia $\sim$, una función $f:A\to Z$ compatible con la relación $\sim$, entonces el siguiente triangulo conmuta:

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A & Z\\
A/\sim
\arrow["f", from=1-1, to=1-2]
\arrow["\pi", swap,from=1-1, to=2-1]
\arrow["\bar{f}", swap, from=2-1, to=1-2]
\end{tikzcd}
\end{document}
```

con $\bar{f}([a])=f(a)$. Además $\bar{f}$ es la única función con esa propiedad.

### Categórico

Sea $A$ un conjunto con una relación de equivalencia $\sim$, una función $f:A\to Z$ compatible con la relación $\sim$, entonces 
tomemos la [[categoría de conos]] bajo $C_{A}^{\sim}$, siendo este el [[funtor]] constantemente $A$, con imagen en la [[categoría]] $C$, pero restringida para que solo contenga las flechas que salen de $A$ compatibles con la relación $\sim$. Los objetos de esta categoría son flechas:
$$
\begin{align}
&A\\
g&\downarrow\\
&B
\end{align}
$$

con $g$ compatible con $\sim$. Dado esto, los morfismos van a ser funciones $\sigma:B\to C$ tales que conmuta

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A & B\\
C
\arrow["f", from=1-1, to=1-2]
\arrow["g", swap,from=1-1, to=2-1]
\arrow["\sigma", swap, from=2-1, to=1-2]
\end{tikzcd}
\end{document}
```
Dicho todo esto el resultado de la prop universal para cocientes nos dice que el cono:
$$
\begin{align}
&A\\
\pi&\downarrow\\
A& /\sim
\end{align}
$$

es inicial. Lo que es equivalente a decir que 
$$
\text{colim}{C_{A}^{\sim}}.
$$


## Observaciones

Demostrado esto, en el resto de propiedades universales del cociente, lo único que hay que chequear es que cada lugar admite una estructura acorde, una vez que tenemos todo en la misma categoría, solo es necesario ver que $\bar{f}$ también se encuentra ahí.


