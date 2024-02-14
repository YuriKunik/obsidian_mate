
## Enunciado

Sea $A$ un [[Dominio de ideales principales|DIP]] entonces todo [[elemento irreducible]] de $A$ es un [[Elementos primos en A|elemento primo]].

## Demostración

Sabemos que todo primo es irreducible. Tomemos $p\in A$ un elemento irreducible y veamos que es primo. Dados $x,y\in A$ tales que $p|xy$, supongamos que $p\nmid x$. Como estamos en un DIP $<p,x> = <\alpha>$. Esto nos dice que $\alpha|p$ ya que $<p> \subset <p,x> = <\alpha>$. Usando que $p$ es irreducible, $\alpha \sim p$ o $\alpha\in A^{*}$. Si $\alpha \sim p$ entonces $x=pk$ lo cual es absurdo ya que $p \nmid x$. Si $\alpha\in A^{*}$ $<p, x> = A$ con lo que $kpy + qxy = y$. Sumando a esto que $pk^{\prime} = xy$ nos queda que $(ky + qk^{\prime})p=y$ con lo que $p|y$.