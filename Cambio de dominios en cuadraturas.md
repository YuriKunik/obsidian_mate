
# Lema
Si $Q_{0}(f)=\sum_{j=0}^n A_{j}f(t_{j})$ es una formula de cuadratura para $\int _{-1}^1 f(x) \, dx$. Entonces, para
$$
x_{j}=\frac{b-a}{2}t_{j}+\frac{a+b}{2}, \quad \forall j = 0,\dots n
$$
se tiene una formula de cuadratura para el intervalo $[a,b]$
$$
\int ^b_{a}f(x) \, dx \sim Q(f)=\sum_{j=0}^n \frac{b-a}{2}A_{j}f(x_{j}).
$$
## Demostración

Hacemos el cambio de variables $x = \alpha t + \beta$ con $\alpha = \frac{b-a}{2}$ y $\beta = \frac{a+b}{2}$. Con esto
$$
\int _{a}^bf(x) \, dx = \int _{-1}^1f(\alpha t+b)\alpha \, dx 
$$
Aplicando la cuadratura a $g(t)=\alpha f(\alpha t+b)$ tenemos
$$
\int _{a}^bf(x) \, dx \sim Q_{0}(g)
$$

Con 
$$
Q_{0}(g)=\sum_{j=0}^n A_{j}g(t)=\sum \alpha A_{j}f(\alpha t_{j}+\beta)
$$

Con esto estamos.