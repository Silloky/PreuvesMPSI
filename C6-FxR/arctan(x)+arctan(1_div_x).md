---
anki_linked: 0
raisonnements:
  - disjonction_de_cas
outils:
  - trigo
kh_n:
  - "4"
display_title: arctan(x)+arctan(1/x)
---
# Calcul de $\arctan(x)+\arctan\left( \frac{1}{x} \right)$

> [!objectif]
>$$
> \forall x \in \mathbb{R}^*,\arctan(x)+\arctan\left( \frac{1}{x} \right)=\begin{cases}
> \frac{\pi}{2} &\text{si }x>0 \\
> -\frac{\pi}{2} &\text{si }x<0
> \end{cases}
> $$
### Démonstration

Soit $x \in \mathbb{R}^*$.
On pose $a=\arctan(x)\in \left[ -\frac{\pi}{2}, \frac{\pi}{2} \right]$ et $b=\arctan\left( \frac{1}{x} \right)\in \left[ -\frac{\pi}{2}, \frac{\pi}{2} \right]$

On calcule $\tan(a+b)$ :
$$
\tan(a+b)=\frac{x+\frac{1}{x}}{1-x \times \frac{1}{x}}=\frac{x+\frac{1}{x}}{1-1}
$$
Or le dénominateur est nul, donc $\tan(a+b)$ n'est pas défini, donc $a+b \equiv \frac{\pi}{2}\pmod \pi$
Et $a+b \in[-\pi,\pi]$, donc $\arctan(x)+\arctan\left( \frac{1}{x} \right) \in \left\{ -\frac{\pi}{2}, \frac{\pi}{2} \right\}$.

***Si $x>0$*** :
$\arctan(x)\in\left[ 0, \frac{\pi}{2} \right]$ et $\arctan\left( \frac{1}{x} \right)\in \left[ 0, \frac{\pi}{2} \right]$
Donc $\arctan(x)+\arctan\left( \frac{1}{x} \right) \in[0,\pi]$, et puisque $\arctan(x)+\arctan\left( \frac{1}{x} \right) \in \left\{ -\frac{\pi}{2}, \frac{\pi}{2} \right\}$, on en déduit que : $\arctan(x)+\arctan\left( \frac{1}{x} \right)=\frac{\pi}{2}$

***Si $x<0$*** :
$\arctan(x)\in\left[ -\frac{\pi}{2}, 0 \right]$ et $\arctan\left( \frac{1}{x} \right)\in \left[ -\frac{\pi}{2}, 0 \right]$
Donc $\arctan(x)+\arctan\left( \frac{1}{x} \right) \in[-\pi,0]$, et puisque $\arctan(x)+\arctan\left( \frac{1}{x} \right) \in \left\{ -\frac{\pi}{2}, \frac{\pi}{2} \right\}$, on en déduit que : $\arctan(x)+\arctan\left( \frac{1}{x} \right)=-\frac{\pi}{2}$

Donc :
$$
\forall x \in \mathbb{R}^*,\arctan(x)+\arctan\left( \frac{1}{x} \right)=
\begin{cases}
\frac{\pi}{2} &\text{si }x>0 \\
-\frac{\pi}{2} &\text{si }x<0
\end{cases}
$$
#### Remarques


