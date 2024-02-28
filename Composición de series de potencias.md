#complejo #seriespotencias #series 

## Construcción

Queremos definir $A\circ B$ con $$
A = \sum a_{n} z^n \quad B=\sum b_{n} z^n.
$$
Para esto, nos gustaría tener una expresión de la forma
$$
A(B(z))=\sum c_{n}z^{n}.
$$
pero la composición tiene la forma
$$
A(B(z)) = \sum a_{j} B^{j}.
$$

Acá vemos que los términos de orden $n$ van a venir dados por todos los $B^{j}$ . Tranquilamente nos podría quedar $c_{n}$ definido como una serie de términos si para todo $j$, existen en $B^{j}$ términos de orden $n$. Para evitar ese problema, observamos que, con $b_{0}=0$, por el [[Potencias de series con termino nulo|lema]], $B^{j}$ tiene coeficiente no nulo para el término de orden $n$ solo si $j<n$. Por lo que para todo $n$, tenemos finitos términos no nulos, con lo cual no es problema conseguir una expresión para $c_{n}$ (es un problemón pero se puede).


