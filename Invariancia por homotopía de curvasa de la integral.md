
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


