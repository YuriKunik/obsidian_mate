
## Enunciado

Sea $f:\mathbb{C}\to \mathbb{C}$ una [[Función holomorfa]] tal que $\lim_{ \lvert z \rvert \to \infty } \frac{f(z)}{z^{n}}=0$ para algún $n\geq 1$. Entonces $f$ es un polinomio de grado menor o igual que $n$.

## Demostración

Tenemos que, $\forall \varepsilon >0$ existe $R> 0$ tal que si $\lvert z \rvert>R$ entonces
$$
\left\lvert  \frac{f(z)}{z^{n}}  \right\rvert \leq \varepsilon
$$
Como esto también vale para $z \in \partial D_{R}(0)$, por la [[Desigualdad de Cauchy]]. Para todo $k \geq n$ vale
$$
\lvert a_{k}  \rvert \leq \frac{\lvert f(\tilde{z}) \rvert }{r^{k}} < \frac{\varepsilon \lvert \tilde{z} \rvert ^{k}}{r^{k}}=\varepsilon
$$
que como vale para todo $\varepsilon$, entonces $a_{k}=0$ para $k\geq n$.