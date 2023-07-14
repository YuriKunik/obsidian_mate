```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A && B\\
& ADJ &\\
X && B \cup_f X\\
\arrow["f", from=1-1, to=1-3]
\arrow["\bar{f}", from=3-1, to=3-3]
\arrow["i", from=1-1, to=3-1]
\arrow["\bar{i}", from=1-3, to=3-3]
\end{tikzcd}
\end{document}
```
