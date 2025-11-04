### Nomenclature sémantique

Il y un **dossier** par chapitre, libellé `Cx-` suivi de 3 lettres désignant le nom du chapitre.

Il y a un fichier par preuve, ou groupe de preuves très similaires (toutes les propriétés de $\ln$ sont par exemple dans le même fichier).

Le nom du **fichier** d'une preuve :
* pas d'espaces → remplacer par _
* pas d'accents
* éviter les majuscules, sauf pour les termes mathématiques tels que les ensembles $\mathbb{R}$, $\mathbb{C}$, etc...
* rentrer les maths en mode texte, mais il y a des restrictions sur les caractères présents dans les nom de fichiers (imposés non pas par moi mais par le système de fichiers/d'exploitation). *Voir les remplacements courants ci-dessous*

La propriété **`display_title`** d'une preuve :
* Aucune restriction sur le texte
* rentrer les maths en texte, remplacements précédents non nécessaires (utilisez les notations standard comme / pour la division, ^ pour l'exponentiation, etc...)

Le **titre** affiché en gros dans le document :
* Ecriture libre
* Peut comporter des maths en $\LaTeX$

Le ***commit message*** rentré lors de la publication des modifications :
* commence par un préfixe (*voir annexe ci-dessous*), suivi (sans espace) d'un ":", puis un espace, puis, un message descriptif de votre contribution, écrit un minuscules.
* si vous y mettez le nom d'un fichier, utilisez le `display_title` que vous mettez en minuscules, c'est aussi simple que ça

##### Remplacements de $\LaTeX$ pour les noms de fichiers :

| Opération      | Symbole usuel      | Symbole nom de fichier |
| -------------- | ------------------ | ---------------------- |
| Division       | a/b                | a_div_b                |
| Limite en $a$  | lim_(x->a)( f(x) ) | lim\_a\_(f(x))         |
| Exponentiation | a^n                | a&n                    |
Abbréviations communes aussi : 
* "fonction" → "fx"
* "bijection" → "bij"

##### Préfixes de *commit message*

| Type de contribution                                            | Préfixe |
| --------------------------------------------------------------- | ------- |
| Nouvelle preuve                                                 | prv     |
| Modification de preuve                                          | edt     |
| Changement d'organisation<br>(renommage de propriétés, de tags) | org     |
| Ajout ou modification d'un template                             | tmt     |
| Modification des macros de maths                                | mac     |
