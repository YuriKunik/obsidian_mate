## Proposición
Si X es no vacío y arco conexo, entonces $H_0(X) \approx \mathbb{Z}$. De esto se sigue, por [[Descomposición de homología singular]], que para un espacio arbitrario $H_0(X)$ es la suma directa de un $\mathbb{Z}$ por cada componente arco conexa de X.

## Demostración
Como tenemos por definición que $H_0(X) = C_0(X)/Im(\partial_1)$, podemos encontrar un iso con $\mathbb{Z}$, mediante un morfismo epi  $\varepsilon:  C_0(X)\rightarrow \mathbb{Z}$ que tenga como $ker(\varepsilon)$  a $Im(\partial_1)$. Nos va a servir $\varepsilon(\sum_i n_i \sigma_i)= \sum_i n_i$. Con esto, nos queda claro que es epi, nos falta ver que su núcleo coincide con la imagen de $\partial_1$.

#### $Im(\partial_1)\subset ker(\varepsilon)$:
Si tomamos un elemento $\zeta \in Im(\partial_1)$, entonces existe un $\sigma: \Delta^1 \rightarrow X$, por lo tanto $\varepsilon(\partial_1)(\sigma) = \varepsilon(\sigma|[v_1]) - \varepsilon(\sigma|[v_0]) = 1-1 =0$.

#### $\ker(\varepsilon) \subset Im(\partial_1)$

Si $\varepsilon \sum_i n_i \sigma_i = 0$, entonces $\sum_i n_i = 0$. Agarremos $\tau_i: I \rightarrow X$ desde un punto $x_0$ a otro $\sigma_i(v_0)$. Cada $\tau_i$ lo podemos ver como un $1$-simplex con $\partial \tau_i = \sigma_i - \sigma_0$. Con esto, tenemos que $\partial(\sum n_i\tau_i ) = \sum n_i \sigma_i  - \sum n_i \sigma_0 = \sum n_i \sigma_i$.

Con esto terminamos.