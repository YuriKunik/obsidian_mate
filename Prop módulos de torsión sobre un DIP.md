
## Enunciado

Sea $A$ un [[Dominio de ideales principales]], sea $M$ un $A$-[[módulo de torsión ]] y $P \subset A$ un conjunto de representantes de las clases de elementos irreducibles. Entonces 
$$
M = \bigoplus_{p\in P} M(p)
$$

## Demostración

### Ver que genera

Dado un $m \in M$ queremos ver que se escribe como 
$$
m = \sum_{p\in P} m_{p}
$$
con $\text{sop}(M)$ finito.

Como estamos en un DIP. el ideal $An(M)=\{ a \in A / am = 0 \}$ es generado por algún $a \in A$. Como $A$ también es DFU. 
$$
a = u \prod_{p \in P} p^{n_{p}}
$$
con soporte finito $S$. Para conseguir el $m$ tomemos 
$$
a_{p}= \frac{a}{p^{n_{p}}}
$$
Con esto $<a_{p}, p \in S> = 1$ por lo que $\exists b_{p}$ tal que 
$$
\sum_{p \in S} a_{p}b_{p}=1
$$
Multiplicando por m a ambos lados tenemos, $m=\sum_{p \in S}a_{p}b_{p}m$. La gracia de esto es que 
$$
p^{n_{p}}a_{p}m = am=0
$$
por lo que, para todo $p \in S$ $a_{m}m\in M(p)$, lo cual nos dice
$$
m = \sum_{p\in S} a_{p}b_{p}m \in \sum_{p \in S}M(P) \subset \sum_{p \in P}M(P)
$$
### Ver que es [[Suma directa interna]]

Sea $\sum_{i=1}^{N}m_{i}=0$, $m_{i}\in M(p_{i})$, $p_{i}^{n_{i}}m_{i}=0$
Queremos ver que $m_{i}=0 \forall i$. 
Sea $q_{i}=\prod_{j\neq i}p_{j}^{n_{j}}$ entonces $<p_{i}^{n_{i}}, q_{i} > = 1$ por lo que $1 = r_{i} p_{i}^{n_{i}} + s_{i}q_{i}$ con $p_{i}^{m_{i}}=0$. $q_{i}m_{j}=0$ $\forall j\neq i$ Además,
$\sum_{i}m_{i}=0$ de donde $m_{i}=-\sum_{j\neq i}m_{j}$. Entonces $q_{i}m_{i}=0$

Finalmente
$$
\begin{align}
m_{i}&=1m_{i} \\
    &= r_{i}p_{i}^{m_{i}}m_{i}+s_{i}q_{i}m_{i} \\
	&= 0
\end{align}
$$
