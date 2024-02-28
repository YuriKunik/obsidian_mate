#complejo #series #seriespotencias 
# Propiedades

Sea $f:U\to \mathbb{C}$ una función
## Analítica $\implies$ Continua.

Si $f$ es [[Función analítica|analítica]] en $z_{0}$, entonces es continua en un entorno de $z_{0}$ y vale $f(z_{0})=a_{0}$.

### Demostración 

Alcanza con ver que, en cierto entorno de $z_{0}$, $f$ es límite [[Convergencia Uniforme|uniforme]] de los polinomios $S_{N}(z)=\sum^N_{n=0}a_{n}(z_{n}-z_{0})^n$. Por lo que es continua ya que límite uniforme de continuas es continua, y $f(z_{0})=a_{0}$ ya que $S(z_{0})=a_{0}$ para todo $N \in \mathbb{N}$.

## Composición de analíticas es analítica.

Si $f$ es [[Función analítica|analítica]] en $z_{0}$ y $g$ es analítica en $f(z_{0})$ entonces $g \circ f$ es analítica en $z_{0}$.

### Demostración

#### Buena definición de $g \circ f$.

Necesitamos un entorno $\tilde{U}$ de $z_{0}$ tal que $f(\tilde{U})\subset Dom(g)$. Tenemos que $g$ es analítica en $f(z_{0})$ por lo que tiene un entorno ${V}$ de $f(z_{0})$ tal que  $g$ es continua. Ahora $f^{-1}({V})$ es un entorno de $z_{0}$ por ser $f$ continua y que cumple que $f(f^{-1}(V))\subset V$. 
Además [[Composición de series de potencias|sabemos que composición de series de potencias es serie de potencias]], por lo que tenemos $g \circ f(z):=\sum_{j\geq 0}a_{j} \left( \sum_{n\geq 1}b_{n}(z-z_{0})^n \right)^j$.

#### Radio de convergencia de la composición

Fijando $r < \rho_{f}$ tal que $\lvert f(z)-f(z_{0}) \rvert < \rho_{g}$ siempre que $\lvert z-z_{0} \rvert<r$ tenemos que la serie converge en $D_{r}(z_{0})$, lo que prueba que el radio de convergencia es mayor o igual que $r$.

## Analítica implica derivable

Si $f$ es analítica en $z_{0}$, entonces es [[Función holomorfa|derivable]] en $z_{0}$ y vale $f^{\prime}(z_{0})=a_{1}$.

### Demostración

Dado $h$ cercano al origen escribimos el cociente incremental
$$
\begin{align}
\frac{f(z_{0}+h)-f(z_{0})}{h} &=\sum_{n\geq 1}a_{n} h^{n-1} \\
	 & =\sum_{n\geq 0}a_{n+1} h^{n} \\
	 & := T(h).
