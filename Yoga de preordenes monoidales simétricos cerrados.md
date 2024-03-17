#7sketches 

Sea $\mathcal{V}$ un [[Preorden monoidal simétrico cerrado]] veamos las consecuencias básicas que tiene esta definición

## Equivalencia de la definición 

Ejercicio 2.8.2 7sketches.

### Preliminares

Tomemos los mapas $(- \otimes v):V\to V$ y $(v \multimap -):V\to V$ teniendo la definición esperada.

### $(v \multimap w)\otimes v \leq w$

Sale directamente de la definición del elemento hom. Sabiendo que vale
$$
(v\multimap w)\leq (v\multimap w) 
$$
tenemos
$$
(v\multimap w)\otimes v \leq w
$$


### $(u \multimap v)\otimes(v\multimap w)\leq (u \multimap w)$

Despejando el $u$ nos queda equivalente a que
$$
(u\multimap v) \otimes (v\multimap w) \otimes u \leq w
$$
pero esto es cierto ya que
$$
(u\multimap v) \otimes (v \multimap w) \otimes u \leq (v\multimap w) \otimes v \leq w 
$$
usando dos veces el item anterior.

### $(- \otimes v)$ es monótona
Tenemos que $(- \otimes v)$ es monótona ya que
$$
x \leq y \implies x \otimes v \leq y \otimes v.
$$

### $(v \multimap -)$ es monótona

Queremos ver
$$
x\leq y \implies (v\multimap x) \leq (v\multimap y)
$$

$$
(v\multimap x) \otimes v\leq  y \implies (v\multimap x) \leq (v \multimap y)
$$
donde la primera desigualdad viene de que $(v \multimap x)\otimes v \leq x \leq y$

### Equivalencia de la definición con respecto a la adjunción

Veamos que un [[Preorden monoidal simétrico]] es cerrado sii $(- \otimes v)$ tiene [[Conexión de Galois|adjunto a derecha]]. En realidad no tenemos que probar nada ya que $v \multimap -$ es monótono, y $(- \otimes v)$ también y la definición de [[Preorden monoidal simétrico cerrado]] es identica a tener una [[Conexión de Galois]] por lo que no nos queda nada que probar y $g(w)$ nos daría el elemento hom para $v \multimap w$.




