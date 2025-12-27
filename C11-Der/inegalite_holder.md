---
anki_linked: 0
raisonnements:
outils:
  - sommes
kh_n:
  - "11"
display_title: Inégalité de Hölder
---
# Inégalité de Hölder

> [!objectif]
> Soit:
> * $n\in \mathbb{N}^*$
> * $x_{1},\dots,x_{n}$ des réels non tous nuls
> * $y_{1},\dots,y_{n}$ des réels non tous nuls
> * $p>0$ et $q> 0$ des réels tels que $\frac{1}{p}+\frac{1}{q}=1$
> 
> Alors :
>$$
> \sum_{i=1}^n |x_{i}y_{i}|\leq \left( \sum_{i=1}^n|x_{i}|^p \right)^{1/p}\left( \sum_{i=1}^n |y_{i}|^q \right)^{1/q}
> $$
### Démonstration

Soit $a_{1},\dots,a_{n}$ des réels non tous nuls et $b_{1},\dots,b_{n}$ des réels non tous nuls.
On suppose que $\sum |a_{i}|^p=\sum |b_{i}|^q=1$.
Or d'après l'[[inegalite_young|inégalité de Young]], pour tout $i \in[\![1,n]\!]$, $|a_{i}b_{i}|\leq \frac{|a_{i}|^p}{p}+ \frac{|b_{i}|^q}{q}$
Donc :
$$
\sum|a_{i}b_{i}|\leq \frac{1}{p}\sum |a_{i}|^p+\frac{1}{q}\sum|b_{i}|^q=\frac{1}{p}+\frac{1}{q}=1
$$
Ainsi dans l'hypothèse que $\sum |a_{i}|^p=\sum |b_{i}|^q=1$, on a $\sum |a_{i}b_{i}|\leq 1$

On pose $X=\left( \sum |x_{i}|^p\right)^{1/p}$ et $Y=\left( \sum |y_{i}|^q \right)^{1/q}$
Puisque les $(x_{i})$ sont non tous nuls, $X>0$ ; de même, $Y>0$.
Pour tout $i\in[\![1,n]\!]$, on pose $a_{i}=\frac{x_{i}}{X}$ et $b_{i}=\frac{y_{i}}{Y}$. Et alors :
$$
\sum |a_{i}|^p=\sum \frac{|x_{i}|^p}{X^p}=\frac{1}{X^{p}}\sum|x_{i}|^p=\frac{1}{\sum|x_{i}|^p}\times \sum|x_{i}|^p=1
$$
De même, on obtient par le calcul $\sum|b_{i}|^q=1$.
On se retrouve donc dans le cas de l'inégalité précédente, donc $\sum |a_{i}b_{i}|\leq 1$.

Donc $\sum \frac{|x_{i}y_{i}|}{XY}\leq 1$, donc $\sum |x_{i}y_{i}|\leq XY$.

D'où :
$$
\sum_{i=1}^n |x_{i}y_{i}|\leq \left( \sum_{i=1}^n|x_{i}|^p \right)^{1/p}\left( \sum_{i=1}^n |y_{i}|^q \right)^{1/q}
$$

#### Remarques


