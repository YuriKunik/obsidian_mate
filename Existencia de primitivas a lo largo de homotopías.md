
## Enunciado

Sean $f:U\to \mathbb{C}$ una [[Función holomorfa]] y $h:[a,b]\times[0,1]\to U$  continua. Entonces existe $F:[a,b]\times[0,1]\to \mathbb{C}$ [[Primitiva a lo largo de homotopías|primitiva]] de $f$ según $h$, que resulta única salvo constantes.

## Demostración

El procedimiento es análogo al utilizado en [[Existencia de primitiva a lo largo de una curva]]. Para cada $(t,s)$ existe un disco $V_{(t,s)}$ centrado en $h(t,s)$ donde $f$ tiene primitiva $g_{(t,s)}$. Volviendo a utilizar el [[número de Lesbegue]], podemos considerar
$$
a=t_{0}<t_{1}\dots<t_{n} =b \quad 0 = s_{0}<s_{1}\dots<s_{n} =1,
$$
$g_{jk}:V_{jk}\to \mathbb{C}$ primitivas de $f$ tales que $h(R_{jk})\subset V_{jk}$. Los $(t_{j},s_{k})$ vienen del cubrimiento $h^{-1}(V_{(t,s)})$, con eso llamamos $V_{jk}$ al $V_{(t,s)}$ que contiene al cuadrado, y $g_{jk}$ a la primitiva de $f$ en ese lugar. Ahora nos queda definir bien a $F$ para que quede continua fijando con cuidado las constantes. 
Tomamos $g_{00}=\tilde{g}_{00}$ y luego, inductivamente:
$$
g_{(j+1)k}:=\tilde{g}_{(j+1)k}+\tilde{g}_{(j+1)k}(h(t_{j+1},s_{k+1})) + g_{jk}(h(t_{j+1},s_{k+1})),
$$

$$
g_{j(k+1)}:=\tilde{g}_{j(k+1)}+\tilde{g}_{j(k+1)}(h(t_{j+1},s_{k+1})) + g_{jk}(h(t_{j+1},s_{k+1})).
$$
la onda es que si dos primitivas coinciden en un punto de borde entonces coinciden en todo el lado ya que $h(L)$ con $L$ el lado es conexo
#todo 