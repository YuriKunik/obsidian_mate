#complejo #integracion 
## Enunciado

Sean $f:U\to \mathbb{C}$ una [[Función holomorfa]], $\gamma :[a,b]\to \mathbb{C}$ una [[curva]] continua. Entonces existe $F:[a,b]\to \mathbb{C}$ [[Primitivas a lo largo de curvas|primitiva]] de $f$ a lo largo de $\gamma$. Además $F$ es única salvo constantes, lo que permite definir
$$
\int_{\gamma}f(z) \, dz := F(b)-F(a)
$$

## Demostración

Como $f$ es holomorfa, para cada $t \in [a,b]$, existe $\tilde{g}_{t}$ primitiva de $f$ en un entorno de $\gamma(t)$, $V_{t}$ (en un disco más precisamente [[Yoga de funciones analíticas#Primitiva de una función analítica]]). Entonces podemos obtener la definición de $F$ como $F(t):=\tilde{g}(\gamma(t))$. Lo que nos falta es ver que las primitivas se pegan bien. Tomamos el cubrimiento $\{ \gamma ^{-1}(V_{t}) \}$ que por el [[número de Lesbegue]] tenemos $a=t_{0} < t_{1} < \dots t_{n} =b$ de forma tal que $\gamma([t_{j}, t_{j+1}]) \subset V_{t}$. Con esto nos queda fijar bien las constantes de las primitivas. Para esto nos alcanza con la siguiente definición. $g_{0}:= \tilde{g}_{0}$ y
$$
g_{j} := \tilde{g}_{j}-\tilde{g}_{j}(\gamma(t_{j} ))+g_{j-1}(\gamma(t_{j} ))
$$
hasta $j=n$. De está forma, la función $F(t):=g_{j}(\gamma(t))$ para $t \in (t_{j}, t_{j+1}]$ resulta continua.


