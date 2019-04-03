PARTIES 1 ET 2 DU COURS OPENCLASSROOMS : PRENEZ GITHUB EN MAIN :
Mon r�sum� sur GIT et GITHUB :

L'appli GIT bash est une console (Terminal) permettant de taper des commandes Linux dans un syst�me Windows, pour enregistrer en local les diff�rentes versions (commit) du code d'un d�veloppeur.
Ces diff�rentes versions sont enregistr�es dans un dossier local appel� "Repository" en anglais, et "d�p�t Git" en fran�ais.
Si le d�veloppeur rencontre une erreur dans son code, l'appli GIT lui permet de revenir en arri�re en ouvrant une version (un commit) de son code qui fonctionnait.
Lorsqu'on d�veloppe un site web, il faut modifier plusieurs fichiers. L'ensemble de ces fichiers s'appelle un commit.
Lorsqu'on d�veloppe � plusieurs, on a besoin de partager du code, donc de le mettre sur le cloud, avec tous ses commit. Le site github.com sert � �a. Il est gratuit si le partage est Public.
Au lieu de modifier les fichiers sur Git bash, on peut travailler plus facilement avec Visual Studio Code.

MON PROJET :

Taper une page en html avec l'appli gratuite Visual Studio Code. Mon Sujet : Comment r�aliser un simulateur de feux tricolores avec une carte Arduino et l'appli mBlock ?
Enregistrer les 4 commit des fichiers modifi�s lors de l'�criture de cette page web, en local avec GIT, puis en public avec github.com
En local, ces fichiers seront enregistr�s sur C:\Users\Marc\GIT\feu-tricolore\manazur\


M�thode d�taill�e :
Ouvrir la console Git bash pour y taper les commandes :
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
Avant d'utiliser la commande push suivante, aller � github.com pour y cr�er un nouveau Repository, nomm� feu-tricolore. Copier dans le presse-papier son adresse qui est https://github.com/Manazur/feu-tricolore.git (pour pouvoir la coller � l'�tape suivante)
git remote add origin https://github.com/Manazur/feu-tricolore.git : ajoute cette adresse comme nouveau Repository sur le remote Github (serveur distant) du projet feu-tricolore
git push origin master : upload le commit 1 local vers Github. Les �tapes suivantes permettent de faire des modifications sur le code, des commit, des push pour mettre � jour les modif sur Github.

Ouvrir le fichier feux-tricolores.html avec Visual Studio Code pour le compl�ter en y ajoutant le style du th�me prism.js  puis l'enregistrer
git add . : ajoute les dossiers et fichiers (modifi�s depuis le dernier commit) � la liste provisoire (non encore enregistr�e) du prochain commit
git commit -m "ajout� le style du th�me prism.js au fichier feux-tricolores.html" : enregistre en local un nouveau commit
git push origin master : upload le nouveau commit vers Github.

git log : affiche la liste des commit effectu�s et des remarques faites sur chaque commit
q : permet de sortir d'un processus qui bloque la console.

Modifier le fichier feux-tricolores.html avec Visual Studio Code pour le compl�ter en y ajoutant le paragraphe "La carte Arduino", l'enregistrer.
Ajouter une image dans C:\Users\Marc\GIT\feu-tricolore\manazur\cours\img\ArduinoNano.jpg
git add . : ajoute automatiquement tous les nouveaux dossiers et fichiers (modifi�s ou supprim�s depuis le dernier commit) � la liste provisoire (non encore enregistr�e) du prochain commit
git commit -m "ajout� le paragraphe La carte Arduino au fichier feux-tricolores.html et l'image ArduinoNano.jpg" : enregistre en local un nouveau commit avec sa remarque
git push origin master : upload le nouveau commit vers Github.

Modifier le fichier feux-tricolores.html avec Visual Studio Code pour le compl�ter en y ajoutant le paragraphe "Le simulateur", l'enregistrer.
Ajouter les images simulation.gif  trafficlight_components.png  reed-switch.jpg  arduino_pinlayout.png dans C:\Users\Marc\GIT\feu-tricolore\manazur\cours\img\
git add . : ajoute automatiquement tous les nouveaux dossiers et fichiers (modifi�s ou supprim�s depuis le dernier commit) � la liste provisoire (non encore enregistr�e) du prochain commit
git commit -m "ajout� le paragraphe Le simulateur au fichier feux-tricolores.html et les images simulation.gif  trafficlight_components.png  reed-switch.jpg  arduino_pinlayout.png" : enregistre en local un nouveau commit avec sa remarque
git push origin master : upload le nouveau commit vers Github.

Modifier le fichier feux-tricolores.html avec Visual Studio Code pour le compl�ter en y ajoutant les paragraphes "Scratch" et "mBlock", l'enregistrer.
git add . : ajoute automatiquement tous les nouveaux dossiers et fichiers (modifi�s ou supprim�s depuis le dernier commit) � la liste provisoire (non encore enregistr�e) du prochain commit
git commit -m "ajout� les paragraphes Scratch et mBlock au fichier feux-tricolores.html" : enregistre en local un nouveau commit avec sa remarque
git push origin master : upload le nouveau commit vers Github.

Modifier le fichier feux-tricolores.html avec Visual Studio Code pour le compl�ter en y ajoutant le paragraphe "Missions", l'enregistrer.
Ajouter l'image "task_3_init.png" dans C:\Users\Marc\GIT\feu-tricolore\manazur\cours\img\
Ajouter le fichier "trafficlight_start.sb2" dans C:\Users\Marc\GIT\feu-tricolore\manazur\scratch\
git add . : ajoute automatiquement tous les nouveaux dossiers et fichiers (modifi�s ou supprim�s depuis le dernier commit) � la liste provisoire (non encore enregistr�e) du prochain commit
git commit -m "ajout� le paragraphe Missions au fichier feux-tricolores.html et l'image task_3_init.png et le fichier trafficlight_start.sb2" : enregistre en local un nouveau commit avec sa remarque
git push origin master : upload le nouveau commit vers Github.

