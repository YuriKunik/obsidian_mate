
## Construcción

Dados $z=x+iy$ y $f=u+iv$ con $u, v$ funciones de $x,y$. Usando las igualdades elementales
$$
x=\frac{z+\overline{z}}{2} \quad \text{e} \quad y=\frac{z-\overline{z}}{2i}.
$$
Podemos derivar formalmente a $f$ respecto de $z$ y $\overline{z}$ :

$$
\begin{align}
\frac{\partial f }{\partial z}&= \frac{1}{2}u_{x} + \frac{1}{2i}u_{y} + i\left( \frac{1}{2}v_{x} + \frac{1}{2i}v_{y}  \right)  \\
     & =\frac{1}{2}[u_{x}+v_{y}+i(v_{x}-u_{y})]
\end{align}
$$

y 

$$
\begin{align}
\frac{\partial f }{\partial \overline{z}}&= \frac{1}{2}u_{x} - \frac{1}{2i}u_{y} + i\left( \frac{1}{2}v_{x} - \frac{1}{2i}v_{y}  \right)  \\
     & =\frac{1}{2}[u_{x}-v_{y}+i(v_{x}+u_{y})]
\end{align}
$$

Con esto obtenemos que las [[Ecuaciones de Cauchy-Riemann]] implican que, para ser $f$ una [[Función holomorfa]] tiene que tener
$\frac{\partial f}{\partial \overline{z}}=0$.
Otra forma de escribir a los operadores de Wirtinger es:

$$
\frac{\partial f}{\partial z} = \frac{1}{2}\left( \frac{\partial f}{\partial x} - i\frac{\partial f}{\partial y}  \right)
$$

y

$$
\frac{\partial f}{\partial \overline{z}} = \frac{1}{2}\left( \frac{\partial f}{\partial x} + i\frac{\partial f}{\partial y}  \right)
$$
## Regla de la cadena formal

Sea $f=u+iv$ con $u$ y $v$ diferenciables, $\gamma :I\to \mathbb{C}$ una curva derivable, entonces
$$
(f \circ \gamma)^\prime = \frac{\partial f}{\partial z} \gamma^\prime + \frac{\partial f}{\partial \overline{z}} \overline{\gamma^\prime } 
$$
### Demostración

Expandamos el término izquierdo:
$$
\begin{align}
(f \circ \gamma)^\prime (t)  & = (u \circ \gamma)^\prime (t) +(v \circ \gamma)^\prime (t)  \\
 &  = \langle \nabla u, \gamma^\prime  \rangle (t) + i\langle \nabla v,  \gamma^\prime  \rangle (t)     \\
     & = u_{x}\gamma^\prime_{1} + u_{y}\gamma^\prime_{2} + i(v_{x}\gamma^\prime_{1} + v_{y}\gamma^\prime_{2})  \\
     & = \frac{\partial f}{\partial x} \gamma^\prime _{1} +i \frac{\partial f}{\partial y} \gamma ^\prime _{2}
     
\end{align}
$$
calculando $\frac{\partial f}{\partial z}\gamma^\prime + \frac{\partial f}{\partial \overline{z}}\overline{\gamma^\prime}$ vemos que nos queda la igualdad de arriba con lo que concluimos la demostración.











