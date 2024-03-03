
## Enunciado

Sea $U$ un conjunto abierto y conexo, $f:U\to \mathbb{C}$ una [[Función analítica]], entonces $f$ es una [[Función abierta]].

### Demostración

Dado un abierto $V\subset U$, tomemos $f(z_{0})\in f(V)$ y busquemos un entorno de $f(z_{0})$, $\tilde{V}$ tal que $z_{0}\in \tilde{V} \subset f(V)$.

#### Caso $f^{\prime}(z_{0})\neq 0$

Podemos aplicar el [[Teorema de la función inversa complejo|teorema de la función inversa]], ya que $f$ es una [[Función holomorfa]] ([[Yoga de funciones analíticas#Analítica implica holomorfa|analítica implica holomorfa]]) por lo que tenemos $\tilde{U}, \tilde{V}$ entornos de $z_{0}, f(z_{0})$ respectivamente, tales que $f: \tilde{U}\to \tilde{V}$ es biyectiva y $f^{-1}$ es holomorfa. Con esto, tomando $f(\tilde{U}\cap V)$ cumple que:
1. $z_{0} \in f(\tilde{U}\cap V)$.
2. $f(\tilde{U}\cap V)$ es abierto por ser pre imagen de un abierto por una función continua ($f(\tilde{U}\cap V)=(f^{-1})^{-1}(\tilde{U}\cap V))$).
3. $f(\tilde{U}\cap V) \subset f(V)$.

#### Caso $f^{\prime}(z_{0})=0$.

##### Subcaso $z_{0}=0$, $f(z_{0})=0$

Tenemos que 
