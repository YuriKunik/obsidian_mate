
## Objetivo

Dada $f\in C[a,b]$ y $a=x_{0}<x_{1}<\dots<x_{n}=b$ buscamos $S$ tal que $S, S^\prime, S^{\prime\prime}$ sean continuas y 
$$
S(x_{j})=f(x_{j})\quad  \text{y} \quad S|_{[x_{j}, x_{j+1}]} \in  \mathcal{P}_{3}
$$
## Teorema

Dada $f \in C[a,b]$ y $a=x_{0},x_{1},\dots,x_{n}=b$ existe una única $S\in C^{2}[a,b]$ tal que
$$
\begin{cases}
S(x_{j})=f(x_{j}) \quad \quad 0\leq j\leq n\\
S|_{[x_{j},x_{j+1}]}\in \mathcal{P}_{3}
\end{cases}
$$

### Demostración

Notaremos
$$
S_{j}=S|_{[x_{j},x_{j+1}]} \quad \quad \text{y} \quad \quad h_{j}=x_{j+1} - x_{j}
$$

La función buscada debe cumplir que $S^{\prime\prime}$ sea una poligonal (ENTENDER). Por lo tanto, si $S^{\prime\prime}(x_{j})=y_{j}$, $S^{\prime\prime}$ se escribe como
$$
S_{j}^{\prime \prime }(x)= y_{j} \frac{x_{j+1}-x}{h_{j}}+y_{j+1} \frac{x-x_{j}}{h_{j}}
$$
Partiendo de esto veamos que podemos elegir los $y_{j}$ de forma tal que $S$ cumpla el resto de las condiciones del teorema.
Integramos dos veces y obtenemos

$$
S_{j}(x)= \frac{y_{j}}{6h_{j}}(x_{j+1}-x)^{3}+\frac{y_{j+1}}{6h_{j}}(x-x_{j})^{3}+c_{j}(x-x_{j})+d_{j}(x_{j+1}-x)
$$

donde $c_{j}$, $d_{j}$ son constantes que vienen de la integración.

#### $c_{j}$ y $d_{j}$ para que $S$ sea continua e interpole

Necesitamos que
$$
S_{j}(x_{j})=f(x_{j}) \quad y \quad S_{j}(x_{j+1})=f(x_{j+1})
$$
Reemplazando en la formula de $S_{j}$ obtenemos que
$$
c_{j}=\frac{f(x_{j+1})}{h_{j}}-\frac{y_{j+1}h_{j}}{6} \quad \text{y} \quad d_{j}=\frac{f(x_{j})}{h_{j}}-\frac{y_{j}h_{j}}{6}
$$

reemplazando y derivando nos queda el siguiente problema

#### ${y_{j}}$ para que $S^\prime$ sea continua e interpole

Te queda un sistema con solución una vez dados valores a $y_{0}$ e $y_{n}$ TODO.


















