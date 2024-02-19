#calculonumerico 

## Enunciado

Sea $g:[a,b]\to \mathbb{R}$ continua y que no cambie de signo, $\xi:[a,b]\to [c,d]$ y $h:[c,d]\to \mathbb{R}$ continua, tales que $h(\xi(x))g(x))$ sea integrable. Entonces existe $\eta \in [c,d]$ tal que
$$
\int _{a}^b g(x)h(\xi(x))\, dx = h(\eta)\int _{a}^b g(x)\, dx 
$$
## Demostración

Supongamos $g(x)\geq 0$, y el caso contrario es análogo. Sean $m$ y $M$ el mínimo y el máximo de $h$ respectivamente. Entonces 
$$
mg(x)\leq h(\xi(x))g(x) \leq Mg(x),
$$

que integrando en todos lados obtenemos
$$
m\int g(x) \, dx \leq \int h(\xi(x))g(x) \, dx  \leq M\int g(x) \, dx ,
$$
De donde
$$
m \leq
\frac{\int h(\xi(x))g(x)  \, dx }{\int g(x) \, dx } \leq M
$$
Por lo tanto, usando Bolzano estamos.