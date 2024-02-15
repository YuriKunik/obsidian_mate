## Teorema de convergencia

Si $f:[a,b]\to \mathbb{R}$ es continua y $f(a)f(b)>0$ entonces el método de bisección genera una sucesión $x_{n}$ tal que

1. $x_{n} \to r$ con $f(r)=0$
2. $\lvert r - x_{n} \rvert \leq \frac{b-a}{2^n}$

### Demostración

En cada paso conseguimos nuevos intervalos $[a_{n}, b_{n}]$ con $a \leq a_{1} \leq a_{2} \dots \leq b$ y $b \geq b_{1} \geq b_{}{2} \dots \geq a$. Como ambas sucesiones son monotonas y acotadas tienen límite. Además,
$$
\lvert b_{n} - a_{n} \rvert \leq \frac{b-a}{2^n} \to 0
$$
Entonces
$$
\lim_{ n \to \infty } a_{n} = \lim_{ n \to \infty } b_{n} = r
$$
Como $f$ es continua y $f(a_{n})f(b_{n})\leq 0$ para todo $n$
$$
f(r)^2 \leq 0
$$
por lo que $f(r) = 0$. Finalmente $a_{n} \leq x_{n} \leq b_{n}$ para todo $n$ por lo que $x_{n} \to r$ y
$$
\lvert r-x_{n} \rvert \leq \lvert b_{n} -a_{n} \rvert \leq \frac{b-a}{2^n}.
$$
