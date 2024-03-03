
## Condición sobre singularidades para que una función entera sea un polinomio.

Sea $f:\mathbb{C}\to \mathbb{C}$ una [[Función entera]]. Si $\infty$ es una [[Singularidad en el infinito]] evitable o un polo, entonces $f$ es un polinomio.

### Demostración

Si $g(z)=f\left( \frac{1}{z} \right)$ se extiende a una función holomorfa, implica que, cerca de $0$, vale $\lvert z^{k}g(z) \rvert\leq M$ para alguna constante $M$, por ser $z^{k}g$ continua.  Entonces, con $w=\frac{1}{z}$. 
$$
\lvert f(w) \rvert \leq M \lvert w \rvert ^{k}
$$
y esto, por el [[Teorema de Louville generalizado]], implica que $f$ es un polinomio de grado menor o igual que $k$.

## Entera y biyectiva

Sea $f:\mathbb{C}\to \mathbb{C}$ una [[Función entera]] y biyectiva, entonces $f$ es una función lineal.