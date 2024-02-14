# Formulas

## Formula del método

$$
x_{n+1} = x_{n}-f(x_{n}) \frac{x_{n}-x_{n-1}}{f(x_{n})-f(x_{n-1})}
$$

## Formula del error

Para expresar el error usamos la definición de diferencias

### Primera diferencia
$$
f[a,b] = \frac{f(b)-f(a)}{b-a} = f^\prime(\xi)
$$
### Segunda diferencia
$$
f[a,b,c] =\frac{\frac{f(c)-f(b)}{c-b}-\frac{f(b)-f(a)}{b-a}}{c-a} = \frac{f[a,c] - f[a,b]}{c-a} 
$$
#### Lema 
$$
f[a,b,c] = \frac{1}{2}f^{\prime\prime}(\xi)
$$
##### Demostración

Tomamos la función
$$
g(x) = f(x) - f(a) + f[a,b](x-a) + f[a,b,c](x-a)(x-b).
$$
Con esta definición, tenemos que $g(a)=0,g(b)=0,g(c)=0$ por lo que $g^\prime$ se anula en al menos dos puntos y esto nos da que exista $g^\prime\prime(\eta)=0$. Derivamos dos veces $g$, evaluamos en $\eta$ y estamos.

### Formula
Versión origina:
$$
e_{n+1}=-e_{n}e_{n-1} \frac{f[x_{n-1}, r, x_{n}]}{f[x_{n-1},x_{n}]}
$$
Versión usando el lema:

$$
e_{n+1}=-e_{n}e_{n-1} \frac{f^{\prime\prime}(\eta_{n})}{f^{\prime} (\xi_{n})}
$$


# Teorema de convergencia local

Si $f^{\prime}(r)\neq 0$, $\lvert f^{\prime\prime} \rvert \leq K$ en un entorno de $r$, si existe $\varepsilon$ tal que $x_{0}, x_{1} \in I_{\varepsilon} = (r-\varepsilon, r+\varepsilon)$ entonces
$$
e_{n} \to 0
$$

## Demostración

Existe $\varepsilon$ tal que $\lvert f^{\prime} \rvert >\delta$ en $I_{\varepsilon}$, entonces si $x_{0},x_{1} \in I_{\varepsilon}$ tenemos que 
$$
\lvert e_{2} \rvert \leq \frac{K}{2\delta}\lvert e_{1} \rvert \lvert e_{2} \rvert \leq \frac{K}{2\delta}\varepsilon^{2}
$$
Si pedimos que 
$$
\frac{K}{2\delta}=\lambda < 1
$$
nos queda que $\lvert e_{2} \rvert\leq\lambda\varepsilon<\varepsilon$. Lo que nos dice que $x_{2} \in I_{\varepsilon}$. Ahora repetimos estos pasos e inductivamente concluimos que

$$
\lvert e_{n} \rvert \leq \lambda^{n-1}\varepsilon\to_{0}.
$$

# Orden de convergencia

TODO.