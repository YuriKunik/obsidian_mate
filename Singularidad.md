
## Definición

Sean $U \subset \mathbb{C}$ un abierto y $z_{0} \in U$. Dada $f :U- \{ z_{0} \}\to \mathbb{C}$ holomorfa, se dice que $z_{0}$ es una **singularidad aislada** de $f$. Si existe $k \in \mathbb{N}_{0}$ mínimo tal que 
$$
\lim_{ z \to z_{0} } (z-z_{0})^{k+1} f(z)=0
$$
decimos que $z_{0}$ es 
1. Una **singularidad evitable**, si $k =0$,
2. Un **polo de orden** $k$, si k>0.

En el caso contrario, se dice que $z_{0}$ es una **singularidad esencial** de $f$.


## Idea

Cuanto mayor es el $k$ más fácil es la convergencia de la función. La onda es que si tenemos un polo de orden $k$, entonces $(z-z_{0})^{k}f(z)$ es holomorfa en $U$ por [[Teorema de Cauchy segunda versión#Un relajamiento de la versión anterior]]. Con esto, el $k$ nos dice cuanto le falta a la función $f$ para ser holomorfa. Si $k=0$, justamente no le faltaba nada y por lo tanto decimos que es evitable.