
## Caso 1: Matriz estrictamente dominante

### Definición

Una matriz $A \in \mathbb{R}^{n \times n}$ es estrictamente dominante si
$$
\lvert a_{ii} \rvert > \sum_{i\neq j} \lvert a_{ij} \rvert .
$$
Teniendo una matriz estrictamente dominante ambos métodos convergen.

### Jacobi converge

Con este método $B_{J}=-D^{-1}(L+U)$. Usando como son las matrices, observamos que:
$$
b_{ij} = \frac{a_{ij}}{a_{ii}} \quad \text{para } i \neq j \text{ y } b_{ii} = 0.
$$
entonces 
$$
\lVert B_{j}\rVert_{\infty} = \text{máx}_{i} \sum_{j \neq i} \frac{\lvert a_{ij} \rvert}{\lvert a_{ii} \rvert } < 1
$$
### Gauss Seidel converge

La matriz $B_{gs} = (-L +D)^{-1}U$. Veamos que $\rho (B) < 1$. Sea $\lambda$ un autovalor de $B$ y $x$ un autovector con $\lVert x \rVert_{\infty} = 1$ tenemos que,
$$
-(L+D)^{-1}Ux=\lambda x
$$
es decir
$$
-Ux=\lambda(L+D)x 
$$
$$
-\sum_{j = i+1}^Na_{ij}x_{j} = \lambda \sum_{j=1}^ia_{ij}x_{j}
$$
o, por último
$$
\lambda a_{ii} x_{i} = - \lambda \sum_{j=1}^i a_{ij}x_{j} - \sum^N_{j=i+1} a_{ij}x_{j}
$$
Tomando módulo y un $i$ tal que $\lVert x \rVert_{\infty} = x_{i}$ obtenemos
$$
\lambda \lvert a_{ii} \rvert \leq \lambda \sum_{j=1}^{i-1} \left\lvert  a_{ij} \right\rvert + \sum_{j=i+1}^N \lvert a_{ij} \rvert   
$$
De esta forma

$$
\lvert \lambda \rvert \leq \frac{\sum_{j=i+1}^{N} \lvert  a_{ij} \rvert }{\lvert a_{ii} \rvert - \sum_{j=1}^{i-1} \lvert a_{ij} \rvert } < 1
$$
por ser $A$ estrictamente diagonal dominante.

## Caso 2: Matriz simétrica definida positiva

### Definición

Vamos a trabar con matrices en $\mathbb{C}^{n\times n}$ por lo que vamos a probar el resultado para matrices hermitanas y definidas positivas. Es decir, matrices para las que valga

$$
A = A^* \quad \text{y } z*Az > 0.
$$
### Gauss-Seidel converge

En este caso $A = L + D + L^*$. Veamos que pasa con el radio espectral de $B_{gs} = -(L+D)^{-1}L^*$.

Para empezar, escribamos $B_{gs} =  -(L+D)^{-1} U = -(L+D)^{-1}(A - (L+D))  =I - (L+D)^{-1}A$. Tomando un par autovalor, autovector, tenemos
$$
\begin{align}
(I-(L+D)^{-1}A)z &= \lambda z  \\
(L + D)z - Az &= \lambda(L+D)z  \\
Az &= (1-\lambda) (L+D)z
\end{align}
$$
Como $Az \neq 0$ por ser inversible y $z \neq 0$ entonces $1-\lambda$ es distinto de 0 ($L + D$) también es inversible. Multiplicando por $z^*$ y despejando obtenemos
$$
\frac{1}{1-\lambda} = \frac{z^*(L+D)z}{z^*Az}
$$
que conjugando y teniendo en cuenta que cosas son reales nos da
$$
\frac{1}{1-\bar{\lambda}} = \frac{z^*(L+D)^*z}{z^*Az}= \frac{z^*(L^*+D)z}{z^*Az}
$$
Ahora, sumando las dos igualdades previas:

$$
2 Re\left( \frac{1}{1-\lambda} \right) = 1+ \frac{z^*Dz}{z^*Az} > 1
$$
donde la desigualdad sale de que $A$ es simétrica y definida positiva. La demostración termina con unos jueguitos con el lambda. Si $\lambda = \alpha + i \beta$,
$$
\frac{1}{1-\lambda}=\frac{1}{1 - \alpha - i \beta} \frac{1-\alpha+i\beta}{1-\alpha+i\beta} = \frac{1-\alpha+i\beta}{(1-\alpha)^2 + \beta^2}
$$

Entonces
$$
Re\left( \frac{1}{1-\lambda} \right) = \frac{1-\alpha}{(1-\alpha)^2 + \beta^2} > \frac{1}{2}
$$

Es decir 

$$
2(1-\alpha)>1-2\alpha + \alpha^2 + \alpha^2 + \beta^2
$$
que nos da $1 > \alpha^2 + \beta^2$. Probando así que $\lvert \lambda \rvert < 1$.

TODO: Tridiagonales