#análisis #series #complejo 
## Enunciado

Dada una sucesión de funciones $f_{n}:U\to \mathbb{C}$ son equivalentes:
1. $f_{n}$ [[Convergencia Uniforme|converge uniformemente]] en $U$
2. Para todo $\varepsilon>0$ existe $N_{0}$ tal que, si $N,M$ cumplen que $N_{0}\leq N \leq M$ entonces $$
\lvert S_{M}(z)-S_{N}(z) \rvert =\left\lvert  \sum_{n=N+1}^M f_{n} (z) \right\rvert < \varepsilon \quad \forall z \in U.
$$
## Demostración

### $1 \implies 2$

Sea $S(z)=\sum f_{n}(z)$ la función dada por la [[Convergencia puntual]] de la sucesión. Tenemos que, dado $\varepsilon > 0$, existe $N_{0} \in \mathbb{N}$ tal que, para todo $N \geq N_{0}$, vale $\lvert S(z)-S_{N}(z) \rvert$ para todo $z \in U$.

Con esto,
$$
\lvert S_{M}(z) - S_{N}(z) \rvert \leq \lvert S_{M}(z)- S(z) \rvert + \lvert S_{N}(z)-S(z) \rvert < \varepsilon.
$$
lo que demuestra $2$

### $2 \implies 1$

Como, para cada $z \in U$, la sucesión $\{ S_{n}(z) \}$ es de [[Sucesión de Cauchy|Cauchy]], converge un $S(z)$. Ahora, podemos tomar $N_{0}$ tal que $\lvert S_{M}(z)-S_{N}(z) \rvert < \frac{\varepsilon}{2}$.  Usando que $S_{n}(z)$ converge a $S(z)$ tomamos un $N_{z}>N_{0}$ tal que  $\lvert S_{n}(z)-S(z) \rvert< \frac{\varepsilon}{2}$. Ahora tenemos
$$
\lvert S(z) - S_{N}(z) \rvert \leq \lvert S(z)-S_{N_{z}}(z) \rvert + \lvert S_{N_{z}}(z)- S_{N}(z) \rvert  < \frac{\varepsilon}{2} \quad \forall N \geq N_{0}
$$


