Mon résumé sur GIT et GITHUB :

L'appli GIT est une console (Terminal) permettant de taper des commandes Linux dans un système Windows, pour enregistrer en local les différentes versions (commit) du code d'un développeur.
Ces différentes versions sont enregistrées dans un dossier local appelé "Repository" en anglais, et "dépôt Git" en français.
Si le développeur rencontre une erreur dans son code, l'appli GIT lui permet de revenir en arrière en ouvrant une version (un commit) de son code qui fonctionnait.
Lorsqu'on développe un site web, il faut modifier plusieurs fichiers. L'ensemble de ces fichiers s'appelle un commit.
Lorsqu'on développe à plusieurs, on a besoin de partager du code, donc de le mettre sur le cloud, avec tous ses commit. Le site github.com sert à ça. Il est gratuit si le partage est Public.


MON PROJET :

Taper une page en html avec l'appli gratuite Visual Studio Code. Mon Sujet : Comment réaliser un simulateur de feux tricolores avec une carte Arduino et l'appli mBlock ?
Enregistrer les 4 commit des fichiers modifiés lors de l'écriture de cette page web, en local avec GIT, puis en public avec github.com
En local, ces fichiers seront enregistrés sur C:\Users\Marc\GIT\feu-tricolore\manazur\


Méthode détaillée :
Ouvrir la console Git pour y taper les commandes :
pwd : affiche l'adresse du dossier de travail en cours /c/users/marc
mkdir git : crée le dossier git
cd git : se déplacer dans le dossier créé
mkdir feu-tricolore : crée le dossier feu-tricolore
cd feu-tricolore : se déplacer dans le dossier créé. Continuer ainsi pour créer les chemins suivants :   C:\Users\Marc\GIT\feu-tricolore\manazur\   C:\Users\Marc\GIT\feu-tricolore\manazur\cours\img   C:\Users\Marc\GIT\feu-tricolore\manazur\scratch\
ls : lister le contenu du dossier de travail en cours. Enregistrer le présent document à C:\Users\Marc\GIT\feu-tricolore\manazur\readme.txt
cd .. : remonter au dossier parent. A utiliser pour se déplacer à C:\Users\Marc\GIT\feu-tricolore\manazur\cours\
touch feux-tricolores.html : crée le fichier à C:\Users\Marc\GIT\feu-tricolore\manazur\cours\feux-tricolores.html   Modifier ce fichier en l'ouvrant dans Visual Studio Code
cd.. : à utiliser pour remonter à C:\Users\Marc\GIT\feu-tricolore\manazur
git status : savoir si le dossier en cours est déclaré comme dossier "Repository"
git init : déclarer le dossier en cours comme nouveau Repository (dépôt Git)
git status : vérifie que le dossier /manazur est déclaré comme Repository, et qu'il contient des fichiers prêt à être ajoutés à un commit
git add . : ajoute les dossiers et fichiers créés dans /manazur à la liste provisoire (non encore enregistrée) du commit 1 initial
git commit -m "arborescence intiale du projet feux tricolores" pour enregistrer en local le commit 1 (l'ensemble des modifications faites en local sur les fichiers) avec sa remarque entre " "
Avant d'utiliser la commande push suivante, aller à github.com pour y créer un nouveau Repository, nommé feu-tricolore. Copier dans le presse-papier son adresse qui est https://github.com/Manazur/feu-tricolore.git
git remote add origin https://github.com/Manazur/feu-tricolore.git : ajoute cette adresse comme nouveau Repository sur le remote Github (serveur distant) du projet feu-tricolore
git push origin master : upload le commit 1 local vers Github



modifier le fichier feux-tricolores.html
git add . pour ajouter ce fichier .html à la liste du commit 2 (ou git add -a feux-tricolores.html )
git push origin master pour duppliquer le commit 2 vers Github (service de cloud pour partager du code entre collaborateurs)
git pull pour duppliquer de Github vers local (pour rapatrier en local les mises à jour faites par les collaborateurs)
git log pour voir la liste des commit effectués et des remarques faites sur chaque commit

Pour en savoir plus sur GIT aller à https://fr.atlassian.com/git/tutorials/setting-up-a-repository

Pour passer de feux-tricolores-0.html à feux-tricolores-1.html :
ajouté le style du thème prism.js

Pour passer de feux-tricolores-1.html à feux-tricolores-2.html :
ajouté le paragraphe "La carte Arduino" et l'image "ArduinoNano.jpg"

Pour passer de feux-tricolores-2.html à feux-tricolores-3.html :
ajouté le paragraphe "Le simulateur" et les images "simulation.gif", "trafficlight_components.png", "reed-switch.jpg", "arduino_pinlayout.png"

Pour passer de feux-tricolores-3.html à feux-tricolores-4.html :
ajouté les paragraphes "Scratch" et "mBlock"

Pour passer de feux-tricolores-4.html à feux-tricolores-5.html :
ajouté le paragraphe "Missions" et l'image "task_3_init.png"