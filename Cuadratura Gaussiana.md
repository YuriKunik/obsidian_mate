#calculonumerico #integracion 

## Objetivo

Vamos a intentar elegir pesos $A_{j}$ y nodos $\{ x_{0},\dots x_{n} \}$ para tener una regla de exactitud $2n+1$. Esto es deseable ya que tenemos $2n+2$ variables juntando todo.

## Preliminares

Vamos a trabajar en $C[a,b]$ con el producto interno
$$
<f, g> = \int _{a}^b f(x)g(x)w(x) \, dx 
$$
con $w(x)$ una función positiva.

### Teorema: Raíces de polinomios ortonormales

Sea $p_{n}$ el polinomio ortonormal del producto interno previo de grado $n$. Todas sus raíces son distintas y se encuentran en el intervalo $(a,b)$.

#### Demostración

##### 1er paso: $p_{n}$ tiene al menos una raíz real
Caso contrario $p_{n}$ tiene signo constante. Suponiendo, sin perdida de generalidad, que $p_{n}>0$
$$
0=<1,p_{n}> = \int _{a}^b f(x)w(x) \, dx > 0 
$$
Lo cual es absurdo y además nos da que tiene alguna raíz en el intervalo.
##### 2do paso: Las raíces de $p_{n}$ son simples

En el caso de que $(x-r)^{2}|p_{n}$ tenemos que $q=\frac{p_{n}}{(x-r)^{2}}$ es un polinomio de grado menor a $n-1$ por lo que es ortogonal a $p_{n}$. Entonces

$$
0 = <p_{n}, q> = \int p_{n}(x) \frac{p_{n}(x)}{(x-r)^{2}} \, dx >0
$$
absurdo.
##### 3er paso: Todas las raíces están en el intervalo $(a,b)$

Si tenemos raíces fuera del intervalo, entonces $q(x)|p(x)$ con $q(x)$ grado menor estricto que $p(x)$ y con todas sus raíces en $(a,b)$. Entonces $\frac{p(x)}{q(x)}$ se mantiene con el mismo signo en $(a,b)$ (supongamos que es positivo) y, de ser de grado mayor que $0$, entonces
$$
0 = <\frac{p(x)}{q(x)}, 1> = \int \frac{p(x)}{q(x)}w(x) \, dx > 0.
$$
Lo cual es absurdo, por lo que $q(x)=p(x)$.
$\square$

### Teorema: Elección de los nodos de Gauss
La fórmula
$$
\int _{a}^b p(x)w(x) \, dx=\sum_{j=0}^n A_{j}p(x_{j}) 
$$
Vale para cualquier polinomio de grado menor o igual a $2n+1$ si y solo si $\{ x_{0},\dots x_{n} \}$ son los ceros de $p_{n+1}$ (poli ortonormal del producto interno).

#### Demostración

##### Vuelta
Sea $p(x)\in P_{2n+1}$ por el algoritmo de división tenemos
$$
p(x)=S(x)p_{n}(x)+R(x)
$$
con $R(x), S(x) \in \mathcal{P}_{n}$. Ahora, al ser $R(x)$ de grado a lo sumo $n$, vale
$$
I(R)=Q(R)
$$
TODO: Checkear que la cuadratura de $n+1$ puntos coincide con la integral de polinomios degrado n o menos.

Entonces
$$
\begin{align}
I(p) & =\int _{a}^b p(x)w(x) \, dx  \\
     & = \int _{a}^b p_{n+1}(x)S(x)w(x) \, dx + \int _{a}^b R(X)w(x)\, dx  \\
     & = 0 + I(R) \\
     & = Q(R)  \\
     & = \sum_{j=0}^n A_{j}R(x_{j}) \\
     & = \sum_{j=0}^n A_{j}p(x_{j})  \\
     & = Q(p)
\end{align}
$$

##### Ida
Supongamos que $\{ x_{j} \}$ es un conjunto de puntos distintos y se verifica
$$
\int _{a}^b p(x)w(x) \, dx = \sum_{j=0}^nA_{j}p(x_{j})
$$
para todo $p \in \mathcal{P}_{2n+1}$. Queremos ver que $\{ x_{j} \}$ son los ceros del polinomio $p_{n}$ del producto interno actual. Tomando $W(x)=\prod_{j=0}^n(x-x_{j})$ el producto $r(x)W(x)$ esta en $\mathcal{P}_{n+1}$ para todo $r$ en $\mathcal{P}_{n}$. Entonces, por la hipótesis
$$
<r, W> = \int _{a}^b r(x)W(x)w(x) \, dx = \sum_{j=0}^n A_{j}r(x_{j})W(x_{j})=0
$$
por lo que $W$ es un polinomio mónico de grado $n+1$ que resulta ortogonal a cualquier polinomio de grado menor o igual que n, en consecuencia $W(x)=q_{n+1}(x)$ y por lo tanto los $x_{j}$ son los ceros de $p_{n+1}$.
$\square$
##### Observación
Este resultado es óptimo.

### Corolario: condición para las $A_{j}$

Dada una fórmula de cuadratura gaussiana $Q_{n}(f)=\sum_{j=0}^nA_{j}f(x_{j})$, entonces $A_{j}>0$ para todo $j=0,\dots,n$.

#### Demostración
Consideremos los polinomios de la base de Lagrange ([[Forma de Lagrange]]) para $(x_{j})$. Tenemos que $(l_{k})^{2}\in \mathcal{P}_{2n}$ y entonces $I(l^{2}_{k})=Q(l^{2}_{k})$. Como $l_{k}(x_{j})=\delta_{kj}$,

$$
0<\int _{a}^b l^{2}_{k}(x)w(x) \, dx = \sum_{j=0}^nA_{j}(l_{k}(x_{j}))^{2} = A_{k}
$$
$\square$