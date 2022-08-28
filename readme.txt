Le script run_test.sh lance les 3 algorithmes sur tous les tests de la base de Varoumas:

Pour lancer le script run_test.sh, il faudra qu'il y ait dans le même répertoire
que le script le dossier "samples" contenant tous les tests de Varoumas
ainsi que l'executable "projet.jar"
Enfin, il faudra utiliser la commande suivante:

bash run_test.sh

Les résultats seront alors écrits dans un fichier test.csv
Le fichier test.csv présent dans le répertoire est issu de ce script (~15min d'execution).

Pour effectuer un test personnalisé, on peut executer directement projet.jar:

L'exécutable projet.jar permet de calculer le cercle minimum d'un ensemble de
points.
Il a été compilé avec la version 60.0 de la JRE.

Cet exécutable requiert en premier argument un fichier contenant un point par
ligne sous la forme suivante:
x y
où x est la coordonnée en abscisse du point et y celle en ordonnée. x et y
doivent être des entiers.

Le deuxième argument est l'algorithme souhaité :
  -0 pour l'algorithme naïf
  -1 pour l'algorithme récursif de Welzl
  -Tout autre valeur pour l'algorithme itératif de Welzl

Enfin un troisième argument peut être ajouté. S'il vaut 1, l'exécutable
affichera la valeur du cercle calculé.

Par exemple, pour le lancer avec le test 2 et afficher le résultat en utilisant
l'algorithme naïf, il conviendra d'utiliser la commande suivante:

java -jar projet.jar samples/test-2.points 0 1

