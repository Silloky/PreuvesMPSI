---
anki_linked: 1
raisonnements:
outils:
  - sommes
  - telescopage
kh_n:
  - "1"
display_title: Formule de Bernoulli
---
# Formule de Bernoulli

> [!objectif]
> Soit $a$ et $b$ des réels et $n$ un entier.
>$$
> a^n-b^n=(a-b)\sum_{k=0}^{n-1}a^{k}b^{n-1-k}
> $$
### Démonstration

$$
\begin{align}
(a-b)\sum_{k=0}^{n-1}a^kb^{n-1-k}&=\sum_{k=0}^{n-1}\left(a^{k+1}b^{n-1-k}-a^kb^{n-k}\right) \\
&=\sum_{k=0}^{n-1}a^{k+1}b^{n-1-k}-\sum_{k=0}^{n-1}a^kb^{n-k} \\
&=\sum_{k=1}^{n}a^{k}b^{n-k}-\sum_{k=0}^{n-1}a^kb^{n-k}  \\
&=a^nb^0+\sum_{k=1}^{n-1}a^{k}b^{n-k}-a^0b^n-\sum_{k=1}^{n-1}a^{k}b^{n-k}  \\
(a-b)\sum_{k=0}^{n-1}a^kb^{n-1-k}&=a^n-b^n
\end{align}
$$
#### Remarques

* On pourrait raccourcir beaucoup en utilisant une somme téléscopique à la première ligne.
