
## Enunciado

Sea $G$ un [[grupo]] y $A$ un conjunto
 en un conjunto $A$, .
Son equivalentes

1. Tener una [[Acción de grupo]] $\sigma:G \to \text{Aut}_{C}(A)$
2.  Tener una función de conjuntos
$$
\rho:G\times A\to A
$$
tal que $\rho(e_{G},a)=a$ $\forall a \in A$ y 
$$
(\forall g, h \in G),(\forall a \in  A): \rho(gh,a)=\rho(g,\rho(h,a))
$$

## Demostración

###  $2\implies 1$ 
Dada una función $\rho$ como en el enunciado, podemos definir el morfismo $\sigma$ como $\sigma(g)=\rho(g,\_)$. Esta función preserva la operación ya que, dados $g,~g' \in G$
$$
\begin{align}
\sigma(gg')(a)&=\rho(gg',a) \\
     & =\rho(g,\rho(g',a)) \\
     & = \sigma(g)(\sigma(g')(a)) \\
     & = \sigma(g)\sigma(g')(a)
\end{align}
$$

Como esto vale para todo $a \in A$ tenemos que $\sigma$ es un morfismo.

###  $1\implies 2$ 

Definimos $\rho(g,a)=\sigma(g)(a)$. Esto cumple todo lo que tiene que cumplir.


