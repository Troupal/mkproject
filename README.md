# mkproject
Créer un nouveau projet d'électronique grâce à la mise en place d'une arborescence et de fichiers via un script shell.

## Installation

### Installation via git (recommandé)
`user@machine:~$ mkdir {script}`  
↪ // Remplacer {script} par le nom du dossier où seront installé vos scripts (p.e. bin)  
`user@machine:~$ cd Chemin/du/dossier/script`  
↪ // Chemin absolu ou relatif du dossier précédement créé  
`user@machine:~$ git clone https://framagit.org/Troupal/mkproject.git`  
↪ // Télécharge le dossier .git sur le serveur GitLab de FramaGit   
`user@machine:~$ export PATH=$PATH:$HOME/script`  
↪ // Exporter dans la viariable d'environnement $PATH le contenu du dossier script  

[![asciicast](https://asciinema.org/a/2pQ3U1goLCPSL7ml6BZI7F2KT.svg)](https://asciinema.org/a/2pQ3U1goLCPSL7ml6BZI7F2KT)

### Installation via wget ou  curl

#### Avec wget

`user@machine:~$ mkdir {script}`   
↪ // Remplacer {script} par le nom du dossier où seront installé vos scripts (p.e. bin)  
`user@machine:~$ cd Chemin/du/dossier/script`   
↪ // Chemin absolu ou relatif du dossier précédement créé  
`user@machine:~$ wget 'https://framagit.org/Troupal/mkproject/-/archive/master/mkproject-master.zip' --output-document 'mkproject-master.zip'`  
↪ // Télécharge l'archive zip sur le serveur GitLab de FramaGit  
`user@machine:~$ unzip mkproject-master.zip && rm mkproject-master.zip`  
↪ // Extraire et supprimer l'archive .zip   
`user@machine:~$ export PATH=$PATH:$HOME/script`  
↪ // Exporter dans la viariable d'environnement $PATH le contenu du dossier script  

[![asciicast](https://asciinema.org/a/tEfJX5mRv8Jbegg7pMmdPEFA9.png)](https://asciinema.org/a/tEfJX5mRv8Jbegg7pMmdPEFA9)

#### Avec curl

`user@machine:~$ mkdir {script}`   
↪ // Remplacer {script} par le nom du dossier où seront installé vos scripts (p.e. bin)   
`user@machine:~$ cd Chemin/du/dossier/script`   
↪ // Chemin absolu ou relatif du dossier précédement créé   
`user@machine:~$ curl 'https://framagit.org/Troupal/mkproject/-/archive/master/mkproject-master.zip' --output 'mkproject-master.zip'`   
↪ // Télécharge l'archive zip sur le serveur GitLab de FramaGit   
`user@machine:~$ unzip mkproject-master.zip && rm mkproject-master.zip`   
↪ // Extraire et supprimer l'archive .zip    
`user@machine:~$ export PATH=$PATH:$HOME/script`   
↪ // Exporter dans la viariable d'environnement $PATH le contenu du dossier script    

## Utilisation du script

L'utilisation de ce script est simple mais si vous avez besoin d'aide il vous suffit, pour afficher l'aide, de taper:

`user@machine:~$ mkproject -h`

Pour afficher l'arborescence des dossier, tapez:

`user@machine:~$ mkproject -l`

Enfin, pour utiliser le script, il vous suffit de taper:

`user@machine:~$ mkproject mon_nom_de_projet`

ou bien

`user@machine:~$ mkproject "Mon nom de projet avec des espaces`

[![asciicast](https://asciinema.org/a/ZVHqQfAYq9qCGNPutY2BDsIdi.svg)](https://asciinema.org/a/ZVHqQfAYq9qCGNPutY2BDsIdi)

## TODO
* Terminer l'option -f
* Créer les fichiers de présentation de chaque dossier (.md)
* Créer les modèles de fichiers selon la nomenclature choisie sauf pour les fichiers .odt.
* Créer une gestion des licences.
