---
anki_linked: 0
raisonnements:
  - recurrence
outils:
  - integration
  - derivation
  - limites
  - bijection
kh_n:
  - "4"
display_title: Propriétés de ln
---
# Propriétés de la fonction $\ln$

> [!objectif]
> Soit $\ln$ l'unique primitive de $x\mapsto\frac{1}{x}$ sur $\mathbb{R}_{+}^*$ qui s'annule en $1$.
> 1. $\ln$ est définie et dérivable (donc continue) sur $\mathbb{R}_{+}^*$ et $\forall x>0,\ln'(x)=\frac{1}{x}$
> 2. $\ln$ est strictement croissante sur $\mathbb{R}_{+}^*$
> 3. $\forall x>0,\ln(x)\leq x-1$
> 4. $\forall (a,b)\in (\mathbb{R}_{+}^*)^{2},\ln(ab)=\ln(a)+\ln(b)$
> 5. $\forall (a,b)\in (\mathbb{R}_{+}^*)^{2},\ln\left( \frac{a}{b} \right)=\ln(a)-\ln(b)$
> 6. $\forall a\in \mathbb{R}_{+}^*,\ln\left( \frac{1}{a} \right)=-\ln(a)$
> 7. $\forall a\in \mathbb{R}_{+}^*, \forall n \in \mathbb{N},\ln(a^n)=n\ln(a)$
> 8. $\lim_{ x \to +\infty }\ln(x)=+\infty$
> 9. $\lim_{ x \to -\infty }\ln(x)=-\infty$
> 10. Il existe un unique réel noté $e$ tel que $\ln(e)=1$
> 11. $\lim_{ x \to 0^+ } \frac{\ln(1+x)}{x}=1$
### Démonstration

##### 1. Définition et dérivabilité

D'après le théorème fondamental de l'analyse, puisque $x\mapsto \frac{1}{x}$ est continue sur $\mathbb{R}_{+}^*$, elle y admet des primitives qui y sont continues.
$\ln$ est une primitive de $x\mapsto \frac{1}{x}$, donc elle est continue sur $\mathbb{R}_{+}^*$, et par définition d'une primitive, $\forall x \in \mathbb{R}_{+}^*,\ln'(x)=\frac{1}{x}$.
Donc $\ln$ est bien dérivable (donc continue) sur $\mathbb{R}_{+}^*$.
##### 2. Stricte croissance

Par définition, $\forall x>0, \ln'(x)=\frac{1}{x}>0$.
Donc $\ln$ est strictement croissante sur $\mathbb{R}_{+}^*$
##### 3. $\forall x>0,\ln(x)\leq x-1$

$\forall x>0,f'(x)=\frac{1}{x}$, donc $\forall x>0,f''(x)=-\frac{1}{x^{2}}<0$
Donc $\ln$ est concave sur $\mathbb{R}_{+}^*$, donc elle est inférieure à toutes ses tangentes.
Or la tangente à $\ln$ au point d'abscisse $1$ vaut : $y=f'(1)(x-1)+f(1)=\frac{1}{1}(x-1)+0=x-1$
Donc $\forall x>0, \ln(x)\leq x-1$
##### 4. $\forall (a,b)\in (\mathbb{R}_{+}^*)^{2},\ln(ab)=\ln(a)+\ln(b)$

Soit $a\in \mathbb{R}_{+}^*$.
On considère $f:\begin{cases}\mathbb{R}_{+}^*\to \mathbb{R} \\ x\mapsto \ln(ax)-\ln(x)\end{cases}$
$f$ est dérivable sur $\mathbb{R}_{+}^*$ et $\forall x \in \mathbb{R}_{+}^*, f'(x)=\frac{a}{ax}-\frac{1}{x}=0$
Or $\mathbb{R}_{+}^*$ est un intervalle, donc $f$ est y constante.
Et $f(1)=\ln(a)-0$.
Ainsi, $\forall x \in \mathbb{R}_{+}^*, \ln(ax)-\ln(x)=\ln(a)$, donc $\forall b\in \mathbb{R}_{+}^*,\ln(ab)=\ln(a)+\ln(b)$
##### 5. $\forall (a,b)\in (\mathbb{R}_{+}^*)^{2},\ln\left( \frac{a}{b} \right)=\ln(a)-\ln(b)$

