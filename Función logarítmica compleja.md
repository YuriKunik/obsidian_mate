#complejo #definiciones #funcioneselementales 
## Construcción

Al buscar definir un logaritmos complejo, necesitamos una función $g(z)=x_{0}+iy_{0}$ tal que
$$
e^{g(z)}=z
$$
si $z= \lvert z \rvert e^{iarg(z)}$,nos queda
$$
e^{g(z)}=e^{x_{0}} e^{iy_{0}} .
$$
Igualando módulo y argumento obtenemos que
$$
x_{0}=\ln(\lvert z \rvert) \quad \text{ y } \quad y_{0}=arg(z)+2\pi k
$$
con $k \in\mathbb{Z}$. Así observamos que, para obtener una rama del logaritmo es necesario arreglar al ambigüedad que nos queda de la elección del $k$.

## Definición

Sea $U \in\mathbb{C}-{0}$ un abierto. Una rama del logaritmo en $U$ es una función $g:U\to \mathbb{C}$ continua tal que 
$$
e^{g(z)}= z \quad \forall z \in U.
$$
es decir, que $g(z)$ sea una inversa continua a izquierda de la [[Función exponencial compleja]].

## Propiedades
### Diferencias entre ramas del logaritmo

Si $U$ es conexo, entonces dos ramas del logaritmo definidas en $U$ difieren en un múltiplo de $2\pi i$

#### Demostración

Dadas dos ramas del logaritmo definidas en $U$, $g$ y $\tilde{g}$ tenemos que vale
$$
e^{g(z)}=z=e^{\tilde{g}(z)}
$$
con lo que $e^{{g(z)}-\tilde{g}(z)}=1$. Entonces $$
g(z)-\tilde{g}(z)=2k_{z}\pi i \quad \text{para algún } k_{z} \in\mathbb{Z}
$$
Entonces tenemos una función que va de $U \to 2\pi i\mathbb{Z}$ que, como $U$ es conexo, tiene que ser constante. $\square$

### Derivabilidad

La forma más simple de ver que una rama del logaritmo $g$ es una [[Función holomorfa]] es mediante el [[Teorema de la función inversa complejo]].  Lo verificamos tomando $z_{0}\in U$ y $f(z)=e^z$. Usando el teorema $\exists V, \tilde{U}$ entornos de $z_{0}$ y $g(z_{0})$ respectivamente tales que
$$
f:\tilde{U}\to V \quad \text{es biyectiva}.
$$
Notar que tomamos $g(z_{0}),z_{0}$ ya que $f(g(z_{0}))=z_{0}$ por ser rama del logaritmo. Entonces existe $f^{-1}:V \to \tilde{U}$ que verifica $f(f^{-1}(z))=z$ en $\tilde{U}$. Ahora $z_{0} \in U \cap \tilde{U}$ y es abierto, por lo tanto, tomando $D_{r}(z_{0})\subset U\cap \tilde{U}$ es conexo y abierto y $f^{-1}$, $g$ son ramas del logaritmo por lo que difieren en una constante ([[Logaritmo complejo#Diferencias entre ramas del logaritmo|prop anterior]]). Con esto demostramos que $g$ es holomorfa en $z_{0}$ ya que es suma de holomorfas. 

#### Formula 
Con esto vemos
$$
1 = [e^{g(z)}]^\prime = e^{g(z)}g^\prime (z) \implies g^\prime (z)=\frac{1}{z}
$$





