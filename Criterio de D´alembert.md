#complejo #series #seriespotencias 
## Enunciado

Supongamos que existe el límite 
$$
L:=\lim_{ n \to \infty } \left \lvert \frac{a_{n} }{a_{n+1}} \right\rvert 
$$
entonces $L$ es el [[Radio de convergencia]].

## Demostración

La demostración vuelve a utilizar la equivalencia entre el [[Lema de Abel]] y la definición de [[Radio de convergencia]]. 

### Supongamos que $r>L$
Entonces existe $n_{0}\in \mathbb{N}$ tal que, para todo $n \geq n_{0}$

$$
r>\left\lvert  \frac{a_{n}}{a_{n+1}}  \right\rvert \geq 0
$$
Con esto 

$$
\lvert a_{n_{0}} \rvert  < r\lvert a_{n_{0}+1}  \rvert < \dots < r^k \lvert a_{n_{0}+k}  \rvert .
$$
Es decir $\lvert  a_{n}\rvert r^n > \lvert a_{n_{0}}r^{n_{0}} \rvert$ por lo que no converge a $0$, que además implica que no converge la sumatoria para $\lvert z \rvert=r$, es decir $L\geq\rho$.

## $r< L$
Podemos fijar $n_{0}$ tal que 
$$
r< \left \lvert  \frac{a_{n}}{a_{n+1}}   \right \rvert 
$$
para todo $n \geq n_{0}$. Usando esta desigualdad, tenemos
$$
\lvert a_{n}  \rvert r^n < \lvert a_{n_{0}}  \rvert r^{n_{0}} \quad n\geq n_{0}
$$
por lo que la sucesión está acotada.

