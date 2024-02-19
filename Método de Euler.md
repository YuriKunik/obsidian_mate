
## Definición

Dada la ecuación diferencial definida en un intervalo $[t_{0}, T]$
$$
\begin{cases}
x^\prime (t)=f(t,x(t)), \\
x(t_{0})=x_{0}
\end{cases}.
$$

Tomamos $n \in \mathbb{N}$ y puntos equiespaciados $t_{0},\dots t_{n}$ con paso $h=\frac{T-t_{0}}{n}$, de manera que $t_{i}=t_{0}+ih$. Con esto armamos la sucesión del método de la siguiente forma
$$
x_{i+1}= x_{i}+hf(t_{i}, x_{i})
$$

En este caso, tenemos que es un [[Método de un paso]] con $\phi=f$

## Orden del método:

El método de Euler tiene [[Orden de un método (EDO)|orden]] $1$ ya que
$$
\tau=\frac{x(t_{i}+h)-x(t_{i})}{h}-f(t_{i}, x(t_{i}))
$$
que a su vez, por el polinomio de taylor, tenemos
$$
\frac{x(t_{i}+h)-x(t_{i})}{h}-f(t_{i}, x(t_{i})) = \frac{h}{2}f^{\prime\prime }(\xi)
$$
con lo cual $\tau=\frac{h}{2}f^{\prime \prime (\xi)} \sim \mathcal{O}^{2}$