FIN de ce chapitre.


PARTIE 3 : COLLABOREZ ET MAITRISEZ VOTRE HISTORIQUE.

Le code principal tap� dans le chapitre pr�c�dent est contenu dans la "branche" appel�e Master. Lorsque qu'on initialise un repository Git, le code est plac� dans cette "branche" Master.
Si on veut tester une autre fonctionnalit� sur notre projet, on �crit son code dans une autre "branche" qu'on cr�e :
git branch nouvelle-branche : cr�e une branche ici nomm�e nouvelle-branche
git checkout nouvelle-branche : se d�placer dans la nouvelle branche
git branch : affiche les noms des diff�rentes branches. Int�r�t des branches : pouvoir les supprimer enti�rement si on d�cide de ne pas d�velopper une fonctionnalit� du projet.
git checkout master : se d�placer dans la branche master
git merge nouvelle-branche : fusionne le code de la branche "nouvelle-branche" dans la branche "master". 
Cette fusion peut �tre conflictuelle si 2 personnes ont modifi� un m�me fichier � la m�me ligne et dans ce cas il s'affiche CONFLICT (content): Merge conflict in master
Il faut alors voir les 2 versions manuellement et n'en garder qu'une, l'enregistrer puis faire un commit :
commit -m "conflit r�solu entre les lignes 20 et 30" : la fusion se fera alors sans avoir besoin de refaire un git merge. V�rifier en faisant un git status.
Les conflits peuvent aussi �tre r�solus plus facilement par des outils graphiques comme vimdiff, meld, opendiff, kdiff3, tkdiff, xxdiff, tortoisemerge, gvimdiff, diffuse, ecmerge, p4merge, araxis, emerge
git mergetool vimdiff : utilise l'outil graphique vimdiff pour afficher simultan�ment 2 fichiers et r�soudre un conflit.
git branch -d nouvelle-branche : supprime cette branche.

POUR savoir qui a modifi� une ligne pr�cise de code dans un projet, utiliser la commande git blame : se d�placer dans /manazur/cours/
git blame feux-tricolores.html : affiche les premiers chiffres du SHA du N� du commit, le nom de l'utilisateur qui a �crit chaque ligne, et l'heure d'enregistrement. Remarque : la console n'affiche que la 1�re page, pour afficher la suite, taper la touche espace. Puis "q" et "Entrer" pour quitter.
git show 4256897 (qui sont les premiers chiffres du SHA d'un commit) : affiche plus de d�tails sur les modifications faites sur chaque ligne d'un fichier, ajout�es (+) ou supprim�es (-)

SECURITE :
Ne jamais commiter sur github de fichiers de configuration contenant des mots de passe, des cl�s d'API, etc. Pour les ignorer, cr�er un fichier .gitignore
Puis l'ouvrir et y �crire le nom des fichiers qu'on veut ignorer, ex. /manazur/scratch/fichier.ext     Ces fichiers seront ignor�s lors d'un git status ou d'un git commit
Par contre le fichier .gitignore lui-m�me doit �tre suivi et plac� dans les commit.

EVITER les commit inutiles :
Si on doit interrompre un travail, par ex pour travailler en urgence sur une autre branche, on pourrait �tre tent� de faire un commit, mais il serait incomplet. Il existe un moyen de mettre de c�t� le travail commenc� en tapant la commande git stash
On peut alors travailler sur une autre branche, faire un commit, puis plus tard poursuivre le travail interrompu apr�s avoir tap� la commande git stash pop

CONTRIBUER � des projets open source :
Faire une PR "pull request", c'est proposer une modification � un projet h�berg� sur Github. Commencer par r�cup�rer le Repository auquel on veut contribuer en cliquant sur "Fork", puis :
copier l'URL https de la copie du repo qu'on a "fork�"
git clone https://github.com/manazur/nomduprojetfork�.git
se d�placer dans le Repo qu'on vient de cr�er
git branch mes-modif : cr�er une nouvelle branche o� je ferai mes modifications
git checkout mes-modif : se d�placer dans cette branche. Remarque : les 2 commandes pr�c�dentes peuvent �tre fusionn�es en tapant git checkout -b mes-modif
Faire mes modifications puis les commiter par ex. git commit -m "Added feature allowing users to comment on the blog articles" (�crire en anglais puisque c'est partag�)
git push origin mes-modif : je ne fais pas un "origin master" puisque je n'ai pas travaill� sur la branche principale master
Une fois mes modifications envoy�es sur mon fork GitHub, il reste � transmettre ma demande de modifications en faisant une pull request : se placer sur mon fork GitHub, sur ma nouvelle branche, et cliquer sur "Compare & pull request".
Je serai alors amen� � r�diger un message en anglais pour pr�senter ma proposition de modifications � l'auteur du projet.




Pour en savoir plus sur GIT aller � https://git-scm.com/book/fr/v1/D%C3%A9marrage-rapide-Installation-de-Git
Un cours complet ici : https://perso.liris.cnrs.fr/pierre-antoine.champin/enseignement/intro-git/
Rq. : Visual Studio Code permet non seulement de taper du code, mais donne acc�s � la console pour taper des commandes GIT.
Un cours complet sur Visual Studio Code : https://www.grafikart.fr/tutoriels/windows-installation-vscode-1021
ou aussi sur https://www.supinfo.com/articles/single/6616-decouvrir-visual-studio-code-2017

