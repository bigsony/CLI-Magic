CLI-Magic
=========

Ensembles de commandes utiles sous GNU/Linux
## Gestion de fichiers
 - `rename 's/ /_/g' *` => Renommer tous les fichier d'un répertoire en replaçant les espaces par des underscores
 - `tar cf - * | (cd ../../httpdocs/; tar xvf -)` => Déplacer un dossier et son contenu sans en modifier les droits

## Gestion d'images
 - `mogrify -resize 150 monimage.jpg` => Redimensionne l'image **monimage.jpg** à 150px de large
 - `mogrify -resize 150 *.jpg` => Redimensionne toutes les images jpg d'un dossier à 150px de large

## Subversion
 - `svn log -l 5` => Retourne les 5 dernières lignes d'un log
 - `svn log -l | grep 'USER'` => Lister l'ensemble des COMMIT par USER
 - `svn log -l | grep 'USER' -c` => Récuperer le nombre de COMMIT par USER

## Grep
 - `grep 'mafonction()' --include='\*.php'` => Rechercher les appels de mafonction() uniquement dans les fichiers php
 - `cat toto.txt | grep 'lorem' -c` => Retourne le nombre de "lorem" dans toto.txt
 - `grep -c ^ toto.txt` => Retourne le nombre de lignes du fichier toto.txt

## Composer
 - `sudo composer self-update` => Mets à jour composer
 - `composer global update` => Mets à jour l'ensembre des paquets gérés par composer