\end{align}
$$
Entonces $T$ es una [[Yoga de funciones analíticas#Analítica $ implies$ Continua|serie de potencias continua]] por lo que $\lim_{ h \to 0 }T(h)=T(0)=a_{1}$.


## Serie de potencias es analítica en todo el radio de convergencia

Sea $S=\sum a_{n}z^{n}$, con [[Radio de convergencia]] $\rho>0$ entonces $S(z)$ es una [[Función analítica]] en $D_{\rho}(0)$ y vale que $S^{\prime}=\sum_{n\geq 0}(n+1)a_{n+1}z^{n}$.
### Aclaración

La definición de una función analítica, nos dice que para cada punto en el conjunto donde sabemos que es analítica, hay una serie de potencias de la forma
$$
A(z)=\sum a_{n} (z-z_{0})^{n}.
$$
Ahora, esto no lo sabemos del mero hecho de tener que $S$ es una serie de potencias. Necesitamos encontrar una serie de potencias centrada en cada punto del radio de potencias.

### Demostración

#### Expresión de la serie de potencias centrada en $z_{0}$:
Dado $z_{0} \in D_{\rho}(0)-\{0\}$ (sacamos el cero ya que en ese punto tenemos la serie de potencias), podemos fijar $r>0$ tal que $r+\lvert z_{0} \rvert<\rho$. Tomando $z \in D_{r}(z_{0})\subset D_{\rho}(0)$ (vale la contención por lo que le pedimos al $r$), escribimos
$$
\begin{align}
\sum_{n\geq 0}^{}  a_{n} z^{n}  &  = \sum_{n\geq 0}^{}  a_{n} (z-z_{0}+z_{0})^{n}  \\
 &   = \sum_{n\geq 0}^{}  a_{n} \sum_{j=0}^{n} {n \choose j} (z-z_{0})^{j}z_{0}^{n-j}  \\
	 &   = \sum_{n\geq 0}^{} \sum_{j=0}^{n} a_{n}{n \choose j} (z-z_{0})^{j}z_{0}^{n-j}  \\
	 &   = \sum_{n\geq 0}^{} \sum_{j\geq 0}^{} I_{[0,n]}(j)a_{n}{n \choose j} (z-z_{0})^{j}z_{0}^{n-j}  \\
\end{align}
$$

Nos gustaría cambiar el orden de las sumatorias pero para eso necesitamos que, llamando $A_{nj}= I_{[0,n]}(j)a_{n}{n \choose j} (z-z_{0})^{j}z_{0}^{n-j}$, 
$$
\sum_{n=0}^{N}  \sum_{j=0}^{M}  \lvert A_{nj} \rvert < C, \quad \forall N,M\in\mathbb{N}.
$$
(vale por lo visto en [[Permutación entre límite y serie#Corolario|intercambio de sumatorias]]). Sabemos que $\sum_{n=0}^{N}  \sum_{j=0}^{M}  \lvert A_{nj} \rvert\leq \sum \sum I_{[0, n]}(j)a_{n}{n \choose j}\lvert  z_{0}\rvert^{n-j} \lvert z-z_{0} \rvert^{j}$. Que nos sirve por cumplir
$$
\sum_{n}\sum_{j} I_{[0, n]}(j)a_{n}{n \choose j}\lvert  z_{0}\rvert^{n-j} \lvert z-z_{0} \rvert^{j} = \sum a_{n} (\lvert z_{0} \rvert + \lvert z-z_{0} \rvert)^{n}.
$$
Para terminar de justificar el cambio en la sumatoria, observemos que $\lvert z_{0} \rvert+\lvert z-z_{0} \rvert\leq \lvert z_{0} \rvert + r < \rho$ por lo que 
$$
\sum a_{n} (\lvert z_{0} \rvert + \lvert z-z_{0} \rvert )^n<\infty.
$$
Con esto conseguimos una cota que nos permite cambiar las sumatorias:

$$
\begin{align}
\sum_{n\geq 0}^{}  a_{n} z^{n}  &   = \sum_{n\geq 0}^{} \sum_{j\geq 0}^{} I_{[0,n]}(j)a_{n}{n \choose j} (z-z_{0})^{j}z_{0}^{n-j}  \\
	 & = \sum_{j\geq 0}\sum_{n\geq 0} I_{[0,n]}(j)a_{n}{n \choose j} (z-z_{0})^{j}z_{0}^{n-j}  \\
	 & = \sum_{j\geq 0}\sum_{n\geq j}a_{n}{n \choose j} (z-z_{0})^{j}z_{0}^{n-j}  \\
	 & = \sum_{j=0}^{\infty}  b_{j} (z-z_{0})^{j}
\end{align}
$$
con 

$$
b_{j} = \sum_{n\geq j}a_{n} {n\choose j}z_{0}^{n-j}.
$$
#### Buena definición de la expresión

Lo último que nos queda verificar es que $b_{j}$ esta bien definido para todo $j$. Esto pasa por que $\sqrt[n]{{n \choose j}} \to 1$, con lo que
$$
\sqrt[n]{ {n\choose k} \lvert a_{n} \rvert  } = \sqrt[n]{{n\choose k}} \sqrt[n]{ \lvert a_{n}  \rvert  }
$$
y, por props del límite superior
$$
\begin{align}
\limsup_{n  \to \infty }  \sqrt[n]{ {n\choose k} \lvert a_{n} \rvert  } & = \limsup_{ n \to \infty }  \sqrt[n]{{n\choose k}} \sqrt[n]{ \lvert a_{n}  \rvert  }  \\
	 & = \lim_{ n \to \infty } \sqrt[n]{{n\choose k}} \limsup_{ n \to \infty } \sqrt[n]{ \lvert a_{n}  \rvert  }   \\
	 & = 1 \rho
\end{align}
$$
donde la última igualdad vale por [[Criterio de Cauchy]]. Entonces la serie
$$
b_{j} = \sum_{n>j}a_{n} {n \choose j}z^j
$$
tiene [[Radio de convergencia]] $\rho$ y, en particular, converge en $z_{0}$.

#### Radio de convergencia y expresión para la derivada.

Con esto nos queda bien definida $\sum_{j\geq 0}^{}b_{j}(z-z_{0})^{n}$ y podemos observar que tiene como radio de convergencia al menos $\rho-\lvert z_{0} \rvert$. Finalmente, por el lema anterior,
$$
S^{\prime }(z_{0})=b_{1}=\sum_{n\geq 1}a_{n} nz_{0}^{n-1}=D_{s}(z_{0}).
$$


## Analítica implica holomorfa

Si $f$ es analítica en $z_{0}$, entonces es una [[Función holomorfa]] en $z_{0}$. Más aún, existe un entorno de $z_{0}$ en el que $f$ es infinitamente derivable. 

### Demostración

Tomando el entorno de $z_{0}$ en el que $f$ coincide con $S$, la serie de potencias centrada en $z_{0}$, entonces, por la prop [[Yoga de funciones analíticas#Serie de potencias es analítica en todo el radio de convergencia|sobre la analicidad de las series de potencias]], $f$ es derivable para todo punto de este entorno y coincide con la serie derivada. Además, como la derivada tiene el mismo radio de convergencia, podemos repetir inductivamente el procedimiento. Para verificar la afirmación anterior, notamos que
$$
\sqrt[n]{ n+1 } \to 1 \quad n\to \infty.
$$
### Observación

Trabajemos un poco más con el resultado anterior. La derivada de $f$ va a satisfacer que, $f^{\prime}(z_{0})=a_{1}$. Ahora, $f^{\prime}$ también es analítica, por lo que $f^{\prime\prime}(z_{0})=\tilde{a_{1}}=2a_{2}$ ya que, en un entorno de $z_{0}$ $f^{\prime}=\sum_{n\geq 0}(n+1)a_{n+1}z^{n}$ . Siguiendo esto, terminamos consiguiendo que
$$
a_{n} = \frac{f^{(n)}(z_{0})}{n!}.
$$
Por lo que podemos concluir
$$
f(z)=\sum_{n\geq 0} \frac{f^{(n)}(z_{0})}{n!}(z-z_{0})^{n}
$$
en un entorno de $z_{0}$.


## Primitiva de una función analítica

Si $f$ es analítica en $U$ y $z_{0}\in U$. Entonces existe un entorno abierto $V\subset U$ de $z_{0}$ y una función $F:V\to \mathbb{C}$ tal que $F^{\prime}(z)=f(z)$ para todo $z \in V$.

### Demostración
Si $f(z)=\sum a_{n}(z-z_{0})^{n}$ en un entorno de $z_{0}$, entonces la serie
$$
I(z)=\sum_{n\geq 0} \frac{a_{n}}{(n+1)}(z-z_{0})^{n}
$$
tiene el mismo radio de convergencia y su derivada coincide con $f$ en un entorno de $z_{0}$.
## Analítica con derivadas nulas

Sea $f$ analítica en $z_{0}$ con $f^{(n)}(z_{0})=0$ para todo $n \in \mathbb{N}_{0}$ entonces $f \equiv 0$ en un entorno de $z_{0}$.

### Demostración

Es directo de [[Yoga de funciones analíticas#Analítica implica holomorfa#Observación]]. 
## Analítica con ceros no aislados

Sea $f$ analítica con $z_{0}$ un $0$ no aislado, entonces $f \equiv 0$ en un entorno de $z_{0}$.

### Demostración

Dado un entorno de $z_{0}$ tal que $f(z)=\sum a_{n} (z-z_{0})^{n}$, entonces, si no vale que $f \equiv 0$, existe un $n_{0}$ mínimo tal que $a_{n_{0}}\neq 0$. Con esto
$$
f(z)=(z-z_{0})^{n_{0}}\sum_{n\geq n_{0}}a_{n} (z-z_{0})^{n-n_{0}}=(z-z_{0})^{n_{0}}h(z)
$$
donde $h(z)$ es una función continua que no se anula en un entorno de $z_{0}$ ya que $h(z_{0})=a_{n_{0}}\neq 0$. Como $(z-z_{0})^{n_{0}}$ solo se anula en $z_{0}$, tenemos que $z_{0}$ no puede ser un $0$ no aislado.

## Condiciones suficientes para que dos funciones analíticas coincidan
1. $f,g:\mathbb{C} \to \mathbb{C}$ tal que $f(x)=g(x)$ para todo $x \in \mathbb{R}$ entonces $f \equiv g$
2. $f,g:U\to \mathbb{C}$ con $U$ abierto conexo. Si $f(z_{n})=g(z_{n})$ para cierto conjunto infinito $\{ z_{n} \}_{n\in\mathbb{N}}\subset K$ con $K$ compacto. Entonces $f \equiv g$ .
3. Sean $U$ abierto, $f:U\to \mathbb{C}$ analítica y $z_{0}\in U$. Si $f\equiv S$ en un entorno de $z_{0}$ y $S$ converge en $D_{r}(z_{0})\subset U$, entonces $f\equiv S$ en $D_{r}(z_{0})$.



## Anillo de funciones analíticas en $U$

Dado $U \subset \mathbb{C}$ abierto conexo, el anillo de funciones analíticas en $U$ es un [[Anillo Íntegro]]:
$$
fg \equiv 0 \implies f\equiv {0} \text{ o } g\equiv 0
$$



