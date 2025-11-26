---
anki_linked: 0
raisonnements:
  - double_implication
outils:
  - suites
  - bornessup
kh_n:
display_title: Caractérisation séquentielle de la borne supérieure
---
# Caractérisation séquentielle de la borne supérieure

> [!objectif]
> Soit $A\in\mathcal{P}(\mathbb{R})$ et $c\in \mathbb{R}$.
> $A$ admet une borne supérieure et $\sup(A)=c$ $\iff$ $c$ est un majorant de $A$ et il existe une suite d'éléments de $A$ qui tend vers $c$
### Démonstration

***Sens $\implies$*** :
On suppose que $A$ admet une borne supérieure notée $c$.
Par définition, $c$ est un majorant de $A$.
Pour tout $n\geq 1,c-\frac{1}{n}\leq c$ donc $c-\frac{1}{n}$ n'est pas un majorant de $A$. Ainsi il existe un élément de $A$ qu'on note $u_{n}$ tel que $u_{n}>c-\frac{1}{n}$.
$(u_{n})_{n\geq 1}$ est une suite d'éléments de $A$ et $\forall n\geq 1, c-\frac{1}{n}<\underbrace{ u_{n}\leq c }_{ \text{car }u_{n}\in A }$.
Enfin, par encadrement, $u_{n}\to c$

***Sens $\impliedby$*** :
Soit $c\in \mathbb{R}$. On suppose que $c$ est un majorant de $A$ et qu'il existe une suite $(u_{n})$ d'élémenrs de $A$ telle que $u_{n}\to c$.
Soit $\varepsilon>0$. $\frac{\varepsilon}{2}>0$ et $u_{n}\to c$, donc il existe $N\in \mathbb{N}$ tel que $\forall n\geq N,|u_{n}-c|\leq \frac{\varepsilon}{2}$.
En particulier, $|u_{N}-c|\leq \frac{\varepsilon}{2}$ donc $\underbrace{ u_{N} }_{ \in A }\geq c- \frac{\varepsilon}{2}>c-\varepsilon$ donc $c-\varepsilon$ n'est pas un majorant.
Ainsi, $c=\sup(A)$


#### Remarques


