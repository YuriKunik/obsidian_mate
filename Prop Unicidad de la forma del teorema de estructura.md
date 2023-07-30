
## Enunciado

Sea $A$ un [[Dominio de ideales principales]], $(n,d_{1},\dots,d_{n})$, $(n',d_{1}',\dots,d'_{n'})$, $n, n' \in \mathbb{N}$, $d_{i},d_{i}' \in A$, $d_{1}|d_{2}|\dots|d_{n}$,$d_{1}'|d_{2}'\dots|d_{n}'$. Suponiendo que los $d_{i}, d_{i}'$ no son [[Grupo de unidades|unidades]].

Si:
$$
M = \bigoplus_{i=1}^{n}A/<d_{i}> \cong  \bigoplus_{i=1}^{n'}A/<d_{i}'> = M'
$$
entonces $n=n'$ y $d_{i} \sim d_{i}'$ para todo $i \in [n]$ 

## Demostración

Sean $M=\oplus_{i=1}^{m}A / <d_{i}> \oplus A^{r}$ y $M'=\oplus_{i=1}^{m'}A / <d_{i}> \oplus A^{r'}$

con los $d_{i}$, $d_{i}'$ dividiendose, dos escrituras basadas en [[Prop Teorema de estructura para módulos finitamente generados sobre un DIP| el teorema de estructura]]. Sumandoles un isomorfismo $f:M\to M'$ queremos ver que 

1. $r=r'$
2. $m=m'$
3. $<d_{i}> = <d_{i}'>$

Como $f(t(M))=t(M')$ entonces $f:\oplus_{i=1}^{n}A / <d_{i}>\to\oplus_{i=1}^{n'}A / <d_{i}'>$ también es un iso
y por lo tanto $\bar{f}:M / t(M) \to M'/t(M')$ también. Entonces $\bar{f}:A^{r}\to A^{r'}$ nos da que, por rango, $r=r'$. 

Para cada $p \in P$, $f(M(p))=M'(p)$. Por lo tanto $\oplus_{i=1}^{m}A / <d_{i}> (p)\cong \oplus_{j=1}^{m'}A / <d_{j}'> (p)$, pero cada componente $p$ primaria tiene una forma conocida, por lo que
$$
\bigoplus_{i=1}^{m}A / < p^{e_{i}} > \to \bigoplus_{j=1}^{m'} A/<p^{e_{j}'}> \quad \text{ con } f \text{ iso}
$$
Con esto el problema se nos transforma en ver que 
$$
m=m', \quad e_{i}=e'_{i}~ ~ ~ ~ \forall i
$$