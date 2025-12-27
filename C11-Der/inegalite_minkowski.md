---
anki_linked: 0
raisonnements:
outils:
  - sommes
kh_n:
  - "11"
display_title: Inégalité de Minkowski
---
# Inégalité de Minkowski

> [!objectif]
> Soit:
> * $n\in \mathbb{N}^*$
> * $x_{1},\dots,x_{n}$ des réels non tous nuls
> * $y_{1},\dots,y_{n}$ des réels non tous nuls
> * $p>1$ un réel
> 
> Alors :
>$$
> \left(\sum_{i=1}^n |x_{i}+y_{i}|^p \right)^{1/p}\leq \left( \sum_{i=1}^n |x_{i}|^p \right)^{1/p} + \left( \sum_{i=1}^n|y_{i}|^p \right)^{1/p}
> $$
### Démonstration

Pour tout $i\in[\![1,n]\!]$ :
$$
\begin{align}
(|x_{i}+y_{i}|^p)&=|x_{i}+y_{i}||x_{i}+y_{i}|^{p-1} \\
&\leq(|x_{i}|+|y_{i}|)|x_{i}+y_{i}|^{p-1} \\
(|x_{i}+y_{i}|^p)&\leq|x_{i}||x_{i}+y_{i}|^{p-1}+|y_{i}||x_{i}+y_{i}|^{p-1}
\end{align}
$$
Donc en sommant sur $i$ :
$$
\sum_{i=1}^n|x_{i}+y_{i}|^p\leq \sum_{i=1}^n|x_{i}||x_{i}+y_{i}|^{p-1}+\sum_{i=1}^n|y_{i}||x_{i}+y_{i}|^{p-1}
$$
Les $(x_{i})$, $(y_{i})$ et $(x_{i}+y_{i})$ sont des réels non tous nuls, et $p>1$, donc $p-1>0$.
On pose $q=\frac{p}{p-1}$. On a bien $\frac{1}{p}+\frac{1}{q}=1$.
Donc d'après l'[[inegalite_holder|inégalité de Hölder]] appliquée à la première inégalité :
$$
\begin{align}
\sum_{i=1}^n|x_{i}||x_{i}+y_{i}|^{p-1}&\leq \left( \sum_{i=1}^n|x_{i}|^p \right)^{1/p}\left( \sum_{i=1}^n\left(|x_{i}+y_{i}|^{p-1}\right)^q \right)^{1/q} \\
&=\left( \sum_{i=1}^n|x_{i}|^p \right)^{1/p}\left( \sum_{i=1}^n|x_{i}+y_{i}|^p \right)^{1/q}  
\end{align}
$$
De même, pour la deuxième, on obtient $\left( \sum_{i=1}^n|y_{i}|^p \right)^{1/p}\left( \sum_{i=1}^n|x_{i}+y_{i}|^p \right)^{1/q}$
Donc :
$$
\left( \sum_{i=1}^n|x_{i}+y_{i}|^p \right)^1\leq \left( \sum_{i=1}^n|x_{i}+y_{i}|^p \right)^{1/q}\left[ \left( \sum_{i=1}^n|x_{i}|^p \right)^{1/p} + \left( \sum_{i=1}^n|y_{i}|^p \right) ^{1/p}  \right] 
$$
Or $1-\frac{1}{q}=1- \frac{p-1}{p}=\frac{1}{p}$.

D'où l'inégalité de Minkowski :
$$
\left( \sum_{i=1}^n|x_{i}+y_{i}|^p \right) ^{1/p}\leq \left( \sum_{i=1}^n|x_{i}|^p \right) ^{1/p}+\left( \sum_{i=1}^n |y_{i}|^p\right)^{1/p} 
$$

#### Remarques


