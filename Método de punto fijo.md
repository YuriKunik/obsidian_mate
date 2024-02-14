
# Existencia de punto fijo

Sea $I = [a,b]$, $g:[a,b]\to \mathbb{R}$ continua, si $g(I)\subset I$ entonces $g$ tiene al menos un punto fijo en $I$.

## Demostración

Como $g(I)\subset I$ se tiene que $a\leq g(a)\leq b$ y $a\leq g(b)\leq b$. Si $a = g(a)$ o $b = g(b)$ ya estamos, caso contrario $g(a)-a \geq 0$ y $g(b)-b \leq 0$ por lo que la función $f(x)=g(x)-x$ tiene al menos una raíz en el intervalo $I$. O, lo que es lo mismo $g$ tiene un punto fijo en $I$.

# Unicidad del punto fijo

Si $g$ es derivable y $\lvert g^\prime \rvert \leq \lambda<1$ para todo $x$ en $I$ y $g(I)\subset I$ entonces $g$ tiene un único punto fijo.

## Demostración

De tener dos puntos fijos, $r_{1}, r_{2}$ con $r_{1} \neq r_{2}$, tenemos
$$
\lvert r_{1}-r_{2} \rvert =\lvert g(r_{1})-g(r_{2}) \rvert = \lvert g^\prime(\xi)(r_{1}-r_{2}) \rvert \leq \lambda \lvert r_{1}-r_{2} \rvert < \lvert r_{1}-r_{2} \rvert
$$
Lo cual es absurdo.

# Teorema de Convergencia

Sea $g:I\to \mathbb{R}$ tal que $\lvert g^\prime (x)\rvert \leq \lambda < 1$ para todo $x$ en $I$ y $g(I)\subset I$ entonces la sucesión $x_{n}$ definida por
$$
x_{n+1} = g(x_{n})
$$
converge al único punto fijo de $g$ y además,
1. $\lvert x_{n} - r \rvert\leq\lambda^n \lvert x_{0}-r \rvert$
2. $\lvert  e_{n} \rvert \leq \frac{\lambda^n}{1-\lambda}\lvert x_{1}-x_{0} \rvert$

## Demostración

Sabemos que en $I$ existe un único punto fijo de $g$, llamado $r$. Ahora, la hipótesis implica que $g$ es Lipschitz de constante $\lambda$. Esto nos da que
$$
\lvert x_{n+1}-r \rvert =\lvert g(x_{n})-g(r) \rvert \leq \lambda \lvert x_{n} -r \rvert \leq \lambda^{n+1} \lvert x_{0}-r \rvert 
$$
De donde vemos que $x_{n}$ converge a r. Además

$$
\lvert x_{0}-r \rvert \leq \lvert x_{0}-x_{1} \rvert + \lvert x_{1}-r \rvert \leq \lvert x_{0}-x_{1} \rvert + \lambda \lvert x_{0}-r \rvert 
$$
que, despejando nos da

$$
(1-\lambda)\lvert x_{0}-r \rvert \leq \lvert x_{1}-x_{0} \rvert .
$$

Finalmente sumando esto a la desigualdad obtenida en el primer paso tenemos $2$.

# Existencia de un intervalo de convergencia

Sea $g:(a,b)\to \mathbb{R}$ una función derivable con derivada continua y $r \in(a,b)$ un punto fijo de $g$ tal que $g^\prime(r)<1$, entonces existe un $\varepsilon>0$ tal que la iteración es convergente siempre que $x_{0} \in I = (r-\varepsilon, r+\varepsilon)$

## Demostración

Como $\lvert g^\prime(r) \rvert < 1$, existe unaa constante $K<1$ y un $0<\varepsilon$ tales que $\lvert g^\prime(x) \rvert<K$ dentro de este intervalo. Entonces $\forall x \in I_{\varepsilon}$,
$$
\lvert g(x)-r \rvert \leq \lvert g^\prime(\xi) \rvert \lvert x-r \rvert \leq K\varepsilon < \varepsilon
$$

por lo que $g(I_{\varepsilon})\subset I_{\varepsilon}$. Con esto aplicamos el resultado de convergencia y estamos.