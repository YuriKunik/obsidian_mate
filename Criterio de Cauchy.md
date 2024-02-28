
## Enunciado

Dada una serie de potencias con coeficientes $\{ a_{n} \}$, definimos
$$
L := \limsup_{ n \to \infty } \sqrt[n]{ \lvert a_{n}  \rvert  }
$$
entonces el [[Radio de convergencia]] cumple $\rho=\frac{1}{L}$.

## Demostración

### $r> \frac{1}{L} \implies a_{n}r^n\nrightarrow 0  \implies \sum a_{n}z^n$ diverge
Dado $r > \frac{1}{L}$, queremos ver que $a_{n}r^n$ no está acotada. Como $L > \frac{1}{r}$ entonces existen infinitos valores de $n$ para los que $\sqrt[n]{ \lvert a_{n} \rvert }> \frac{1}{r}$ o, lo que es equivalente $\lvert a_{n} \rvert r^n > 1$ para infinitos valores. Por lo tanto, $a_{n}r^n \nrightarrow 0$ que a su vez implica que, si $r> \frac{1}{L}$ y tomamos $z$ con $\lvert z \rvert = r$ entonces $\sum a_{n}z^n$ diverge. 

### $r< \frac{1}{L} \implies \sqrt[n]{ \lvert a_{n} \rvert }< \frac{1}{r}$ luego $a_{n}r^n$ es acotada $\implies r\in \mathcal{A}$

