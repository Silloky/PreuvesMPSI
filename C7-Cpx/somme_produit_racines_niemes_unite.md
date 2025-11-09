---
anki_linked: 0
raisonnements:
outils:
  - sommes
  - produits
kh_n:
  - "5"
display_title: Somme et produit des racines n-ièmes de l'unité
---
# Somme et produit des racines $n$-ièmes de l'unité

> [!objectif]
> Soit $n\geq 2$
>1. $\sum_{\omega \in \mathbb{U}_{n}}\omega=0$
>2. $\prod_{\omega \in \mathbb{U}_{n}}\omega=(-1)^{n+1}$
### Démonstration

##### 1. Somme
Soit $n\geq 2$.
$$
\sum_{\omega \in \mathbb{U}_{n}}\omega=\sum_{k=0}^{n-1}e^{i \frac{2k\pi}{n}}=\sum_{k=0}^{n-1}\left( e^{i \frac{2\pi}{n}} \right)^k=\frac{1-e^{i \frac{2n\pi}{n}}}{1-e^{i \frac{2\pi}{n}}}=0 
$$
##### 2. Produit
Soit $n\geq 2$.
$$
\prod_{\omega \in \mathbb{U}_{n}}\omega=\prod_{k=0}^{n-1}\left( e^{i \frac{2\pi}{n}} \right)^k=\left(e^{i \frac{2\pi}{n}}  \right)^{\sum_{k=0}^{n-1}k}=\left( e^{i \frac{2\pi}{n}} \right)^{\frac{n(n-1)}{2}}=e^{i(n-1)\pi}=(e^{i\pi})^{n-1}=(-1)^{n-1}
$$

#### Remarques


