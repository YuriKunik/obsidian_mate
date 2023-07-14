
## Enunciado

Sea $A$ un [[Dominio Euclideano]] entonces $A$ es [[Dominio de ideales principales|DIP]].

## Demostración

Dado un [[Ideal]] $I$ queremos ver que existe $a\in A$ tal que $<a> = I$. Como $\mathbb{N}$ es un [[conjunto bien ordenado]] tenemos un elemento $a$ de $A-\{ 0 \}$ con $\delta$ mínimo. Si $\delta(a) =\delta(b)$ entonces $a=bq$ ya que no tenemos $r$ tal que $\delta(r)<\delta(b)$. De la misma manera conseguimos $b=aq^{\prime}$ por lo que $b\sim a$. Tomemos el mínimo $i$ dentro del ideal $I$. Con esto, dado $a \in I$ tenemos que $a=i\cdot q + r$ con $\delta(r) < \delta(i)$ o $\delta(r)=0$. Como $a-i\cdot q \in I$ entonces $r \in I$ por lo que $r = 0$ ya que no puede tener $\delta$ menor que $i$. Entonces $a = iq$ con lo que podemos concluir que $I = <i>$.