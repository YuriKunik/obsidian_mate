## Formula
$x_{n+1} = x_{n} - \frac{f(x_{n})}{f^\prime(x_{n})}$
## Teorema de existencia

Si existe el límite de la sucesión $(x_{n})$ entonces converge a una raíz.

### Demostración

Sea $\lim_{ n \to \infty }x_{n} = r$ entonces 
$$
f^\prime(x_{n})(x_{n+1}-x_{n}) = f(x_{n}).
$$
Como ambas funciones son continuas, podemos tomar límite de ambos lados y nos queda que $0 = f(r)$.

## Fórmula del error

La sucesión del error está dada por
$$
\begin{align}
e_{n+1} & =x_{n+1}-r \\
     & = x_{n}-\frac{f(x_{n})}{f^\prime(x_{n})} - r  \\
      & =e_{n}-\frac{f(x_{n})}{f^\prime(x_{n})} \\
     & = \frac{e_{n}f^\prime(x_{n})- f(x_{n})}{f^\prime(x_{n})}
 
\end{align}
$$
Usando el polinomio de taylor de orden 2, centrado en $r$, evaluado en $x_{n}$, se puede simplificar un poco más la expresión:
$$
0 = f(r) = f(x_{n})-(x_{n}-r)f^\prime(x_{n}) + \frac{1}{2}(x_{n}-r)^2f^{\prime\prime}(\xi)
$$
con $\xi$ entre $r$ y $x_{n}$. Reemplazando en la formula de $e_{n+1}$ nos da
$$
e_{n+1} = \frac{1}{2} \frac{f^{\prime\prime}(\xi)}{f^\prime(x_{n})}e_{n}
$$
## Teorema de convergencia

Si $r$ es un cero simple de $f$ y sea $I=[r-\alpha, r+ \alpha]$ un intervalo taal que $\lvert f^\prime(x) \rvert \geq \delta > 0$ y $f^{\prime\prime}$ está acotada. Entonces existe $\varepsilon > 0$ tal que $I_{\varepsilon} = [r-\varepsilon, r+\varepsilon] \subset I$ y se tiene que $\lvert e_{n} \rvert \to 0$ y 
$$
\lvert e_{n+1}  \rvert \leq \frac{1}{2} \frac{M}{\delta} \lvert e_{n} \rvert ^2 \quad \text{para }x_{0} \in I_{\varepsilon}
$$
### Demostración

Tomemos $\varepsilon > 0$ tal que 
$$
\frac{1}{2} \frac{M}{\delta}\varepsilon = \lambda < 1.
$$
Entonces, si $x_{0} \in I_{\varepsilon}$ tenemos que $\lvert e_{0} \rvert= \lvert x_{0}-r \rvert < \varepsilon$. Usando la formula del error que conseguimos antes y las cotas de las funciones,
$$
\lvert e_{1} \rvert = \lvert x_{1} -r \rvert \leq \lambda \lvert e_{0} \rvert 
$$
siguiendo esto
$$
\lvert e_{n} \rvert \leq \lambda^n \lvert e_{0} \rvert 
$$
que como $0 <\lambda < 1$ $e_{n} \to 0$. La desigualdad la obtenemos directamente de la formula del error.

## Teorema de convergencia global.

Sea $f$ dos veces derivable tal que $f^{\prime\prime} > 0$ y f cambie de signo. Dado cualquier valor inicial $x_{0}$, si f no alcanza su mínimo en $x_{0}$ entonces el método converge.

### Demostración

Supongamos que $f$ es monótona creciente. En este caso, $f$ tiene una ñ
única raíz, r. 

Si $x_{0} > r$ entonces $x_{1} < x_{0}$ pues $x_{1}=x_{0}-\frac{f(x_{0})}{f^\prime(x_{0})}$ pues el termino que resta es positivo (pensar un poquito). Veamos que $x_{1} > r$. Por taylor
$$
0 = f(r) \geq f(x_{0}) + f^\prime(x_{0})(r-x_{0})
$$
y por la definición de $x_{1}$

$$
0 = f(x_{0}) + f^\prime(x_{0})(x_{1}-x_{0})
$$

así, despejando, obtenemos que $x_{1} \geq r$. 

Siguiendo estos pasos nos armamos una sucesión monótona acotada que, por lo tanto es convergente a una raíz de $f$. Como en este caso es única, $x_{n} \to r$.

En el caso de $f$ monótona decreciente, la prueba es análoga. Y si $f$ no es ninguna de las dos, entonces alcanza un mínimo en un punto $c$. Si $x_{0} > c$, (el otro caso es análogo) tenemos dos opciones, o $x_{0} > r$ y podemos asumir que $f$ es monótona creciente, o $x_{0} < r$ y entonces con $x_{1}$ estaríamos en $x_{1} > r$ (por la desigualdad que obtuvimos en el primer caso) y podríamos proseguir de igual manera
