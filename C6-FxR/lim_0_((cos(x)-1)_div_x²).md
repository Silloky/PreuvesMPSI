---
anki_linked: 1
raisonnements:
outils:
  - trigo
kh_n:
  - "4"
display_title: lim_(x->0)( (cos(x)-1)/x^2 )
---
# Calculer $\lim_{ x \to 0 }\frac{\cos(x)-1}{x^{2}}$

> [!objectif]
>$$
> \lim_{ x \to 0 } \frac{\cos x -1}{x^{2}}=-\frac{1}{2}
> $$
### Démonstration

On sait que $\lim_{ x \to 0 }\frac{\sin x}{x}=1$, donc en particulier : $$\lim_{ x \to 0 } \frac{\sin\left( \frac{x}{2} \right)}{\frac{x}{2}}=1$$
Et donc : $$\lim_{ x \to 0 } \frac{\sin^{2}\left( \frac{x}{2} \right)}{\frac{x^{2}}{4}}=1$$
Or pour tout $x \in \mathbb{R}$, $\cos(2x)=1-2\sin ^{2}(x)$, donc $\sin ^{2}(x)=\frac{1-\cos(2x)}{2}$ et donc $\sin ^{2}\left( \frac{x}{2} \right)=\frac{1-\cos\left( x \right)}{2}$.
Donc en remplaçant :
$$
\lim_{ x \to 0 } \frac{\frac{1-\cos(x)}{2}}{\frac{x^{2}}{4}}=1\quad\text{donc}\quad \lim_{ x \to 0 } \frac{1-\cos(x)}{x^{2}}=\frac{1}{2} 
$$
Et enfin :
$$
\lim_{ x \to 0 } \frac{\cos x -1}{x^{2}}=-\frac{1}{2}
$$

#### Remarques


