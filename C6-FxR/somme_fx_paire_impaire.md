---
anki_linked: 0
raisonnements:
  - analyse_synthese
outils:
kh_n:
  - "1"
display_title: Somme fonctions paires et impaires
---
# Somme fonctions paires et impaires

> [!objectif]
> Toute fonction de $\mathbb{R}$ dans $\mathbb{R}$ peut s'écrire comme la somme du fonction paire et d'une fonction impaire.
### Démonstration

Soit $f:\mathbb{R}\to \mathbb{R}$.

***Analyse*** :
Soit $f_{p}$ une fonction paire et $f_{i}$ une fonction impaire telles que $f=f_{i}+f_{p}$
Soit $x \in \mathbb{R}$.
Alors $f(x)=f_{i}(x)+f_{p}(x)$ et $f(-x)=f_{p}(-x)+f_{i}(-x)=f_{p}(x)-f_{i}(x)$
Donc par somme : $f_{p}(x)=\frac{1}{2}(f(x)+f(-x))$
Et par différence : $f_{i}(x)=\frac{1}{2}(f(x)-f(-x))$

***Synthèse*** :
On pose :
$$
\begin{cases}
f_{p}:\begin{cases}
\mathbb{R}\to \mathbb{R} \\
x\mapsto \frac{1}{2}(f(x)+f(-x))
\end{cases} \\
f_{i}:\begin{cases}
\mathbb{R}\to \mathbb{R} \\
x\mapsto \frac{1}{2}(f(x)-f(-x))
\end{cases}
\end{cases}
$$
Soit $x \in \mathbb{R}$.
On calcule : $f_{p}(-x)=\frac{1}{2}(f(-x)+f(x))=f_{p}(x)$
Et : $f_{i}(-x)=\frac{1}{2}(f(-x)-f(x))=-\frac{1}{2}(f(x)-f(-x))=- f_{i}(x)$
Enfin : $f_{p}(x)+f_{i}(x)=f(x)$

***Bilan*** :
On peut écrire $f$ sous la forme d'une somme d'une fonction paire et d'une fonction impaire

#### Remarques


