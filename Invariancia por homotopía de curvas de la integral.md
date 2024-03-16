
## Enunciado

Sea $f:U\to \mathbb{C}$ una [[Función holomorfa]] y sean $\gamma_{0},\gamma_{1}:[a,b]\to \mathbb{C}$ [[curva|curvas]] continuas tales que $\gamma_{0}$ es [[Homotopía entre curvas complejas|homotopica]] $\gamma_{1}$. Entonces

$$
\int_{\gamma_{0}}f(z) \, dz = \int_{\gamma_{1}}f(z) \, dz 
$$

## Demostración

Primero tomamos $F$ una [[Primitiva a lo largo de homotopías]] para $f, h$. Dado $s \in[0,1]$ tenemos que $F_{s}(t)=F(s,t)$ es una [[Primitivas a lo largo de curvas|primitiva]] a lo largo de $h(-,s)=h_{s}(t)$. En particular, resulta
$$
	\int_{h_{s}} f(z) \, dz = F(b,s)-F(a, s)
$$
Para nuestro caso tenemos

$$
	\int_{\gamma_{0}} f(z) \, dz = F(b,0)-F(a, 0)
$$

$$
	\int_{\gamma_{1}} f(z) \, dz = F(b,1)-F(a, 1)
$$

Si la homotopía es con extremos fijos, se cumple, para todo $s$, que $h(a,s)=z_{a}$ y $h(b,s)=z_{b}$. Esto implica que en un entorno cualquier $s_{0}$
$$
F(a,s)=g_{(a,s_{0})}(h(a,s))\equiv g_{(a,s_{0})}(z_{a}).
$$
y
$$
F(b,s)=g_{(b,s_{0})}(h(b,s))\equiv g_{(b,s_{0})}(z_{b}).
$$
En otras palabras, $F$ es localmente constante y por lo tanto constante en la segunda variable. Así
$$
\int_{\gamma_{1}}f(z) \, dz - \int_{\gamma_{0}}f(z) \, dz = F(b,1)-F(b,0) - [F(a,1)-F(a,0)]=0.
$$

En cambio, si $h$ es una homotopía entre [[lazo|lazos]], en un entorno de cualquier $s_{0}$ se verifica que
$$
F(b,s)-F(a,s)= g_{b,s_{0}}(h(b,s))-g_{a,s_{0}}(h(a,s))
$$
Con esto, cerca de $h(a,s_{0})$ las primitivas difieren de una constante por lo que $F(b,-)-F(a,-)$ es constante y, en particular
$$
\int_{\gamma_{0}}f(z) \, dz = F(b,0)-F(a,0)=F(b,1)-F(a,1)= \int_{\gamma_{1}}f(z) \, dz  
$$


## Idea
TODO