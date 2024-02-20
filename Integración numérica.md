
## Objetivo

Dada una función continua $f$ en un intervalo $[a,b]$ tomamos nodos $\{ x_{0},\dots, x_{n} \}$ en el intervalo, aproximamos a $f$ por un polinomio $p_{n}$ y lo integramos obteniendo
$$
\begin{align}
Q(f)&=\int _{a}^b p_{n} (x) \, dx \\
& = \int _{a}^b \sum_{j=0}^n f(x_{j} )l_{j} (x)\, dx \\
& = \sum_{j=0}^n A_{j} f(x_{j} )
\end{align}
$$
## Fórmulas de Newton-Côtes

Utilizamos nodos equiespaciados en el intervalo $[a,b]$. Consideramos $h=\frac{b-a}{n}$ y $x_{j}=a+jh$. Si $j = 0,\dots n$ es una **formula de Newton Côtes cerrada** y si excluimos los bordes es **abierta**.

### Regla de trapecios cerrada:

Se remplaza la función $f$ por la recta que une $(a,f(a))$ con $(b,f(b))$. la recta está dada por $p(x)=f(a)+ \frac{f(b)-f(a)}{b-a}(x-a)$, integrando obtenemos:
$$
\begin{align}
\int _{a}^bp(x) \, d &= f(a)+ \left. \frac{f(b)-f(a)}{b-a} \frac{(x-a)^{2}}{2} \right|_{a}^b \\
     & =f(a)(b-a)+ \frac{f(b)-f(a)}{2} (b-a)

\end{align}
$$
es decir:
$$
\int _{a}^bf(x)\, dx \sim T(f)= \frac{b-a}{2}(f(a)+f(b))
$$

### Regla de trapecios abierta:

Similar a la anterior pero tomamos como nodos los tercios medios del intervalo para construir la recta. Con esto
$$
\int _{a}^b f(x) \, dx \sim \frac{3h}{2}(f(x_{1} + f(x_{2}))) 
$$