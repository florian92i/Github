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
 
 ## Les commandes de Git
 
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
 
 ###  Gérer un repository
 
 ``git add``
 
 Git génère un index de tous les fichiers dont il doit faire le suivi. Lorsque vous créez un fichier dans un repository, vous devez donc l'ajouter à l'index Git à l'aide de la commande ``git add`` nomDeVotreFichier.extension
 
Gagner du temps, vous pouvez ajouter tous les fichiers dans le répertoire courant en tapant ``git add`` .

*******

### Modifiez votre repository

``git commit``

Vous devez demander à Git d'enregistrer vos modifications en faisant un ``git commit``. L'option-m vous permet de lui envoyer un message décrivant les modifications effectuées

``git commit -m "La V2 pour hack la nasa est fini !" ``



L'option   -a demande à Git de mettre à jour les fichiers déjà existants dans son index exemple :

``git commit -a -m "Ajouté itinéraire dans checklist-vacances.md"``

*******

### Historique de nos commits 

``git log``    

affiche la liste de tous les commits que tu as réalisés

*******

