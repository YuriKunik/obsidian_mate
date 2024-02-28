#complejo #series #seriespotencias #inducción   
## Enunciado

Sea $A=\sum a_{n}z^n$ una serie de potencias con $a_{0}=0$, entonces $A^j$ tiene término de orden $n$ nulo para todo $n < j$.

## Demostración 

Hagamos la demostración por inducción en $j$.

### Caso base:

Tomando $j=1$, tenemos que $a_{0}=0$ por lo que vale el enunciado.

### Caso general:

Asumamos que para todo $h<j$ vale que los términos $n$-ésimos con $n<h$ de la serie $A^h$ son nulos. Tomemos $n < j$ y tratemos de mostrar que el término de orden $n$ de $A^j$ es nulo. Vale que $A^j=A^{j-1}A$, con $A^{j-1}$ teniendo todos los términos de orden $< j-1$ nulos. Con ésto ya estaríamos en el caso en el que $n<j-1$ ya que, si 
$$
A^j = \sum_{k\geq 0}c^{(j)}_{k}z^k
$$
entonces
$$
c^{j}_{n}=\sum_{k=0}^n c^{(j-1)}_{k}a_{n-k}=0.
$$

Ahora, si $n=j-1$ entonces
$$
\begin{align}
c^{j}_{n}&=\sum_{k=0}^{j-1} c^{(j-1)}_{k}a_{n-k} \\
	 & = c^{j-1}_{j-1}a_{0}  \\
	 & = 0.
\end{align}
$$

Lo que termina la demostración.