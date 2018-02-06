# Git et Github

## Les commandes de base de la console

### Connaître votre répertoire courant

``pwd``

*******

### Connaître les fichiers dans le répertoire courant
 ``ls``
 
 Si vous souhaitez voir les éléments de votre répertoire courant sous forme de liste, vous pouvez ajouter l'option ``-l`` à la commande ls. Vous pouvez également afficher plus d'informations sur ces éléments en utilisant l'option ``-a``
 
 
 `$> ls -la`\
Cette commande affiche les fichiers cachés ( commençant par un "." exemple : ".fichierCaché" ) et en précisant les droits sur ce fichier, s'il est de type fichier ou répertoire et de manière structurée.

 
 *******

 ### Créer un fichier
 
 `touch nomDuFichier.extension`
 
 *******

 ### Créer un dossier
 
 `mkdir leNomDuRepertoire`
 
 ### Afficher le contenu d’un fichier
 
 `cat nomDuFichier.extension`
 
 La commande cat affiche tout le fichier, pour afficher le fichier peu à peu, préconiser l'usage de la commande : 
 
`more nomDuFichier.extension`
 
 ### Se déplacer dans les répertoires
 `cd`
 
 La commande `cd` permet de se déplacer dans un repertoire ( uniquement un répertoire ! ). 
 
 `cd nomDuRep/` \
 `cd nomDuRep/nomDuSousRep/` \
 `cd ..` Permet de remonter dans le répertoire parent \
 `cd -` Permet de revenir dans le répertoire précédent 
 
 
 
 # Les commandes de Git
 https://doc.ubuntu-fr.org/tutoriel/console_ligne_de_commande
 ### Pour copier / coller sur Windows ou UNIX
 
 ``Ctrl`` +``V`` && ``Shift`` + ``Inser``
 
 *******

 ### Afficher toutes les commandes disponibles sur git 
 
 ``git``
 
 *******

 ### Activer un dossier comme repository Git
 
 ``git init``
 
 *******

 Il suffit de se placer dans ce dossier avec le Terminal puis d'utiliser la commande ``git init``
 
 ### Gérer un repository
 
 ``git add``
 
 Git génère un index de tous les fichiers dont il doit faire le suivi. Lorsque vous créez un fichier dans un repository, vous devez donc l'ajouter à l'index Git à l'aide de la commande 
 
 `git add nomDeVotreFichier.extension`
 
Gagner du temps, vous pouvez ajouter tous les fichiers dans le répertoire courant en tapant :

`git add .` 

*******

#### Modifiez votre repository

``git commit``

Vous devez demander à Git d'enregistrer vos modifications en faisant un ``git commit``. __Le commit est obligatoire__ afin d'expliquer les modifications effectuées.

`git commit` \
Cette commande ouvre un editeur de texte où vous pouvez y écrire votre commit \

``git commit -m "La V2 pour hack la nasa est fini !" ``\
Cette commande permet d'écrire directement le message du commit grâce au paramètre `-m`

``git commit -a -m "Ajouté itinéraire dans checklist-vacances.md"``\
L'option   -a demande à Git de mettre à jour les fichiers déjà existants dans son index exemple :

*******

#### Historique de nos commits 

``git log``    

Affiche la liste de tous les commits que tu as réalisé

* son SHA : son identifiant unique, qui se présente sous forme d'une longue chaîne de caractères et de nombres. Par exemple : "87753191cef0bdb955a4cb4ff841f7c2cce4cb1c".

* son auteur : qui a fait le commit (utile lorsque vous travaillez à plusieurs sur un projet !)

* sa date

* sa description : vous vous rappelez, c'est le message de description que vous indiquez avec l'option  -m lorsque vous faites votre git commit 

*******

### Positionner sur un commit donné de votre historique

``git checkout SHADuCommit`` (SHADuCommit identifiant unique quand on tape git log on peut le voir)

cela va créer une branche parallèle 

*******

### Revenir à votre branche principale (au commit le plus récent)

``git checkout master``

*******

# Github

#### Astuce quand on est sur le site github

Pour mieux vous y retrouver dans votre code en ligne : __appuyez sur la touche t__, vous pourrez alors __faire une recherche__ dans vos noms de fichiers en tapant un mot / des lettres clé 

### Récupérez du code d'un autre repository

* Tout d'abord copier l'url

*******

![alt text](https://github.com/florian92i/Github/blob/master/img/clone.PNG)

* Ensuite

``git clone lienFourniParGitHub``

*******

### Créez votre premier repository

 Cliquez sur le bouton "Create new" symbolisé par un signe "+" en haut à droite de votre écran, puis "New repository"
 
 *******

### Envoyez votre code sur GitHub
 
``git push origin master``

Cette commande demande à Git:"Envoie mes modifs dans la branche master de mon remote origin."

*******

### Récupérez des modifications qui on été fait sur un projet github

``git pull origin master``

Envoie dans mon répertoire local les dernières modifications de la branche master située sur mon remote origin. 

*******

## Les branches github

### Voir les branches présentes dans votre repo

``git branch``

### Créer une nouvelle branche

``git branch nouvelle-branche``

###  Ce placer dans une autre branche à l'intérieur de votre repo

``git checkout nouvelle-branche``

création + position = ``git checkout -b ma-branche``

### Fusionnez des branches

Il va souvent vous arriver de vouloir ajouter  dans une branche A les mises à jour que vous avez faites dans une autre branche B
on se place dans la branche  A:
``git checkout brancheA``

Ensuite on fusionne 

``git merge brancheB`` 

### Contribuez à des projets open source

https://openclassrooms.com/courses/gerer-son-code-avec-git-et-github/contribuer-a-des-projets-open-source
