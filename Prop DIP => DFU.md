
## Enunciado

Sea $A$ un [[Anillo]], entonces si $A$ es un [[Dominio de ideales principales]],  también es un [[Dominio de factorización única]].

## Demostración

Sea $A$ un [[Dominio de ideales principales]], por [[Prop DIP => primo es equivalente a irreducible]] sabemos que cumple la segunda condición de ser DFU, (según [[Prop DFU es casi equivalente a que primo = irreducible]]). Nos falta ver que DIP. implica que todo elemento se escribe como un producto de [[Elemento irreducible|elementos irreducibles]].

Para esto usemos que DIP implica [[Anillo noetheriano]] ya que todo [[Ideal]] es un [[Ideal finitamente generado]] al ser generado por un único elemento ([[Prop Equivalencia de Noetheriano para anillos]]). Con esto en mente veamos como podemos obtener una escritura en elementos irreducibles para un $a \in A$.

En la demo de abajo vamos a usar constantemente [[Prop DIP => todo elemento es divisible por un irreducible]]

Tomemos $a \in A$ entonces existe $p_{0}$ tal que $p_{0} | a$, llamemos $b_{0}$ al elemento de $A$ tal que $b_{0}p_{0}=a$. Para $b_{0}$ existe $p_{1}$ irreducible que lo divide, y $b_{1}$ tal que $b_{1}p_{1}=b_{0}$. Este $p_{1}$ sigue dividiendo a $a$ ya que divide a $b_{0}$ y $b_{1}$ divide a $b_{0}$. Siguiendo así nos armamos una sucesión, $b_{0},b_{1},\dots,b_{n}$ junto con otra de irreducibles, $p_{1},p_{2},\dots,p_{n}$ tal que $b_{n}p_{n}=b_{n-1}$. Los $b_{n}$ nos dan una cadena, $<b_{0}>\subset<b_{1}>\subset\dots$ que por noetherianidad se estaciona para un $N$. Cuando $<b_{N}>= < b_{N+1} >$, $p_{N+1}b_{N+1}=p_{N+1}sb_{N}=b_{N}$ con $s \in A^{*}$. Esto nos dice que $p_{N+1}$ no puede ser irreducible, ya que $p_{N+1}s-1=0$ por lo tanto $b_{N}$ no admitía ningún divisor irreducible, lo que hace que $b_{N}$ sea una unidad. Con lo cual nos queda que 
$$
a=p_{0}p_{1}\dots p_{N} b_{N}
$$
con $p_{0},\dots,p_{n}$ irreducibles y $b_{N}$ una unidad.
