
## Enunciado

Sea $A$ un [[Anillo noetheriano]], entonces $A[x]$ es noetheriano.

## Demostración

Sea $J$ un [[ideal]] de $A[x]$ por [[Prop Equivalencia de Noetheriano para anillos]] nos alcanza ver que es un [[Ideal finitamente generado]]. Tomemos los ideales de $A$
$$
J^{n}=\{ a \in A / \exists f\in J \text{ con } f=ax^{n}+ a_{n-1}x^{n-1}\dots + a_{0} \}.
$$
Es claro que son ideales, nos falta ver que son una cadena. Dado $a \in J^{n}$ entonces $\exists f$ con $\text{gr(f)=n}$ y coeficiente principal $a$, con esto $xf \in J^{n+1}$ ya que es de grado $n+1$ y es de la forma $ax^{n+1}+a_{n-1}x^{n}\dots a_{0}x$. Como $J^{n}\subset J^{n+1}$ existe $N$ tal que $J^{n}=J^{N}$ para todo $n\geq N$. Por ser ideales, estos $J'$s son finitamente generados, con lo cual existen $(a_{i}^{j})_{i\leq r(j)}$ tal que generan $J^{j}$ para todo $0\leq j \leq N$. La clave de la demostración es que vamos a tener
$$
J= < f_{i}^{j}, 0\leq i\leq r(j)~ ~ ~ 0\leq j\leq N >
$$

Veamos haciendo inducción en el grado de $f \in J$ 

### Caso base:$d=0$
$f \in J$ de grado $0$ es una constante, por lo tanto $a \in J_{0}$ ya que $a = f$ como $J_{0}= <f_{i}^{0}, 0\leq i \leq r(0)> \subset < f_{i}^{j}, 0\leq i\leq r(j)~ ~ ~ 0\leq j\leq N >$ estamos.

### Paso inductivo
Si todo $f$ de grado $d$ está en el ideal generado por los $f_{i}^{j}$ tomemos un polinomio de grado $d+1$ y veamos que también lo está. Tenemos dos casos:

#### $d\leq N$

El coeficiente principal $a_{d}$ esta en $J_{d}$, entonces 
$$a_{d}=\sum_{i=0}^{r(d)}b_{i}a_{i}^{d}.$$
Con esta construcción 
$$
\text{gr}(f-\sum_{i=0}^{r(d)}b_{i}f_{i}^{d}) < d
$$
ya que le sacamos el coeficiente principal, con lo que $f \in <f_{i}^{j}>$

#### $d > N$

Tenemos que $a_{d} \in J_{d} = J_{N}$ entonces $a_{d}= \sum_{i=1}^{r(N)}b_{i}a_{i}^{N}$

$$
\text{gr}(f-x^{d-N}\sum_{i=0}^{r(N)}b_{i}f_{i}^{N}) < d
$$
entonces $f \in <f_{i}^{n}>$.