## Objetivo

Dada una función $f$ vamos a tratar de resolver los siguientes problemas

### Problema A: Versión discreta

Dados $w_{0}, \dots, w_{n}$ constantes positivas, $m< n$ y valores $(x_{i},f(x_{i}))$, con $i=0,\dots n$ se trata de hallar $p \in \mathcal{P}_{n}$ que minimice
$$
\sum_{i=0}^n w_{i}(p(x_{i})-f(x_{i}))^{2}.
$$
### Problema B: Versión continua

Dada una función $w(x)$ positiva en $[a,b]$, dada $f$ y $m \in \mathbb{N}$ se trata de hallar $p \in \mathcal{P}_{m}$ que minimice
$$
\int_{a}^b w(x)(f(x)-p(x))^{2}\, dx 
$$

## Preliminares

Para resolver ambos problemas vamos a trabajar en espacios vectoriales con producto interno. Lo primero que tenemos que notar es que los dos problemas anteriores se traducen a encontrar funciones de un subespacio que minimicen la distancia a nuestra función. La distancia, en este caso, viene dada por una norma.

### Teorema:

Dado un subespacio $S$ de un espacio vectorial con producto interno $V$, tomando $x \in V$, $y \in S$ son equivalentes
1. $\lVert x-y \rVert = \text{mín}_{s \in S}\lVert x-s \rVert$
2. $< x-y, s^\prime> = 0$ para todo $s^\prime \in S$
Además un elemento de $S$ que verifique estas propiedades es único.

#### Demostración

##### $1 \Rightarrow 2$
Sea $s \in S$ veamos que $< x-y, s> = 0$. Tenemos que $y+s \in S$
$$
\lVert x-y \rVert^{2} \leq \lVert x-(y+s) \rVert ^{2}=\lVert x-y \rVert ^{2}- 2 \langle x-y,s \rangle + \lVert s \rVert ^{2}.
$$
Entonces, para todo $s \in S$
$$
\langle x-y, s \rangle \leq \lVert s \rVert ^{2}
$$
en particular vale para $ts$ con $t \in \mathbb{R}$. De esto tenemos que, si $t>0$
$$
\langle x-y, s \rangle \leq t\lVert s \rVert ^{2}
$$
que, haciendo tender $t \to 0$ nos da $\langle x-y,s \rangle\leq 0$. Con $t<0$ obtenemos la otra desigualdad.
##### $2 \Rightarrow 1$
Tomando $s \in S$ usemos que $y-s \in S$. Entonces
$$
\begin{align}
   \lVert x-s \rVert^{2} &= \lVert x-y  + y-s\rVert ^{2} \\
     & = \lVert x-y \rVert ^{2} + \lVert y-s \rVert ^{2} \\
     & \geq \lVert x-y \rVert ^{2}
\end{align}
$$
Tomando raíz cuadrada de ambos lados y mínimo sobre $S$ se obtiene la igualdad ya que $y \in S$.


## Caso discreto
En $\mathbb{R}^n$ consideramos el producto escalar dado por los pesos $w_{0},\dots w_{n}$,
$$
\langle x,y \rangle = \sum^n_{i=0}x_{i}y_{i}w_{i}.
$$
Para los datos $(x_{i}, f(x_{i}))$ queremos encontrar un polinomio $p \in \mathcal{P}_m$ con $n>m+1$ que minimice la distancia entre los vectores $(f(x_{1}),\dots f(x_{n}))$ y $(p(x_{1}), \dots, p(x_{n}))$.

Si $p(x)= \sum_{i=0}^ma_{i}x^i$, entonces tenemos el sistema
$$
Aa=
\begin{pmatrix}
1 & x_{1} & \dots & x_{1}^m \\
1 & x_{2} & \dots & x_{2}^m \\
\vdots & \vdots &  \ddots & \vdots \\
1 & x_{n} & \dots & x_{n}^m \\
\end{pmatrix}

