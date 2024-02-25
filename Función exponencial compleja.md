#complejo #funcioneselementales 

## Definición

Dado $z=x+yi \in \mathbb{C}$ definimos la función exponencial como
$$
e^z=e^x(\cos(y)+i\sin(y)).
$$

## Propiedades

### Derivabilidad

Veamos que $f(z)=e^z$  es una [[Función holomorfa]]. Las [[Ecuaciones de Cauchy-Riemann]] nos quedan
$$
u_{x}=e^x\cos(y)= v_{y}
$$
y
$$
u_{y} = -e^x\sin(y)=-v_{x}.
$$

### Invarianza frente a la derivación

Armando la derivada con las funciones coordenadas tenemos
$$
f^{\prime} = u_{x} + iv_{x} = f.
$$

Con lo que la exponencial compleja sigue cumpliendo lo mismo que cumplía en $\mathbb{R}$. Además sigue siendo la única con $f(0)=1$ y en este caso podemos probarlo sin necesidad de ecuaciones diferenciales.

#### Unicidad de funciones invariantes al derivarlas

Supongamos que existe $g$ satisfaciendo $g^\prime = g$ y $g(0)=1$. Entonces, usando que $f(z)=e^z$ no se anula:
$$
h(z)=\frac{g(z)}{f(z)}
$$
es derivable con derivada:
$$
h^\prime (z)= \frac{g(z)f(z)-g(z)f(z)}{f(z)^{2}}= 0
$$
por lo que $h(z) \equiv 1$ usando que [[Derivada nula implica función constante]]
