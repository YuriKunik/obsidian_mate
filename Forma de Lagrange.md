# Polinomio interpolador de Lagrange
## Base de Lagrange

Dados $(x_{i})_{i=0}^n$ datos, la base de Lagrange es
$$
l_{j}(x) = \frac{\prod_{i\neq j}(x-x_{i})}{\prod_{i\neq j}(x_{j}-x_{i})}
$$
estos polinomios de grado $n$ cumplen que 
$$
l_{j}(x_{i}) = \delta_{ij}.
$$

## Polinomio interpolador

Dada una tabla de datos

| $x_{0}$ | $x_{1}$ | $\dots$ | $x_{n}$ |
| ------- | ------- | ------- | ------- |
| $y_{0}$ | $y_{1}$        | $\dots$        | $y_{n}$        |
Existe un único polinomio de grado menor o igual a $n$ que interpola la tabla.

Este polinomio es
$$
p_{n}(x)= \sum_{i=0}^{n}y_{i}l_{j}(x)
$$

## Cálculo del error

Queremos ver que pasa con el error que se comete al interpolar una función mediante un polinomio interpolador. Para esto notamos/definimos lo siguiente.

1. El error va a ser $E_{n}(x)=f(x)-p_{n}(x)$
2. Notemos el siguiente polinomio $W_{n+1}(x)=\prod_{i=0}^{n}(x-x_{i})$
### Teorema 
Sean $f \in C^{n+1}[a,b]$ y $p_{n}\in \mathcal{P}_{n}$ el polinomio interpolador de $f$ en $x_{0}, x_{1}, \dots, x_{n}$. Para cada $x \in [a,b]$ existe $\xi \in [a,b]$ tal que
$$
E_{n}(x)=f(x)-p_{n}(x)= \frac{f^{(n+1)}(\xi)}{(n+1)!}W_{n+1}(x)
$$

#### Demostración

Ya sabemos que la formula del error es valida para los $(x_{j})$. Probémoslo para el resto de los valores en el intervalo. Fijado $x$ definimos la siguiente función de $t$
$$
F(t) = f(t) - p_{n}(t) - \alpha W_{n+1}(t)
$$
con $\alpha = \frac{f(x)-p_{n}(x)}{W_{n+1}(x)}$ para que $F(x) = 0$. Esta función está bien definida y es $0$ para todos los $x_{j}$. Con esto, sabemos por el [[teorema de Rolle]] que $F^{n+1}$ tiene una raíz $\xi \in (a,b)$.
Como
$$
F^{n+1}(t)= f^{n+1}(t)-(n+1)!\alpha
$$
se obtiene, evaluando en $\xi$ la formula que queríamos.
