# Forma de Newton

La forma de Newton para interpolar funciones tiene la ventaja de que es escalable al agregar datos, no requiere calcular todo de nuevo. El principio se basa en las diferencias divididas

## Diferencias divididas

### Primera diferencia dividida
$$
f[x_{0},x_{1}]= \frac{f(x_{1})-f(x_{0})}{x_{1}-x_{0}}
$$
### Segunda diferencia dividida

$$
f[x_{0},x_{1},x_{2}]= \frac{f[x_{1},x_{2}]-f[x_{0},x_{1}]}{x_{2}-x_{0}}
$$
### Formula general

$$
f[x_{0},x_{1}, \dots, x_{n}]= \frac{f[x_{1},\dots, x_{n}]-f[x_{0},\dots, x_{n-1}]}{x_{n}-x_{0}}
$$

## Construcción del polinomio

La forma de Newton para el polinomio interpolador es:

$$
p_{n}(x) = f(x_{0}) + f[x_{0},x_{1}](x-x_{0})+ \dots + f[x_{0},\dots,x_{n}]\prod_{i=0}^{n-1}(x-x_{i})
$$

Esta formula se puede derivar pero no tiene mucho sentido. Lo único destacable es que es bastante análoga a la forma de un polinomio de Taylor.

## Formula del error para Newton

Siendo $p_{n}$ el polinomio interpolador de $f$ en $x_{j}$, entonces el error cumple que
$$
E_{n}(x)=f[x_{0},\dots x_{n},x]W_{n+1}(x))
$$
### Demostración

Agregamos $x_{n+1}$ a la sucesión ${x_{0},\dots, x_{n}}$ y usamos que
$$
p_{n+1} = p_{n} + f[x_{0},\dots,x_{n+1}]W_{n+1}(x)
$$
Con lo que el error satisface
$$
E_{n}(x_{n+1})=f(x_{n+1})-p_{n}(x_{n+1})=f[x_{0},\dots,x_{n+1}]W_{n+1}(x)
$$
tomando $x_{n+1}=x$ estamos.

### Resultado extra (ya lo habíamos probado antes)

$$
f[x_{0},\dots x_{n}]=\frac{f^{n}(\xi)}{(n)!}
$$

Esto se obtiene fácil de la formula previa que teníamos para el error de interpolación.