Soit $(a,b)\in (\mathbb{R}_{+}^*)^{2}$.
Or $\ln(a)=\ln\left( b \times \frac{a}{b} \right)=\ln(b)+\ln\left( \frac{a}{b} \right)$.
Donc $\ln\left( \frac{a}{b} \right)=\ln(a)-\ln(b)$
##### 6. $\forall a\in \mathbb{R}_{+}^*,\ln\left( \frac{1}{a} \right)=-\ln(a)$

C'est un cas particulier de la propriété précédente.
Soit $a \in \mathbb{R}_{+}^*$.
$\ln\left( \frac{1}{a} \right)=\ln(1)-\ln(a)=-\ln(a)$
##### 7. $\forall a\in \mathbb{R}_{+}^*, \forall n \in \mathbb{N},\ln(a^n)=n\ln(a)$

*Par récurrence évidente* :
Pour tout $n\in \mathbb{N}$, on pose $H_{n}:\forall a\in \mathbb{R}_{+}^*, \ln(a^n)=n\ln(a)$
***Initialisation*** :
En $0$ : $\ln(a^0)=\ln(1)=0$ et $0\ln(a)=0$
Donc $H_{0}$ est vraie et $H_{n}$ est initialisée en $0$.
***Hérédité*** :
Soit $n\in \mathbb{N}$. On suppose $H_{n}$.
$\ln(a^{n+1})=\ln(a^n\times a)=\ln(a^n)+ \ln(a)=n\ln(a)+\ln(a)=(n+1)\ln(a)$
Donc $H_{n+1}$ est vraie et $H_{n}$ est héréditaire.
##### 8. $\lim_{ x \to +\infty }\ln(x)=+\infty$

Soit $M\in \mathbb{R}$.
On a $2>1$, donc puisque $\ln$ est strictement croissante sur $\mathbb{R}_{+}$, $\ln(2)>\ln(1)=0$. Donc $\ln(2)$ est positif.
D'après le caractère archimédien des réels, il existe $n\in \mathbb{N}$ tel que $n\ln(2)\geq M$
On pose $A=2^n$.
Soit $x\geq A$. Donc $\ln(x)\geq \ln(2^n)=n\ln(2)\geq M$.
Donc $x\geq M$.
Ainsi, on a bien : $\forall M\in \mathbb{R},\exists A\in \mathbb{R}_{+}^*,\forall x \geq A,f(x)\geq M$, qui est la définition d'une limite en $+\infty$ en $+\infty$.
Donc $\lim_{ x \to +\infty }\ln(x)=+\infty$.

##### 9. $\lim_{ x \to 0^+ }\ln(x)=-\infty$

On sait que $\frac{1}{x}\xrightarrow[x\to 0^+]{}+\infty$ et que $\ln(x)\xrightarrow[x\to +\infty]{}+\infty$
Donc par composition $\ln\left( \frac{1}{x} \right)\xrightarrow[x\to 0^+]{}+\infty$
Or $\ln\left( \frac{1}{x} \right)=-\ln(x)$
Donc on a $-\ln(x)\xrightarrow[x\to 0^+]{}+\infty$.
Ainsi, $\lim_{ x \to 0^+ }$
$$
\forall a\in \mathbb{R}_{+}^*, \forall n \in \mathbb{N},\ln(a^n)=n\ln(a)
$$
##### 10. Il existe un unique réel noté $e$ tel que $\ln(e)=1$

On sait que $\ln$ réalise une bijection de $\mathbb{R}_{+}^*$ dans $\mathbb{R}$ donc, puisque $1\in \mathbb{R}$, on peut affirmer que $1$ admet un unique antécédent dans $\mathbb{R}_{+}^*$, que l'on peut noter $e$.

##### 11. $\lim_{ x \to 0^+ } \frac{\ln(1+x)}{x}=1$

On sait que $\ln$ est dérivable sur $\mathbb{R}_{+}^*$, donc en particulier :
$\ln'(1)=\lim_{ x \to 1 } \frac{\ln(x)-\ln(1)}{x-1}=\lim_{ x \to 1 } \frac{\ln(x)}{x-1}$
Or $\ln'(1)=\frac{1}{1}=1$, donc $\lim_{ x \to 1 } \frac{\ln(x)}{x-1}=1$
De plus, $\lim_{ x \to 0^+ }(1+x)=1$, donc par composition, on obtient que $\lim_{ x \to 0^+ } \frac{\ln(1+x)}{x}=1$


#### Remarques


