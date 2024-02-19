
## Idea

Los métodos de Taylor parten de aproximar a $x(t)$ por su [[Polinomio de Taylor]] de orden $k$ y usar eso para conseguir el siguiente punto de la sucesión. Es decir, tomamos el polinomio de taylor centrado en $t$ de orden k y evaluamos en $t+h$
$$
x(t+h)=x(t)+hx^\prime (t)+\frac{1}{2}h^{2}x^{\prime \prime }(t)\dots + \frac{1}{k!}x^{(k)}(t)+\frac{1}{(k+1)!}h^{k+1}x^{k+1}(\xi)
$$
Trabajando en el intervalo $[t_{0},T]$ y buscando obtener una aproximación de $x(T)$. Elegimos $n\in \mathbb{N}$ y $t_{1},\dots t_{n}$ puntos equiespaciados, $t_{i}=t_{0}+ih$, $i=0,\dots n$, con $h=\frac{T-t_{0}}{n}$.

## Orden 1
El método de taylor de orden $1$ es directamente el [[Método de Euler]] ya que
$$
x_{i+1}=x_{i}+hf(t_{i},x_{i}) = x_{i}+hx^\prime (t_{i})
$$
## Orden 2
Para el método de orden 2 necesitamos calcular
$$
\begin{align}
x^{\prime \prime }(t)&=(f(t,x(t)))^\prime  \\
     & = f_{t}(t,x(t))+f_{x}(t,x(t))x^\prime (t) \\
     & = f_{t}(t,x(t))+f_{x}(t,x(t))f(t,x(t)) \\
\end{align}
$$

Entonces nos queda
$$
x_{i+1}=x_{i}+hf(t_{i},x_{i})+\frac{h^{2}}{2}(f_{t}(t_{i},x_{i})+f_{x}(t_{i},x_{i})f(t_{i},x_{i}))
$$
Es decir, es un [[Método de un paso]] con $\phi(t,x,h)=f(t,x)+\frac{h}{2}(f_{t}(t,x)+f_{x}(t,x)f(t,x))$

