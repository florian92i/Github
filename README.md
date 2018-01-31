# Git et Github

## Les commandes de base de la console

### Connaître votre répertoire courant

``pwd``

*******

### Connaître votre répertoire courant
 ``ls``
 
 Si vous souhaitez voir les éléments de votre répertoire courant sous forme de liste, vous pouvez ajouter l'option ``-l`` à la commande ls. Vous pouvez également afficher plus d'informations sur ces éléments en utilisant l'option ``-a``
 
 *******

 ### Créer un fichier
 
 `` touch ``
 
 *******

 ### Créer un dossier
 
 ``mkdir``
 
 ### Afficher le contenu d’un fichier
 
 ``cat``
 
 # Les commandes de Git
 
 ### Pour copier coller sur windows 
 
 ``Ctrl`` +``V`` && ``Shift`` + ``Inser``
 
 *******

 ### Afficher toute les commandes disponible sur git 
 
 ``git``
 
 *******

 ### Activer un dossier comme repository Git
 
 ``git init``
 
 *******

 Il suffit de se placer dans ce dossier avec le Terminal puis d'utiliser la commande ``git init``
 
 ### Gérer un repository
 
 ``git add``
 
 Git génère un index de tous les fichiers dont il doit faire le suivi. Lorsque vous créez un fichier dans un repository, vous devez donc l'ajouter à l'index Git à l'aide de la commande ``git add`` nomDeVotreFichier.extension
 
Gagner du temps, vous pouvez ajouter tous les fichiers dans le répertoire courant en tapant ``git add`` .

*******

#### Modifiez votre repository

``git commit``

Vous devez demander à Git d'enregistrer vos modifications en faisant un ``git commit``. L'option-m vous permet de lui envoyer un message décrivant les modifications effectuées

``git commit -m "La V2 pour hack la nasa est fini !" ``



L'option   -a demande à Git de mettre à jour les fichiers déjà existants dans son index exemple :

``git commit -a -m "Ajouté itinéraire dans checklist-vacances.md"``

*******

#### Historique de nos commits 

``git log``    

affiche la liste de tous les commits que tu as réalisés

* son SHA : son identifiant unique, qui se présente sous forme d'une longue chaîne de caractères et de nombres. Par exemple : "87753191cef0bdb955a4cb4ff841f7c2cce4cb1c".

* son auteur : qui a fait le commit (utile lorsque vous travaillez à plusieurs sur un projet !)

* sa date

* sa description : vous vous rappelez, c'est le message de description que vous indiquez avec l'option  -m lorsque vous faites votre git commit 

*******

### Positionner sur un commit donné de votre historique

``git checkout SHADuCommit`` (SHADuCommit identifiant unique quand on tape git log on peut le voir)

cela va crée une branche parallele 

### revenir à votre branche principale (au commit le plus récent)

``git checkout master``

# Github

#### Astuce quand on est sur le site github

Pour mieux vous y retrouver dans votre code en ligne : __appuyez sur la touche t__, vous pourrez alors __faire une recherche__ dans vos noms de fichiers en tapant un mot / des lettres clé 

### Récupérez du code d'un autre repository

![alt text](https://github.com/florian92i/Github/blob/master/img/clone.PNG)
