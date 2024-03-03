
## Enunciado

Sea $\gamma$ una curva [[continua]] y cerrada,  Para todo $w \notin \text{im}(\gamma)$, entonces el [[Indice de una curva]] verifica $I(\gamma,w)\in \mathbb{Z}$

## Demostración

Siguiendo la definición, $I(\gamma, w)= \frac{1}{2\pi i}[F(b)-F(a)]$, donde $F$ es una primitiva de la función $\frac{1}{z-w}$ a lo largo de $\gamma$. Podemos elegir $F$ de manera que $e^{F(t)}=\gamma(t)-w$; de esta forma,
$$
e^{F(b)-F(a)}= \frac{\gamma(b)-w}{\gamma(a)-w}=1
$$
de modo que $F(b)-F(a)=2k\pi i$, es decir, $I(\gamma, w)= k$.