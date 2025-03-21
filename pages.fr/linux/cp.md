# cp

> Copier fichiers et répertoires.
> Plus d'informations : <https://www.gnu.org/software/coreutils/manual/html_node/cp-invocation.html>.

- Copier un fichier vers un autre emplacement :

`cp {{chemin/vers/fichier_original.ext}} {{chemin/vers/fichier_cible.ext}}`

- Copier un ficher d'un répertoire vers un autre en conservant le nom du fichier :

`cp {{chemin/vers/fichier_original.ext}} {{chemin/vers/repertoire_cible}}`

- Copier récursivement le contenu d'un répertoire vers un autre emplacement (si la destination existe, le répertoire est copié dans celle-ci) :

`cp {{[-r|--recursive]}} {{chemin/vers/repertoire_source}} {{chemin/vers/repertoire_cible}}`

- Copier récursivement le contenu d'un répertoire vers un autre emplacement en mode verbeux (affichage des noms fichiers à mesure de leur copie) :

`cp {{[-vr|--verbose --recursive]}} {{chemin/vers/repertoire_source}} {{chemin/vers/repertoire_cible}}`

- Copier les fichiers textes vers un autre emplacement, en mode interactive (demande une confirmation avant d'écrire par dessus un fichier du même nom) :

`cp {{[-i|--interactive]}} {{*.txt}} {{chemin/vers/repertoire_cible}}`

- Suivre le lien symbolique avant de copier (copie le fichier lié, et non le lien) :

`cp {{[-L|--dereference]}} {{link}} {{chemin/vers/repertoire_cible}}`

- Utiliser le chemin complet du fichier source, créant tout répertoire manquant lors de la copie :

`cp --parents {{chemin/vers/fichier_source}} {{chemin/vers/fichier_cible}}`
