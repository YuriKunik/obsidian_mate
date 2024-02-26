
## Enunciado

Dada una serie de potencias con coeficientes $\{ a_{n} \}$, definimos
$$
L := \limsup_{ n \to \infty } \sqrt[n]{ \lvert a_{n}  \rvert  }
$$
entonces el [[Radio de convergencia]] cumple que $\rho=\frac{1}{L}$.

## Demostración

Dado $r > \frac{1}{L}$, queremos ver que $a_{n}r^n$ no está acotada. Como $L > \frac{1}{r}$ entonces existen infinitos valores de $n$ para los que $\sqrt[n]{ \lvert a_{n} \rvert }> \frac{1}{r}$ o, lo que es equivalente $\lvert a_{n} \rvert r^n > 1$ para infinitos valores