#construcciones #topoalg #matemática 
## Construcción

Dado un [[Delta Complejos|Delta Complejo]] $X$ con ${\sigma^n_\alpha}$ sus morfismos. Tenemos grupos abelianos libres $\Delta_n(X)$ con generadores los [[n Simplices|n-simplices]] $\varphi^n_\alpha$.  Estos grupos vienen con morfismos $\partial_n : \Delta_{n+1} \rightarrow \Delta_n$   definidos como:
$$
\partial_n([v_0, ...,v_n]) = \sum (-1)^i \sigma_\alpha([v_0, ..., \hat{v_i}, ..., v_n)])
$$
Cada uno va a ser llamado **morfismo de borde**. 

Con esto se puede probar que $\partial_{n} \circ \partial_{n+1} = 0$, por lo que $Im(\partial_{n+1}) \subset Ker(\partial_n)$. Así conseguimos una [[Cadena de Complejos]] 
```tikz
\usepackage{amsfonts}
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	 \dots & C_{n+1} & C_n \dots & \dots C_1 & C_0 & 0
	\arrow["\partial_{n+1}", from=1-1, to=1-2]
	\arrow["\partial_{n}", from=1-2, to=1-3]
	\arrow["\partial_{0}", from=1-4, to=1-5]
	\arrow["", from=1-5, to=1-6]
\end{tikzcd}
\end{document}
```
con $C_{n}= \Delta_{n}(X)$.

Finalmente, el n-ésimo grupo de homología simplicial lo podemos definir como $H_n^{\Delta} = ker(\partial_n)/Im(\partial_{n+1})$.
