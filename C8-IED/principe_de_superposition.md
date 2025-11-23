---
anki_linked: 0
raisonnements:
outils:
  - edl
kh_n:
  - "7"
display_title: Principe de superposition
---
# Principe de superposition

> [!objectif]
> Soit $y_{1}$ et $y_{2}$ deux fonctions.
> On suppose :
> * $y_{1}$ solution de l'EDL $(1):y^{(n)}+a_{n-1}(x)y^{(n-1)}+\dots+a_{0}(x)y=b_{1}(x)$
> * $y_{2}$ solution de l'EDL $(2):y^{(n)}+a_{n-1}(x)y^{(n-1)}+\dots+a_{0}(x)y=b_{2}(x)$
>
>Alors pour tout $(\lambda_{1},\lambda_{2})\in \mathbb{R}^{2}$, la fonction $\lambda_{1}y_{1}+\lambda_{2}y_{2}$ est solution de l'EDL :
> $$
> (12): y^{(n)}+a_{n-1}(x)y^{(n-1)}+\dots+a_{0}(x)y=\lambda_{1}b_{1}(x)+\lambda_{2}b_{2}(x)
> $$
### Démonstration

*On suppose les hypothèses vérifiées.*

$y_{1}$ et $y_{2}$ sont $n$-fois dérivables sur $I$, donc $\lambda_{1}y_{1}+\lambda_{2}y_{2}$ est $n$-fois dérivable sur $I$ et :
$$
\begin{align}
\forall x \in I,&\quad(\lambda_{1}y_{1}+\lambda_{2}y_{2})^{(n)}(x)+\dots+a_{0}(x)(\lambda_{1}y_{1}+\lambda_{2}y_{2}) \\
&=\lambda_{1}y_{1}^{(n)}(x)+\lambda_{2}y_{2}^{(n)}(x)+\dots + a_{0}(x)\lambda_{1}y_{1}+a_{0}(x)\lambda_{2}y_{2} \\
&= \lambda_{1} \left( y_{1}^{(n)}+\dots +a_{0}(x)y_{1}(x) \right)+\lambda_{2}\left( y_{2}^{(n)}(x)+\dots+a_{0}(x)y_{2}(x) \right)  \\
&=\lambda_{1}b_{1}(x)+\lambda_{2}b_{2}(x)
\end{align}
$$
Ainsi $\lambda_{1}y_{1}+\lambda_{2}y_{2}$ est bien solution de l'EDL $(12)$.


#### Remarques


