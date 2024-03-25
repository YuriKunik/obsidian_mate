
## Construcción

### Orden $1$

Dada $f:U \subset E\to F$, $E, F$ [[espacio normado|espacios normados]]. Si $f$ es diferenciable y su diferencial $Df:U \to B(E,F)$ es continuo, decimos que $f$ es $C^{1}$.

### Orden 2

Nos podemos preguntar si $Df$ es diferenciable, esto es ver que exista $T:U\to B(E,B(E,F))$ transformación lineal de manera tal que
$$
\lim_{ h \to 0 } \frac{Df(x+h)-Df(x)-T_{x}(h)}{h} = 0
$$
para cada $x \in U$, con $T(x)(h)=T_{x}(h)$. Función exponencial por medio, podemos identificar a $T$ con $D^{2}f: E\times E\to F$ tomando $D^{2}f(x,y):= T_{x}(y)$. Con esto, $D^{2}(f)$ es una [[Forma multilineal]] y además se puede probar que es simétrica. 

### Caso general

Finalmente tenemos que $f$ es $C^{k}$ si $D^{k}f :U\to B_{sim}(E^{k}, F)$ es continuo.
