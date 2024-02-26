#complejo #series 
## Enunciado

Para cada $m \in \mathbb{N}$, sea $\{ z_{nm} \}_{n\geq 0}$ una sucesión. Supongamos cumplen las siguientes propiedades:
    1. Existe $A_{n}$ tal que $\sum_{n=0}^\infty A_{n} < \infty$ y $\lvert z_{nm} \rvert \leq A_{n}$ para todo $m$ y todo $n$.
    2. Para todo $n$ existe $z_{n}$ tal que $\lim_{ m \to \infty }z_{mn}=z_{n}$.

Entonces la serie $\sum_{n=0}^\infty z_{n}$ converge y vale
$$
\lim_{ m \to \infty } \sum_{n=0}^\infty z_{mn}=\sum_{n=0}^\infty z_{n}. 
$$

## En criollo

Tenemos una sucesión en dos variables ${z_{nm}}$ tal que  converge tendiendo $m$ a infinito para todo valor de ${n}$ y además cada $z_{mn}$ está acotado para cada $n$ por $A_{n}$ y esa cota sirve para todo $m$.

## Demostración

Tomando límite tenemos que $z_{n} \leq A_{n}$, de modo que esta última serie converge. Dado $\varepsilon >0$ podemos tomar $N_{0}$ de manera tal que $\sum_{n=N_{0}+1}^\infty A_{n} < \frac{\varepsilon}{3}$. Entonces

$$
\left \lvert\sum_{n=N_{0}+1}^\infty (z_{mn}-z_{n} )  \right\rvert 
< \frac{2\varepsilon}{3}
$$
(Desigualdad triangular).  Por otra parte, empleando la primera hipótesis podemos tomar $M_{0}$ tal que para $m\geq M_{0}$ resulte
$$
\left\lvert  \sum_{n=0}^{N_{0}} (z_{mn} -z_{n}  ) \right\rvert < \frac{\varepsilon}{3}.
$$
Juntando todo

$$
\left \lvert  \sum_{n=0}^\infty z_{mn}-\sum_{n=0} ^\infty z_{n}  \right\rvert \leq \left\lvert  \sum_{n=0}^{N_{0}}(z_{nm} -z_{n}  )  \right\rvert +\left\lvert  \sum_{n=N_{0}+1}^\infty(z_{nm} -z_{n}  )  \right\rvert < \varepsilon.
$$

## Corolario

Se puede cambiar el orden de dos sumatorias consecutivas siempre que
$$
\sum_{n=0}^N \sum_{m=0}^M \lvert a_{nm}  \rvert \leq C
$$









