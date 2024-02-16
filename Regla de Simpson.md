#calculonumerico #integracion
## Construcción

La idea es cambiar a $f$ por un polinomio de grado $2$. Como necesitamos 3 puntos elegimos $\{a, \frac{a+b}{2}, b\}$

Por el [[Cambio de dominios en cuadraturas]] podemos ver la formula de Simpson en el $[-1,1]$
$$
\int _{-1}^{1} p(x) \, dx = 2\left[ a_{0}+\frac{a_{2}}{3} \right]=\frac{2}{6} [6a_{0}+2a_{2}]
$$
Por otro lado $p(x)$ verifica
$$
\begin{pmatrix}
1 & -1 & 1 \\
1 & 0 & 0 \\
1 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
a_{0} \\
a_{1} \\
a_{2}
\end{pmatrix}
=\begin{pmatrix}
f(-1) \\
f(0) \\
f(1) 
\end{pmatrix}
$$
De donde, $a_{0}=f(0)$, $a_{1}=\frac{f(1)-f(-1)}{2}$ y $a_{2}=\frac{f(-1)-2f(0)+f(1)}{2}$
Luego 
$$
\int _{-1}^1 f(x) \, dx \sim \frac{2}{6}[f(-1)+4f(0)+f(1)]
$$

### Puntos
$\{a, \frac{a+b}{2}, b\}$
### Expresión
$$
S(f)=\frac{h}{3}[f(a)+4f(a+h)+f(b)]
$$

### Versión abierta
Igual que antes pero interpolamos en ${-\frac{1}{2},0, \frac{1}{2}}$.

## Error

Si $f \in C^4[a,b]$, el error que se produce al aproximar $\int f \, dx$ está dado por
$$
R(f)=-\frac{1}{90}\left( \frac{b-a}{2}\right)^5 f^{(4)}(\eta) \quad \text{ para } \eta \in (a,b)
$$

### Demostración

TODO

## Simpson compuesto
Tenemos que
$$
S_{j}(f)=\frac{h_{3}}f\left( x_{j}+4f\left(\frac{(x_{j}+x_{j+1})}{2}\right) +  f(x_{j+1})\right)
$$

Sumamos y tenemos la fórmula general
TODO
### Error: 
$$
R(f)=-\frac{h^4}{180}(b-a)f^{(4)}(\eta)
$$






