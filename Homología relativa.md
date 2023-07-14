#matemática #construcciones #topoalg 
## Definición
X espacio topológico, definimos $C_{n}(X,A)$ como el grupo cociente $C_{n}(X) / C_{n}(A)$ ($C_{n}$ los grupos que forman la [[Homología Singular]]) . Como el morfismo $\partial: C_{n}(X)\to C_{n-1}(X)$ manda $C_n(A)$ en $C_{n-1}(A)$, induce un morfismo $\partial: C_{n}(X,A) \to C_{n-1}(X,A)$ que nos da una [[Cadena de Complejos]].
Con esto pasamos a la homología de la forma usual, definiendo $H_n(X,A)$ como $ker(\partial) / Im(\partial)$.

## Observaciones
- Elementos de $H_n(X,A)$ son representados por ciclos relativos: n-cadenas $\alpha \in C_{n}(X)$ tal que $\partial \alpha \in C_{n-1}(A)$.
- Un ciclo relativo es trivial en $H_{n}(X,A)$ sii es un borde relativo: $\alpha = \partial \beta + \gamma$ 