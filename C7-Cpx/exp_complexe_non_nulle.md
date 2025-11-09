---
anki_linked: 1
raisonnements:
outils:
  - module
kh_n:
display_title: Exponentielle complexe non nulle
---
# Exponentielle complexe non nulle

> [!objectif]
>$$
> \forall z\in \mathbb{C},e^z\neq 0
> $$
### Démonstration

Soit $z\in \mathbb{C}$.
$$
\begin{align}
|e^z|&=\left| e^{\mathrm{Re}(z)}\times e^{i\mathrm{Im}(z)} \right| \\
&=\left| e^{\mathrm{Re}(z)} \right| \times \left| e^{i\mathrm{Im}(z)} \right|  \\
|e^z|&=e^{\mathrm{Re}(z)}\times 1
\end{align}
$$
Or $\mathrm{Re}(z)\in \mathbb{R}$, donc $e^{\mathrm{Re}(z)}>0$ (c'est l'exponentielle réelle).
Donc $|e^z|>0$, donc $e^z\neq 0$

#### Remarques


