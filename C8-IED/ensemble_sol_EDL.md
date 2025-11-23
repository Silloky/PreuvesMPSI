---
anki_linked: 0
raisonnements:
outils:
  - edl
kh_n:
  - "6"
  - "7"
display_title: Structure de l'ensemble de solutions d'une EDL
---
# Structure de l'ensemble de solutions d'une EDL

> [!objectif]
> On note :
> * $(E)$ l'EDL : $y^{(n)}+a_{n-1}(x)y^{n-1}+\dots+a_{0}(x)y=b(x)$
> * $(E_{H})$ sont EDLHA
> * $S$ les solutions de $(E)$
> * $S_{H}$ les solutions de $(E_{H})$
> * $y_{p}$ une solution de $(E)$
>  
>  Alors :
>$$
> S=\{ y_{p}+y_{0}\mid y_{0} \in S_{H} \}
> $$
### Démonstration

On pose $S'=\{ y_{p}+y_{0} \mid y_{0}\in S_{H} \}$. Montrons que $S=S'$.

***Sens $\subset$*** :
Soit $y\in S$.
On a $y=y+y_{p}-y_{p}=y_{p}+(y-y_{p})$
Or $y$ et $y_{p}$ sont solutions de $(E)$, donc d'après le principe de superposition, $y-y_{p}$ est solution de $(E_{H})$, et donc $y-y_{p}\in S_{H}$
Donc $y\in S'$.

***Sens $\supset$*** :
Soit $y\in S'$. Il existe $y_{0}\in S_{H}$ tel que $y=y_{p}+y_{0}$.
Or $y_{p}$ est solution de $(E)$ et $y_{0}$ est solution de $(E_{H})$ donc d'après le principe de superposition, $y$ est solution de $(E)$.
Donc $y\in S$

#### Remarques


