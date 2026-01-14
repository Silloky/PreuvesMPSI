---
anki_linked: 0
raisonnements:
outils:
  - dl
kh_n:
  - "12"
display_title: Etude asymptotique de x->sqrt{ x^2+1 }+sqrt{ x^2-1 }
---
# Etude asymptotique de $x\mapsto \sqrt{ x^{2}+1 }+\sqrt{ x^{2}-1 }$

> [!objectif]
> On pose $f:\sqrt{ x^{2}+1 }+\sqrt{ x^{2}-1 }$
> $f$ admet deux asymptotes obliques d'équations $y=2x$ et $y=-2x$, et elle est située sous ses tangentes.
### Démonstration

On pose $g:h\mapsto f\left( \frac{1}{h} \right)$.

On étudie **d'abord en $+\infty$** ; or si $\frac{1}{h}\to +\infty$, alors $h\to 0^+$.
Donc :
$$
\begin{align}
g(h)&=\sqrt{ \frac{1}{h^{2}}+1 }+\sqrt{ \frac{1}{h^{2}}-1 } \\
&=\frac{1}{|h|}\left( \sqrt{ 1+h^{2} }+\sqrt{ 1-h^{2} } \right) \\ \\
&= \frac{1}{h}\left( 1+\frac{h^{2}}{2}-\frac{1}{8}h^{4}-\frac{h^{2}}{2}-\frac{1}{8}h^4 +o(h^4)\right) \\
g(h)&=\frac{2}{h}-\frac{1}{4}h^{3}+o(h^{3}) 
\end{align}
$$
Donc $f(x) \underset{ +\infty }{ = } 2x-\frac{1}{4x^3}+o\left( \frac{1}{x^{3}} \right)=2x+ o(x)$.
Donc $f$ admet en $+\infty$ une asymptote oblique d'équation $y=2x$ et :
$$
f(x)-2x\underset{ +\infty }{ = }-\frac{1}{4x^{3}}+o\left( \frac{1}{x^{3}} \right)\underset{ +\infty }{ \sim } -\frac{1}{4x^{3}}\leq 0
$$
Donc $f$ est au-dessous de son asymptote en $+\infty$

**Puis en $-\infty$.**
$\forall x \in \mathbb{R}, f(-x)=\sqrt{ (-x)^{2}+1 }+\sqrt{ (-x)^{2}-1 }=\sqrt{ x^{2}+1 }+\sqrt{ x^{2}-1 }=f(x)$.
Donc $f$ est impaire, ainsi sa courbe est symétrique par rapport à l'axe des ordonnées.
Donc en $-\infty$, $f$ admet une tangente d'équation $y=-2x$ qui est au-dessus de $f$.

#### Remarques


