#álgebra #categorias 
## Definición

Un **monoide** es un conjunto $M$, junto con un producto $\otimes :M\times M\to M$ de forma tal que;
1. Existe un elemento distinguido $I$ tal que $I \otimes a=a$ y $a \otimes I=a$ para todo $a \in M$.
2. Para todo $a,b,c \in M$, vale que $a \otimes (b \otimes c) = (a\otimes b)\otimes c$.

## Construcción categórica

Otra forma de ver a los monoides es como una [[Categoría]] con un único elemento $m$. En este caso identificamos a los elementos con los morfismos del conjunto $\text{Hom}(m,m)$ 

## Simétrico

Decimos que es simétrico si la operación $\otimes$ es conmutativa.