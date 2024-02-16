#calculonumerico #integracion
## Construcción

Es el método de integración más simple. Para integrar usa los puntos de los extremos de los intervalos y reemplaza la función por la recta que los une.
### Puntos
$\{a, b\}$
### Polinomio
$$
p(x)=f(a)- \frac{f(b)-f(a)}{b-a}(x-a)
$$
### Expresión
$$
T(f)=\frac{b-a}{2}(f(a)+f(b))
$$
## Error

Si $f \in C^2[a,b]$, el error que se produce al aproximar $\int _{a}^b f(x) \, dx$ esta dado por
$$
R(f)=-\frac{(b-a)^{3}}{12}f^{\prime \prime}(\eta), \quad \text{con } \eta \in (a,b) 
$$
### Demostración.
El error en un principio está dado por
$$
R(f)=I(f)-T(f)=\int _{a}^b \frac{f^{\prime \prime }(\xi(x))}{2}W_{2}(x) \, dx.
$$
La segunda igualdad vale al ser lineal la integral y la cuadratura $T$ una integral de un polinomio interpolador de grado 1 de $f$ en $\{a,b\}$. Por esto último aparece $W_{2}(x)=(x-a)(x-b)$ y la fórmula del error de un polinomio interpolador. Ahora, $W_{2}$ no cambia de signo en $(a,b)$ y $f^{\prime\prime}$ es continua, por lo que podemos aplicar el [[Valor medio integral generalizado]] y obtener
$$
\begin{align}
R(f)&=f^{\prime \prime }(\eta)\int _{a}^b (x-a)(x-b) \, dx \\
     & =-\frac{f^{\prime \prime }(\eta)}{12}(b-a)^{3}
\end{align}
$$

## Trapecios compuesta

Tomando $x_{j}=a+jh$ con $h=\frac{b-a}{n}$ y $j=0,\dots n-1$,
$$
T_{j}(f)=\frac{h}{2}(f(x_{j}+x_{j+1}))
$$

entonces, sumando todo
$$
T(f)=\frac{h}{2}\left[ f(x_{0})+\sum_{j=1}^{n-1}2f(x_{j}) + f(x_{n}) \right]
$$
### Error

Para cada subintervalo cometemos un error $R_{j}(f)=-\frac{f^{\prime \prime }(\eta_{j})}{12}h^{3}$. Entonces
$$
R(f)=-\frac{h^{3}}{12}\sum f^{\prime \prime }(\eta_{j})
$$
usando el [[lema para error de cuadraturas compuestas]] con $a_{i}=1$ tenemos

$$
R(f)=-\frac{h^{2}}{12}(b-a)f^{\prime  \prime }(\eta)
$$