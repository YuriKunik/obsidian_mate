Dado un [[Espacio de Banach]] $E$, un *fibrado vectorial* es una tripla $(X, M, \pi)$ con $\pi :X\to M$ de forma tal que, existe un cubrimiento por abiertos $\{ U_{i} \}_{i \in I}$ que cumple:
1. Para cada $i \in I$ existe un [[difeomorfismo]] $\tau _{i}:\pi^{-1}(U_{i})\to U_{i} \times E$ tal que $\pi = pr_{1}\circ \tau _{i}$ y en particular $\tau_{ip}:=\tau_{i}|_{\pi^{-1}(p)}$ sea un [[isomorfismo]].
2. $\tau_{ip} \circ \tau_{jp}^{-1}$ sea un isomorfismo de espacios de banach
3. Para cada $i, j \in I$, la función $p \mapsto \tau_{ip} \circ \tau_{jp}^{-1} \in \mathcal{B}(E)$ sea diferenciable.