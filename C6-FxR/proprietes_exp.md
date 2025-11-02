---
anki_linked: 0
raisonnements:
outils:
  - bijection
  - integration
  - limites
kh_n:
  - "4"
display_title: Propriétés de exp
---
# Propriétés de la fonction $\exp$

> [!objectif]
> Soit $\exp$ la bijection réciproque de $\ln$
> 1. $\exp$ est définie et dérivable (donc continue) sur $\mathbb{R}$ et $\forall x \in \mathbb{R}, \exp'(x)=\exp(x)$
> 2. $\exp$ est strictement croissante sur $\mathbb{R}$
> 3. $\exp(0)=1$
> 4. $\forall x \in \mathbb{R}, \exp(x)\geq x+1$
> 5. $\forall (a,b)\in \mathbb{R}^{2},\exp(a+b)=\exp(a)\times \exp(b)$
> 6. $\lim_{ x \to +\infty }\exp(x)=+\infty$
> 7. $\lim_{ x \to -\infty }\exp(x)=0^+$
> 8. $\exp(1)=e$
> 9. $\lim_{ \substack{x\to 0 \\ x\neq 0} } \frac{\exp(x)-1}{x}=1$
### Démonstration

##### 1. Définition et dérivabilité

$\exp$ est la bijection réciproque de $\ln:\mathbb{R}_{+}^+ \to \mathbb{R}$, donc par définition d'une bijection réciproque, $\exp$ est définie sur $\mathbb{R}$.
On sait que $\ln$ est dérivable sur $\mathbb{R}_{+}^*$, et que $\forall x \in \mathbb{R}_{+}^*,\ln'(x)=\frac{1}{x}\neq 0$, donc sa dérivée ne s'annule pas.
Ainsi, d'après le [[theo_derivabilite_bijection_reciproque|théorème de la dérivabilité de la bijection réciproque]], $\exp$ est dérivable sur $\mathbb{R}$ et $\forall x \in \mathbb{R}, \exp'(x)=\frac{1}{(\ln'\circ \exp)(x)}=\frac{1}{\frac{1}{\exp(x)}}=\exp(x)$
##### 2. Stricte croissance

$\exp$ est la bijection réciproque de $\ln$, donc d'après le [[monotonie_bijection_reciproque|théorème de la bijection monotone]], $\exp$ est monotone et du même sens de variation que $\ln$.
Or $\ln$ est strictement croissante sur $\mathbb{R}_{+}^*$, donc $\exp$ est strictement croissante sur $\mathbb{R}$.
##### 3. $\exp(0)=1$

On note $\exp(0)=e_{0}$. Donc $\ln(\exp(0))=\ln(e_{0})$, donc $\ln(e_{0})=0$ (par définition de la bijection réciproque).
Autrement dit, $\int_{1}^{e_{0}} \frac{1}{x} \, \mathrm{d}x=0$
Or $x\mapsto \frac{1}{x}$ est est continue et ne s'annule pas $\mathbb{R}_{+}^*$, donc la seule possibilité est que $e_{0}=1$ afin d'avoir une intégrale nulle.
Donc $e_{0}=1$ et $\exp(0)=1$
##### 4. $\forall x \in \mathbb{R}, \exp(x)\geq x+1$

On sait que $\forall x \in \mathbb{R}_{+}^*,\ln(x)\leq x-1$.
De plus, soit $x \in \mathbb{R}$. $\exp(x)\in \mathbb{R}_{+}^*$, donc $\ln(\exp(x))\leq \exp(x)+1$, donc $x\leq \exp(x)+1$.
Enfin, $\exp(x)\geq x-1$
##### 5. $\forall (a,b)\in \mathbb{R}^{2},\exp(a+b)=\exp(a)\times \exp(b)$

Soit $(a,b)\in \mathbb{R}^2$.
$\exp(a)>0$ et $\exp(b)>0$, donc $\exp(a)\times \exp(b)>0$.
Donc $\ln(\exp(a)\times \exp(b))=\ln(\exp(a))+\ln(\exp(b))=a+b$
Or $\ln(\exp(a+b))=a+b$, et on sait que $\ln$ est injective.
Donc $\exp(a+b)=\exp(a)\times \exp(b)$
##### 6. $\lim_{ x \to +\infty }\exp(x)=+\infty$

Soit $x \in \mathbb{R}$.
On pose $y=\exp(x)$. Donc $x=\ln(y)$.
On suppose que $x\to +\infty$. Donc $\ln(y)\to +\infty$.
Or on sait que $\lim_{ y \to +\infty }\ln(y)=+\infty$.
Puisque $\ln$ est strictement croissante sur tout son ensemble de définition, on déduit que cette limite de $+\infty$ n'est atteinte qu'une seule fois.
Ainsi, $\exp(x)=y\to +\infty$
Donc $\lim_{ x \to +\infty }\exp(x)=+\infty$
##### 7. $\lim_{ x \to -\infty }\exp(x)=0^+$

Soit $x \in \mathbb{R}$.
On pose $y=\exp(x)$, donc $x=\ln(y)$.
On suppose que $x\to -\infty$, donc $\ln(y)\to -\infty$.
Or on sait que $\lim_{ y \to 0^+ }\ln(y)=-\infty$
Puisque $\ln$ est strictement croissante sur tout son ensemble de définition, on déduit que cette limite de $-\infty$ n'est atteinte qu'une seule fois.
Donc $\exp(x)=y\to 0^+$
Donc $\lim_{ x \to -\infty }\exp(x)=0^+$
##### 8. $\exp(1)=e$

Soit $x\in \mathbb{R}$ tel que $\exp(x)=e$.
Donc $x=\ln(e)$, or on sait que $\ln(e)=1$, donc $x=1$.
Donc $\exp(1)=e$
##### 9. $\lim_{ \substack{x\to 0 \\ x\neq 0} } \frac{\exp(x)-1}{x}=1$

On sait $\exp'(0)=\lim_{ \substack{x\to 0 \\ x\neq 0} } \frac{\exp(x)-\exp(0)}{x-0}=\lim_{ \substack{x\to 0 \\ x\neq 0} } \frac{\exp(x)-1}{x}$
Or $\exp'(x)=\exp(0)=1$
Donc $\lim_{ \substack{x\to 0 \\ x\neq 0} } \frac{\exp(x)-1}{x}=1$

#### Remarques


