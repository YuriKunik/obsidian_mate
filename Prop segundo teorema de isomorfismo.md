
## Enunciado

Sean $H, K$ [[subgrupo|subgrupos]] de un [[Grupo]] G, si $H$ es un [[Subgrupo Normal]], entonces

1. $HK$ es un subgrupo de $G$ y $H$ es normal en $HK$.
2. $H \cap K$ es normal en K y
$$
\frac{HK}{H} \cong \frac{K}{H\cap K}
$$

## Demostración

Verifiquemos que $HK$ es un subgrupo de $G$ cuando $H$ es normal. La forma canchera de ver esto es observando que
$$
HK = \cup_{k\in K} Hk = \cup_{k\in K} \pi^{-1}(\pi(k)) = \pi^{-1}(\pi(K))
$$

Para la otra parte, tomemos $\varphi: K \to \frac{HK}{H}$ que mande $k \mapsto [k]$, entonces si $k\in H \cap K$ es claro que $\varphi (k)=0$. Por otro lado, si $\varphi(k)=[k]=e$ es porque $k \in H$ y por lo tanto en $H \cap K$. Nos falta ver que es sobre. Dado $[hk] \in \frac{HK}{H}$, $h^{-1}hk = k$ entonces $hk \sim k$ y $\varphi(k)=[k]$ con lo que ya estaríamos.