\begin{pmatrix}
a_{0} \\
a_{1} \\
\vdots \\
a_{m}
\end{pmatrix}
=
\begin{pmatrix}
p(x_{1}) \\
p(x_{2}) \\
\vdots \\
p(x_{n})
\end{pmatrix}.
$$

Con esto el problema se traduce a encontrar un vector $a \in \mathbb{R}^{m+1}$ tal que la distancia
$$
\lVert Aa-b \rVert,
$$
sea mínima. 

Para resolverlo en el caso del producto interno euclideo tenemos los resultados siguientes

### Lema: matriz adjunta
Sea $A \in \mathbb{R}^{n\times m}$, $x \in\mathbb{R}^n$, e $y \in \mathbb{R}^m$. Vale
$$
\langle A^Ty, x \rangle = \langle y, Ax \rangle 
$$

#### Demostración:
Hacer la cuenta

### Teorema: Distancia a subespacio

Sea $A \in \mathbb{R}^{n\times m}$ y $b \in \mathbb{R}^n$. Son equivalentes:
1. $x_{0} \in \mathbb{R}^m$ minimiza $\lVert Ax-b \rVert$.
2. $x_{0}$ es solución del sistema $A^TAx=A^Tb$.
Además, si los vectores columnas de la matriz $A$ son linealmente independientes, existe $x_{0}$, solución del sistema y es único.

#### Demostración:

Notemos por $S$ al subespacio $\text{im}(A)\subset \mathbb{R}^n$. Con esto $1$ nos dice que $x_{0}$ está minimizando la distancia a $S$, que sabemos por el teorema de los preliminares que es equivalente a
$$
\langle b-Ax_{0}, Ax \rangle = 0 \quad\forall x \in  \mathbb{R}^m
$$
Por el lema anterior, sabemos que esto también es equivalente a que
$$
\langle A^T(b-Ax_{0}), x \rangle = 0 \quad\forall x \in  \mathbb{R}^m,
$$

inclusive para $x=A^T(b-Ax_{0})$, con lo cual $x_{0}$ cumple
$$
A^TAx_{0}=A^Tb.
$$
yendo para atrás tenemos la vuelta. Para la unicidad llamemos $A_{j}$ a los vectores columnas de $A$. Asumamos que son li. Siempre podemos escribir a $Ax$ como $$
Ax = \sum_{i=1}^{m}A_{j}x_{j}.
$$
Ahora, veamos que $A^TA$ es inversible. Si $A^TAx=0$ 
$$
\langle A^TAx, x \rangle = 0 
$$
con lo que $\lVert Ax \rVert^{2} = 0$ lo que implica que $Ax=0$ y por lo tanto que $x=0$ ya que las columnas de $A$ eran l.i. 

## Caso continuo

Vamos a usar bases ortonormales aprovechando la propiedad de que todo $x \in V$ se escribe como
$$
x=\sum_{i=1}^n \langle x,v_{i} \rangle v_{i}
$$

### Teorema: Existencia de realizador de la distancia

Dado $x \in V$ y un subespacio $S\subset V$ de dimensión finita, existe un único $y\in S$ que satisface
$$
\langle x-y,s \rangle = 0 \quad \forall s \in  S.
$$
#### Demostración:

Sea $\{ v_{1},\dots,v_{n} \}$ una bon. de $S$. El elemento $y$ buscado es 
$$
y = \sum_{i=1}^n \langle x, v_{i} \rangle v_{i}.
$$
En efecto, veamos que vale lo pedido para cada elemento de la base (y por lo tanto para cualquier $s \in S$)
$$
\begin{align}
\langle x-y, v_{j} \rangle &= \langle x, v_{j} \rangle - \langle y, v_{j} \rangle  \\
     & = \langle  x, v_{j}  \rangle - \langle x, v_{j} \rangle  \\
     & = 0
\end{align}
$$
La unicidad la sabíamos de antes.

