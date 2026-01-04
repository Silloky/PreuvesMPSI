---
anki_linked: 0
raisonnements:
outils:
  - dl
kh_n:
  - "11"
display_title: Somme et produit de DL
---
# Somme et produit de DL

> [!objectif]
> Soit $n\in \mathbb{N}$ et $f$ et $g$ deux fonctions définies au voisinage de $0$.
> On dispose de deux $DL_{n}(0)$ :
> * $f(x)\underset{ 0 }{ = }a_{0}+a_{1}x+a_{2}x^2+\dots+a_{n}x^n+o(x^n)$
> * $g(x)\underset{ 0 }{ = }b_{0}+b_{1}x+b_{2}x^{2}+\dots+b_{n}x^n+o(x^n)$
> 
> Alors :
> * La somme des $DL_{1}(0)$ est un $DL_{1}(0)$ dont la partie régulière est la somme des parties régulières
> * Le produit des $DL_{1}(0)$ est un $DL_{1}(0)$ dont la partie régulière est le produit des parties régulières, tronqué à l'ordre $n$
### Démonstration

##### 1. Somme

$$
\begin{align}
f(x)+g(x)&\underset{ 0 }{ = }(a_{0}+a_{1}x+\dots+o(x^n))+(b_{0}+b_{1}x+\dots+o(x^n)) \\
&\underset{ 0 }{ = } (a_{0}+b_{0})+(a_{1}+b_{1})x+\dots+\underbrace{ o(x^n)+o(x^n) }_{ o(x^n) } \\
f(x)+g(x)&\underset{ 0 }{ = }(a_{0}+b_{0})+(a_{1}+b_{1})x+\dots+o(x^n)
\end{align}
$$
Il s'agit bien d'un $DL_{1}(0)$.

##### 2. Produit

On note $P$ et $Q$ les parties régulières respectives des $DL_{1}(0)$ de $f$ et $g$. Alors :
$$
\begin{align}
f(x)g(x)&\underset{ 0 }{ = }(P(x)+o(x^n))(Q(x)+o(x^n)) \\
&\underset{ 0 }{ = } P(x)Q(x)+P(x)o(x^n)+Q(x)o(x^n)+o(x^n)^2 \\
f(x)g(x)&\underset{ 0 }{ = }P(x)Q(x)+o(x^n)
\end{align}
$$
Puisque les termes d'ordre $\geq n$ sont négligeables, on peut tronquer le polynôme $PQ$ à l'ordre $n$.
Et c'est bien un $DL_{1}(0)$ de $f\times g$.

#### Remarques


