Mon r�sum� sur GIT et GITHUB :

L'appli GIT est une console (Terminal) permettant de taper des commandes Linux dans un syst�me Windows, pour enregistrer en local les diff�rentes versions (commit) du code d'un d�veloppeur.
Ces diff�rentes versions sont enregistr�es dans un dossier local appel� "Repository" en anglais, et "d�p�t Git" en fran�ais.
Si le d�veloppeur rencontre une erreur dans son code, l'appli GIT lui permet de revenir en arri�re en ouvrant une version (un commit) de son code qui fonctionnait.
Lorsqu'on d�veloppe un site web, il faut modifier plusieurs fichiers. L'ensemble de ces fichiers s'appelle un commit.
Lorsqu'on d�veloppe � plusieurs, on a besoin de partager du code, donc de le mettre sur le cloud, avec tous ses commit. Le site github.com sert � �a. Il est gratuit si le partage est Public.


MON PROJET :

Taper une page en html avec l'appli gratuite Visual Studio Code. Mon Sujet : Comment r�aliser un simulateur de feux tricolores avec une carte Arduino et l'appli mBlock ?
Enregistrer les 4 commit des fichiers modifi�s lors de l'�criture de cette page web, en local avec GIT, puis en public avec github.com
En local, ces fichiers seront enregistr�s sur C:\Users\Marc\GIT\feu-tricolore\manazur\


M�thode d�taill�e :
Ouvrir la console Git pour y taper les commandes :
pwd : affiche l'adresse du dossier de travail en cours /c/users/marc
mkdir git : cr�e le dossier git
cd git : se d�placer dans le dossier cr��
mkdir feu-tricolore : cr�e le dossier feu-tricolore
cd feu-tricolore : se d�placer dans le dossier cr��. Continuer ainsi pour cr�er les chemins suivants :   C:\Users\Marc\GIT\feu-tricolore\manazur\   C:\Users\Marc\GIT\feu-tricolore\manazur\cours\img   C:\Users\Marc\GIT\feu-tricolore\manazur\scratch\
ls : lister le contenu du dossier de travail en cours. Enregistrer le pr�sent document � C:\Users\Marc\GIT\feu-tricolore\manazur\readme.txt
cd .. : remonter au dossier parent. A utiliser pour se d�placer � C:\Users\Marc\GIT\feu-tricolore\manazur\cours\
touch feux-tricolores.html : cr�e le fichier � C:\Users\Marc\GIT\feu-tricolore\manazur\cours\feux-tricolores.html   Modifier ce fichier en l'ouvrant dans Visual Studio Code
cd.. : � utiliser pour remonter � C:\Users\Marc\GIT\feu-tricolore\manazur
git status : savoir si le dossier en cours est d�clar� comme dossier "Repository"
git init : d�clarer le dossier en cours comme nouveau Repository (d�p�t Git)
git status : v�rifie que le dossier /manazur est d�clar� comme Repository, et qu'il contient des fichiers pr�t � �tre ajout�s � un commit
git add . : ajoute les dossiers et fichiers cr��s dans /manazur � la liste provisoire (non encore enregistr�e) du commit 1 initial
git commit -m "arborescence intiale du projet feux tricolores" pour enregistrer en local le commit 1 (l'ensemble des modifications faites en local sur les fichiers) avec sa remarque entre " "
Avant d'utiliser la commande push suivante, aller � github.com pour y cr�er un nouveau Repository, nomm� feu-tricolore. Copier dans le presse-papier son adresse qui est https://github.com/Manazur/feu-tricolore.git
git remote add origin https://github.com/Manazur/feu-tricolore.git : ajoute cette adresse comme nouveau Repository sur le remote Github (serveur distant) du projet feu-tricolore
git push origin master : upload le commit 1 local vers Github



modifier le fichier feux-tricolores.html
git add . pour ajouter ce fichier .html � la liste du commit 2 (ou git add -a feux-tricolores.html )
git push origin master pour duppliquer le commit 2 vers Github (service de cloud pour partager du code entre collaborateurs)
git pull pour duppliquer de Github vers local (pour rapatrier en local les mises � jour faites par les collaborateurs)
git log pour voir la liste des commit effectu�s et des remarques faites sur chaque commit

Pour en savoir plus sur GIT aller � https://fr.atlassian.com/git/tutorials/setting-up-a-repository

Pour passer de feux-tricolores-0.html � feux-tricolores-1.html :
ajout� le style du th�me prism.js

Pour passer de feux-tricolores-1.html � feux-tricolores-2.html :
ajout� le paragraphe "La carte Arduino" et l'image "ArduinoNano.jpg"

Pour passer de feux-tricolores-2.html � feux-tricolores-3.html :
ajout� le paragraphe "Le simulateur" et les images "simulation.gif", "trafficlight_components.png", "reed-switch.jpg", "arduino_pinlayout.png"

Pour passer de feux-tricolores-3.html � feux-tricolores-4.html :
ajout� les paragraphes "Scratch" et "mBlock"

Pour passer de feux-tricolores-4.html � feux-tricolores-5.html :
ajout� le paragraphe "Missions" et l'image "task_3_init.png"