Con esto podemos definir la proyección $P:V\to S$ que por el teorema de equivalencia de distancia a un subespacio sabemos que nos va a dar el elemento a distancia mínima de $S$ para cada $v$.

### Proyección sobre el subespacio de polinomios

Tomando $V = C[a, b]$ y el subespacio $S=\mathcal{P}_{n}$, dado un producto interno obtenemos una base ortogonal $\{ q_{0},\dots, q_{n} \}$ partiendo de $\{ 1,x, \dots x^n \}$ y una ortonormal $\{p_{0},\dots, p_{n} \}$.

La forma que tienen estos polinomios es
$$
q_{0}=1, \quad p_{0}=\frac{1}{\lVert q_{0} \rVert }
$$
y
$$
q_{k}(x)=x^k - \sum_{i=1}^{k-1}\langle x^k,p_{i} \rangle p_{i}(x) \quad p_{k}(x)=\frac{q_{k}}{\lVert q_{k} \rVert }.
$$
#### Forma general
Con esto, la solución al problema se sigue de los teoremas demostrados anteriormente y va a ser
$$
P(f)=\sum_{i=0}^n \langle f,p_{i} \rangle p_{i}
$$

#### Forma recursiva
Si un producto interno en $C[a,b]$ satisface que $\langle xf,g \rangle=\langle f,xg \rangle$ entonces los polinomios ortogonales mónicos satisfacen

$$
q_{n}(x)=(x-a_{n})q_{n-1}(x)-b_{n}q_{n-2}(x)
$$
con 
$$
a_{n}= \frac{\langle xq_{n-1}, q_{n-1} \rangle }{\langle q_{n-1}, q_{n-1} \rangle } \quad b_{n}= \frac{\langle q_{n-1}, q_{n-1} \rangle }{\langle q_{n-2}, q_{n-2} \rangle }
$$
##### Demostración

Sea $n \geq 2$. Como $0$ es raíz del polinomio $q_{n}(x)-q_{n}(0)$
$$
xr_{n-1}=q_{n}(x)-q_{n}(0)
$$
Como $q_{n}$ es mónico, $r_{n-1}$ también lo es. Entonces
$$
q_{n} (x)=xr_{n-1} (x)+q_{n} (0)=xq_{n-1}+x(r_{n-1}(x)-q_{n-1}(x) )+q(0)  
$$
Ahora $r_{n-1}-q_{n-1}$ es de grado menor o igual a $n-2$ por ser ambos restandos mónicos. Usando que tenemos una base ortonormal de $\mathcal{P}_{n-1}$ escribimos
$$
x(r_{n-1}(x)-q_{n-1}(x) )+q_{n}(0) = \sum_{j=0}^{n-1}\beta _{j} q_{j} (x)
$$
Si $i < n-2$
$$
\begin{align}
0 &= \langle q_{n} , q_{i}  \rangle  \\
&= \langle  (x+\beta_{n-1})q_{n-1}(x)+\sum_{j=0}^{n-2} \langle \beta_{j}, q_{j} \rangle, q_{i}   \rangle  \\
&=\langle xq_{n-1}, q_{i}  \rangle + \beta_{i} \langle q_{i} , q_{i}  \rangle  

\end{align}
$$
Ahora, $xq_{i}$ es de grado menor o igual a $n-1$. Entonces
$$
\langle xq_{n-1}, q_{i}   \rangle=\langle q_{n-1}, xq_{i}   \rangle  = 0
$$
Con lo que concluimos que $\beta_{i}=0$ para $i<n-2$. Por lo tanto, si
$a_{n}=-\beta_{n-1}$ y $b_{n}=-\beta_{n-2}$ conseguimos la formula recursiva del enunciado.
Para obtener una expresión de los $a_{n}$ y $b_{n}$ hacemos producto interno entre $q_{n}$ y $q_{n-1}$ por un lado y $q_{n}$ y $q_{n-2}$ por el otro . 