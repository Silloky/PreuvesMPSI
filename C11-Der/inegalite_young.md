---
anki_linked: 0
raisonnements:
outils:
  - derivation
kh_n:
  - "11"
display_title: Inégalité de Young
---
# Inégalité de Young

> [!objectif]
>Soient $p>0$ et $q>0$ des réels tels que $\frac{1}{p}+\frac{1}{q}=1$.
>Alors :
>$$
> \forall(x,y)\in \mathbb{R}^{2}, |xy|\leq \frac{|x|^p}{p}+ \frac{|y|^q}{q}
> $$
### Démonstration

Soient $x$ et $y$ deux réels.
On suppose que $x\neq 0$ et $y\neq 0$, car sinon c'est évident. Donc $(|x|^p,|y|^q)\in(\mathbb{R}^*_{+})^{2}$.
Or $\ln$ est concave sur $\mathbb{R}_{+}^*$, donc puisque $\frac{1}{p}+\frac{1}{q}=1$ :
$$\ln \left( \frac{1}{p}|x|^p + \frac{1}{q}|y|^q \right)\geq \frac{1}{p}\ln(|x|^p)+ \frac{1}{q}\ln(|y|^q)=\ln(|x|)+\ln(|y|)=\ln(|xy|) $$
La fonction $\exp$ est croissante sur $\mathbb{R}$, donc :
$$
\forall(x,y)\in \mathbb{R}^{2},|xy|\leq \frac{|x|^p}{p}+\frac{|y|^q}{q}
$$

#### Remarques


