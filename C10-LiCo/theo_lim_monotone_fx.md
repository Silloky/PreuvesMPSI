---
anki_linked: 0
raisonnements:
  - disjonction_de_cas
outils:
  - bornessup
  - limites
kh_n:
  - "9"
display_title: Théorème de la limite montone (fonctions)
---
# Théorème de la limite monotone (fonctions)

> [!objectif]
> Soit $\alpha<\beta$ des réels, $I=]\alpha,\beta[$ et $f$ une fonction définie et croissante sur $I$.
> 1. $f$ admet en tout point de $I$ une limite finie à gauche et une limite finie à droite, et :
> $$
> \forall a\in I,\qquad \sup_{\substack{x \in I \\ x<a}}f(x)=\lim_{ x \to a^- } f(x)\leq f(a)\leq \lim_{ x \to a^+ } =\inf_{\substack{x\in I\\x>a}}f(x)
> $$
> 2. $f$ admet une limite à droite (pas forcément finie) en $\alpha$ et $\lim_{ x \to \alpha^+ }f(x)=\inf_{x \in I}f(x)$
> 3. $f$ admet une limite à gauche (pas forcément finie) en $\beta$ et $\lim_{ w \to \beta^- }=\sup_{x \in I}f(x)$
### Démonstration

##### 1. Inégalité en tout point de $I$

Soit $a \in I$.

$f(a-1)\in f(]-\alpha,a[)$ donc $f(]-\alpha,a[)$ est non-vide.
Soit $y \in f(]-\alpha,a[)$. Il existe $x \in]\alpha,a[$ tel que $f(x)=y$.
$f$ est supposée croissante, donc puisque $x<a$, on a $y=f(x)\leq f(a)$, ainsi $f(]\alpha,a[)$ est majoré par $f(a)$.
Donc $f(]\alpha,a[)$ est non-vide et majoré, donc il admet une borne supérieure qu'on note $c=\sup_{x<a}f(x)$.

Soit $\varepsilon>0$.
$c-\varepsilon<\varepsilon$, donc $c-\varepsilon$ n'est pas un majorant de $f(]\alpha,a[)$.
Donc il existe $x_{0}\in]\alpha,a[$ tel que $f(x_{0})>c-\varepsilon$.
On pose $\eta=a-x_{0}>0$ car $x_{0}<a$.

Soit $x \in]\alpha,a[$ tel que $|x-a|\leq \eta$.
Donc $-\eta\leq x-a\leq \eta$, donc $a-\eta\leq x<a$ car $x \in]\alpha,a[$.
Donc $a-(a-x_{0})\leq x<a$, et donc $x_{0}\leq x<a$.
Puisque $f$ est croissante, $f(x_{0})\leq f(x)$.
Ainsi $c-\varepsilon<f(x_{0})\leq f(x)\leq c<c+\varepsilon$, et donc $|f(x)-c|\leq \varepsilon$.
Et donc $f(x)\xrightarrow[x\to a^-]{}c=\sup_{x<a}f(x)\leq f(a)$ car $f(a)$ est un majorant.

De même, $f(x)\xrightarrow[x\to a^+]{}\inf_{x>a}f(x)\geq f(a)$  car $f(a)$ est un minorant.

D'où : $\forall a\in I, \sup_{\substack{x \in I \\ x<a}}f(x)=\lim_{ x \to a^- } f(x)\leq f(a)\leq \lim_{ x \to a^+ } =\inf_{\substack{x\in I\\x>a}}f(x)$
##### 2. Limite en $\alpha^+$

On pose $m=\inf_{x \in I}f(x)\in \overline{\mathbb{R}}$.

Si $m=-\infty$ :
Soit $M \in \mathbb{R}$. $M>-\infty$ donc $M$ n'est pas un minorant, donc il existe $x_{0}\in I$ tel que $f(x_{0})<M$.
On pose $\eta=x_{0}-\alpha>0$ car $x_{0}\in I$ donc $x_{0}>\alpha$
Pour tout $x \in I$ tel que $|x-\alpha|\leq \eta$, on a $x\leq x_{0}$ donc par croissance de $f$, $f(x)\leq f(x_{0})<M$.
Ainsi $\lim_{ x \to \alpha^+ }f(x)=-\infty=m$.

Si $m>-\infty$, alors $m\in \mathbb{R}$
Soit $\varepsilon>0$. 
$m+\varepsilon>m$ donc $m+\varepsilon$ n'est pas un minorant, donc il existe $x_{0}\in I$ tel que $f(x_{0})<m+\varepsilon$.
On pose $\eta=x_{0}-\alpha>0$ car $x_{0}\in I$ donc $x_{0}>\alpha$.
Pour tout $x \in I$ tel que $|x-\alpha|\leq \eta$, on a $x\leq x_{0}$ donc par croissance de $f$, $m\leq f(x)\leq f(x_{0})<m+\varepsilon$, donc $0\leq f(x)-m\leq \varepsilon$, donc $|f(x)-m|\leq\varepsilon$.
Donc $\lim_{ x \to \alpha^+ }f(x)=m$

Donc dans tous les cas, $\lim_{ x \to \alpha^+ }f(x)=\inf_{x \in I}f(x)$
##### 3. Limite en $\beta^-$

Démonstration quasi-identique à la limite de $\alpha^+$.

#### Remarques


