
## Enunciado

Sea $A$ un [[dominio]]. Son equivalentes
1. $A$ es [[Dominio de factorización única|DFU]] 
2. Vale la primera propiedad de los DFU y todo elemento irreducible es primo.

## Demostración

### 1) $\implies$ 2)

Sabemos que [[Prop elemento primo implica irreducible|primo implica irreducible]], veamos que en un DFU también vale la vuelta. Sea $a$ un [[Elemento irreducible]] queremos ver que, si $a|xy$ entonces $a|x$ o $a|y$.
Al estar en un DFU, $x=r_{1}r_{2}\dots r_{n}$  e $y=s_{1}s_{2}\dots s_{m}$ lo cual nos da una escritura en irreducibles de $xy = r_{1}r_{2}\dots r_{n}s_{1}s_{2}\dots s_{n}$. Ahora $a|xy$ entonces $ak=xy$. El producto $ak$ tiene como escritura $at_{1}t_{2}\dots t_{n+m-1}$ con $k=t_{1}t_{2}\dots t_{n+m-1}$ entonces $a\sim r_{j}$ o $a\sim{s_{i}}$ por lo que $a|x$ o $a|y$ demostrando así que va a ser primo.

### 2) $\implies$ 1)

Supongamos que  tenemos dos factorizaciones para un elemento $a\in A$:
$$
a=r_{1}r_{2}\dots r_{n}
$$
$$
a = s_{1}s_{2}\dots s_{m}
$$
$r_{1}|a=s_{1}s_{2}\dots s_{m}$ entonces $r_{1}|s_{j}$, al ser $r_{1}$ irreducible no es una [[Grupo de unidades|unidad]]  por lo que está [[Elementos asociados|asociado]] a $s_{j}$. Ahora tachamos estos dos elementos y seguimos... 