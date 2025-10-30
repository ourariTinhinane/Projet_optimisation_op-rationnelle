But : prioriser le raccordement des bâtiments les plus simples tout en maximisant le nombre de prises raccordées, en mutualisant les lignes quand c’est utile.

Métriques (difficulté & priorisation)

Conformément à la discussion :

Difficulté(infrastructure) = longueur / nombre_de_maisons_que_cela_permet_de_raccorder. 


Ajustements pratiques :

Si etat = à_remplacer, appliquer un surcoût multiplicatif.

Si cout est disponible et plus fiable que longueur, on peut pondérer :
difficulte_infra = alpha * cout + (1 - alpha) * longueur / max(1, nb_maisons).

Difficulté(bâtiment) = somme des difficultés des infrastructures qui le raccordent (on somme les difficultés et non “les intérêts”). On commence par les points les plus faciles. (Cela reprend la contrainte 
“on fait la somme des difficultés, pas des intérêts, et on démarre par le plus simple.”)
