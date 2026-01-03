---
anki_linked: 0
raisonnements:
outils:
  - dl
kh_n:
  - "11"
display_title: Développement limité de tan à l'ordre 5
---
# Développement limité de $\tan$ à l'ordre $5$

> [!objectif]
> Le développement limité de $\tan$ à l'ordre $5$ en $0$ est:
> $$
 \tan \underset{ 0 }{ = } x+ \frac{x^{3}}{3} + \frac{2x^5}{5}+o(x^5)
> $$
### Démonstration

D'après la formule de Taylor, on a les DL suivants (à l'ordre $5$) :
* $\sin x\underset{ 0 }{ = } x- \frac{x^{3}}{6}+\frac{x^5}{120}+o(x^5)$
* $\cos x \underset{ 0 }{ = } 1- \frac{x^{2}}{2}+ \frac{x^4}{24}+o(x^5)$
Pour tout $x$, on pose $u(x)= -\frac{x^{2}}{2}+\frac{x^4}{24}+o(x^4)$. On remarque que $\cos x \underset{ 0 }{ = }1+u(x)$
Or on sait que $\frac{1}{1+u}\underset{ 0 }{ = }1-u+u^{2}+o(u^{2})$ (DL usuel).
Donc ici :
$$
\begin{align}
\frac{1}{\cos x}&\underset{ 0 }{ = }1-u(x)+u^{2}(x)+o(u^{2}) \\
&\underset{ 0 }{ = } 1 +\frac{x^{2}}{2}- \frac{x^4}{24}+\left( -\frac{x^{2}}{2} \right)^{2}+o(x^4) \\
\frac{1}{\cos x}&\underset{ 0 }{ = } 1+ \frac{x^{2}}{2}+\frac{5x^4}{24}+o(x^4)
\end{align}
$$
On effectue le produit terme à terme avec $\sin x$ :
$$\begin{align}
\tan x &\underset{ 0 }{ = } \frac{1}{\cos x}\times \sin x \\
&\underset{ 0 }{ = }\left( x- \frac{x^{3}}{6}+\frac{x^5}{120} \right)\left( 1+\frac{x^{2}}{2}+\frac{5x^4}{24} \right)+o(x^5) \\
&\underset{ 0 }{ = }x+ \frac{x^{3}}{2}+\frac{5x^5}{24}-\frac{x^{3}}{6}-\frac{x^5}{12}+\frac{x^5}{120}+o(x^5) \\
\tan x&\underset{ 0 }{ = }x+ \frac{x^{3}}{3}+\frac{2x^5}{15}+o(x^5)
\end{align}$$
D'où le résultat.


#### Remarques


