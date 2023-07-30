
## Enunciado

Sea $A$ un [[Dominio de ideales principales]], $\alpha \in A^{r\times s}$ una [[Matriz en anillos|matriz]], entonces existe $\beta \in A^{r\times s}$ tal que $\beta$ es diagonal ($\beta_{ij}=0$ si $i\neq j$) y $\alpha \equiv\beta$

## Demostración

La demostración consiste en dar un algoritmo para diagonalizar matrices.

La prueba es en dos pasos

### Paso (a)

#### Enunciado

Existen matrices elementales $E_{1},\dots,E_{n} \in A^{r\times r}$ $E_{1}^{\prime},\dots,E_{n}^{\prime} \in A^{s\times s}$ tales que 
$$
\beta = E_{1}\dots E_{n}\alpha E^{\prime}_{1}\dots E^{\prime}_{n}
$$
es diagonal $\beta=\text{diag}(d_{1},d_{1},\dots d_{R})$ con $R=\text{mín}\{ r, s \}$

#### Demostración

Supongamos que $A$ es un [[Dominio Euclideano]], con $\delta:A-\{ 0 \}\to \mathbb{N}$

Si $\alpha=0$, $\alpha$ es diagonal

Si $\alpha\neq 0$, sea
$$
\delta(\alpha)=\text{mín}\{ \delta(\alpha_{ij}),\alpha_{ij}\neq 0, 1\leq i\leq r, 1\leq j\leq s \},
$$
tomemos el $(i, j)$ para que este mínimo se realice ($\delta(\alpha)=\delta(\alpha_{ij})$). Dividamos cada elemento de fila $i$ y columna $j$ por $\alpha_{ij}$ de la siguiente forma
$$
\alpha_{kj}=\alpha_{ij}q_{kj}+r_{kj}\quad \text{donde } r_{kj}=0 \text{ o } \delta(r_{kj})\leq\delta(\alpha_{ij})
$$
Por [[Operaciones elementales de matrices]] remplazamos cada $\alpha_{kj}$ por $r_{kj}$. Para las columnas procedemos de forma parecida pero con $\alpha_{ik}$.
Esto nos deja en dos posibles casos, 
1. La nueva fila $i$ y la nueva columna $j$ son nulas (excepto en el lugar $(i,j)$). Si pasa esto seguimos con la matriz $(r-1)\times(r-1)$ ya que podemos permutar para llevar $(i,j)$ a $(1,1)$. Denotamos a $\alpha_{ij}=d_{1}$
2. Volvemos a calcular $\delta(\alpha)$ y este va a ser estrictamente más chico que el anterior. Iteramos y después de finitos casos tenemos que llegar al caso 1.


### Paso (b)

#### Enunciado

Además $\beta$ a $\text{diag}(d_{1}^{\prime},d_{2}^{\prime},\dots,d_{R}^{\prime})$ con $d_{1}^{\prime} | d_{2}^{\prime}, d_{2}^{\prime}|d_{3}^{\prime},\dots,d_{R-1}^{\prime} | d_{R}^{\prime}$

#### Demostración

Hagamos los siguientes casos a mano

##### $r=s=2$
Con $d\equiv d^{\prime}=\text{diag}(d_{1}^{\prime}, d_{2}^{\prime})$
para esto tomamos $d_{1}^{\prime}=\text{mcd}\{ d_{1},d_{2} \}$, $d_{2}^{\prime}=\frac{d_{1}d_{2}}{d_{1}^{\prime}}$ 

Como $d_{1}^{\prime} | d_{1},d_{2}$, $d_{1}=d_{1}^{\prime}e_{1}$ y $d_{2}=d_{1}^{\prime}e_{2}$ con $e_{1},e_{2} \in A$ y también $d_{1}^{\prime}=rd_{1}+sd_{2}$
Hagamos cuentas
$$
\begin{align}

\begin{pmatrix}
d_{1} & 0 \\
0 & d_{2}
\end{pmatrix}
& \equiv
\begin{pmatrix}
d_{1} & d_{2} \\
0 & d_{2} \\ 
\end{pmatrix}\quad (1)
 \\
 
&\equiv
\begin{pmatrix}
d_{1} & d_{2} \\
0 & d_{2} \\ 
\end{pmatrix}
\begin{pmatrix}
r & -e_{2} \\
s & e_{1} \\ 
\end{pmatrix} \quad (2)\\

& = 
\begin{pmatrix}
d_{1}^{\prime} & 0 \\
d_{2}s & d_{2}^{\prime}
\end{pmatrix} \quad (3)\\

&\equiv
\begin{pmatrix}
d_{1}^{\prime} & 0 \\
0 & d_{2}^{\prime}
\end{pmatrix}\quad (4)

\end{align}
$$

Aclarando un poco, $(1)$ es sumar la 2da fila a la primera
$(2)$ es multiplicar por una matriz con determinante 1, (3)
el resultado de la multiplicación y $(4)$ restar la 1ra fila a la segunda y luego restar la primera otra vez pero multiplicada por $re_{1}$.

##### $r=s=3$

Tenemos $\text{diag}(d_{1},d_{2},d_{3})$
$$
\begin{align}
\text{diag}(d_{1},d_{2},d_{3}) & \equiv\text{diag}(d_{1}', d_{2}', d_{3}) \\
	 & \equiv \text{diag}(d_{1}'',d_{2}', d_{3}'') \\
	 & \equiv \text{diag}(d_{1}'',d_{2}'',d_{3}'')
\end{align}
$$
Por cuestiones del caso anterior se puede ver que $d_{1}''|d_{2}''|d_{3}''$

##### Caso general

Por inducción en $N$:

$$
\begin{align}
\text{diag}(d_{1},d_{2},\dots,d_{N}) &\equiv \text{diag}(d_{1}',d_{2}',\dots,d_{N}) \\
 &\equiv   \text{diag}(d_{1}'',d_{2}',d_{3}',\dots,d_{N}')  \\
&\equiv \text{diag}(D_{1},D_{2},\dots,D_{N})
\end{align}
$$

En la primera igualdad aplicamos el caso base, en la segunda la HI. a $(d_{1}',d_{3},\dots,d_{N})$ y en la última a $(d_{2}',d_{3}',\dots, d_{N}')$.
