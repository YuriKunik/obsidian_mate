## Idea
Mediante un [[Método de un paso]] obtener el mismo error que los [[Métodos de Taylor]] pero sin necesidad de conocer las derivadas de $f$. 

## Métodos de orden 2
### Deducción 

El [[Métodos de Taylor#Orden 2|método de taylor de orden 2]] se basa en:

$$
x(t+h)=x(t)+hT_{2}(t,x(t),h)+O(h^{3})
$$

Ahora buscamos $\phi_{2}(t,x,h)$ que no involucre cálculo de derivadas de $f$ y que cumpla

$$
x(t+h)=x(t)+h\phi_{2}(t,x(t),h)+O(h^{3})
$$
Para esto es suficiente que valga
$$
T_{2}(t,x(t),h)-\phi_{2}(t,x(t),h) = O(h^2), \quad \text{(1)}
$$
ya que la fórmula tiene el $h$ multiplicando.

Como candidatos para la función del método proponemos:
$$
A_{1}f(t,x(t)) + A_{2}f(t+\alpha h, x(t)+\alpha hf(t,x(t)))
$$
Es decir, aproximar por $x^\prime$ y por una aproximación de $x^{\prime \prime }$. 
Para despejar $A_{1},A_{2},\alpha$ hacemos Taylor en dos variables para $f(t,x(t))$ incrementando en ambas direcciones  
$$
f(t+\alpha h, x(t)+\alpha f(t,x(t))h) = f(t,x)+f_{t}(t,x)\alpha h + f_{x}(t,x)\alpha hf(t,x)+ O(h^{2}).
$$


Reemplazando todo en (1) tenemos que 
$$
A_{1}+A_{2}=1, \quad \quad A_{2}\alpha=\frac{1}{2}
$$

de donde
$$
A_{2}=\frac{1}{2\alpha} \quad \quad A_{1}=1-\frac{1}{2\alpha}.
$$


Es decir, hay infinitas soluciones dependiendo de $\alpha$

### Fórmula general para orden 2

De la deducción anterior obtenemos una familia de métodos dada por:
$$
x_{i+1}=x_{i}+h\phi_{2}(t,x(t),h) \quad \text{ con } \phi_{2}(t,x,h)=\left( 1-\frac{1}{2\alpha} \right)f(t,x)+ \frac{1}{2\alpha} f(t+\alpha h,x+\alpha hf(t,x)).
$$

### Método de Euler modificado
Tomamos $\alpha = \frac{1}{2}$, con lo que $A_{1}=0$ y $A_{2}=1$.
$$
x_{i+1}=x_{i}+\frac{h}{2}\left[ f\left( t_{i}+\frac{h}{2}, x_{i}+\frac{h}{2}f(t+i,x_{i}) \right) \right]
$$

### Método de Heun
Tomamos $\alpha = 1$, con lo que $A_{1}=A_{2}=\frac{1}{2}$ .
$$
x_{i+1}=x_{i}+\frac{h}{2}\left[f(t_{i}, x_{i}) + f\left( t_{i}+h, x_{i}+hf(t+i,x_{i}) \right) \right]
$$


## Definición General

En el caso general vamos a pedir tener un [[método de un paso]] donde
$$
x_{i+1}=x_{i}+h \phi_{k}(t,x,h)
$$
con 
$$
T_{k}(t,x,h)-\phi_{k}(t,x,h)=O(h^k)
$$
siendo $T_{k}$ el operador del [[Métodos de Taylor|metodo de taylor de orden k]] y 
$$
\phi_{k}(t_{i},x_{i},h)=A_{1}f(\theta_{1},\gamma_{1})+\dots+A_{N}f(\theta_{N},\gamma_{N})
$$
## Método de orden 4
El método de orden $4$ tiene la forma
$$
x_{i+1} = x_{i} + \frac{h}{6}[K_{1}+K_{2}+K_{3}+K_{4}],
$$

Donde,
$$
\begin{align}
K_{1}&=f(t_{i},x_{i}) \quad \quad \quad \quad \quad \quad \quad \quad  K_{3}=f\left( t_{i}+\frac{h}{2}, x_{i}+\frac{h}{2}K_{2} \right)\\
K_{2}&= f\left(  t_{i}+\frac{h}{2} , x_{i} + \frac{h}{2}K_{1} \right) \quad         K_{4}= f(t_{i}+h, x_{i}+hK_{3})
\end{align}
$$


