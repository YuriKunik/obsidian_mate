#complejo 
## Definición

Sean $f:U\to \mathbb{C}$, $h:[a,b]\times[0,1]\to \mathbb{C}$ funciones continuas. Decimos que $F:[a,b]\times[0,1]\to \mathbb{C}$ es una **primitiva según $f$ a lo largo de $h$** si, para todo $(s_{0},t_{0}) \in [a,b]\times[0,1]$, existen $J_{(s_{0},t_{0})}$ y $V_{(s_{0},t_{0})}$ entornos de $(s_{0}, t_{0})$, $h(t_{0},s_{0})$ correspondientemente, tales que

1. $h(J_{s_{0},t_{0}}) \subset V_{(s_{0},t_{0})}$,
2. existe $g:V\to \mathbb{C}$ primitiva de $f$ tal que $F(s,t)=g(h(s,t))$ para todo $(s,t)\in J$.

## Idea

La idea de este resultado es definir algo análogo a [[Primitivas a lo largo de curvas]] pero para [[Homotopía entre curvas complejas]].