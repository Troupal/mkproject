# mkproject
Créer un nouveau projet d'électronique grâce à la mise en place d'une arborescence et de fichiers via un script shell.

## Installation

### Installation via git (recommandé)
`user@machine:~$ mkdir {script}` // Remplacer {script} par le nom du dossier où seront installé vos scripts (p.e. bin)
`user@machine:~$ cd Chemin/du/dossier/script` // Chemin absolu ou relatif du dossier précédement créé
`user@machine:~$ git clone https://framagit.org/Troupal/mkproject.git` // Télécharge le dossier .git sur le serveur GitLab de FramaGit 
`user@machine:~$ export PATH=$PATH:$HOME/script` // Exporter dans la viariable d'environnement $PATH le contenu du dossier script

### Installation via wget ou  curl

#### Avec wget

`user@machine:~$ mkdir {script}` // Remplacer {script} par le nom du dossier où seront installé vos scripts (p.e. bin)
`user@machine:~$ cd Chemin/du/dossier/script` // Chemin absolu ou relatif du dossier précédement créé
`user@machine:~$ wget 'https://framagit.org/Troupal/mkproject/-/archive/master/mkproject-master.zip' --output-document 'mkproject-master.zip'` // Télécharge l'archive zip sur le serveur GitLab de FramaGit
`user@machine:~$ unzip mkproject-master.zip && rm mkproject-master.zip` // Extraire et supprimer l'archive .zip 
`user@machine:~$ export PATH=$PATH:$HOME/script` // Exporter dans la viariable d'environnement $PATH le contenu du dossier script

[![asciicast](https://asciinema.org/a/EHCtyTKRVP9SOm3N5FdzxqEg0.png)](https://asciinema.org/a/EHCtyTKRVP9SOm3N5FdzxqEg0)

#### Avec curl

`user@machine:~$ mkdir {script}` // Remplacer {script} par le nom du dossier où seront installé vos scripts (p.e. bin)
`user@machine:~$ cd Chemin/du/dossier/script` // Chemin absolu ou relatif du dossier précédement créé
`user@machine:~$ curl 'https://framagit.org/Troupal/mkproject/-/archive/master/mkproject-master.zip' --output 'mkproject-master.zip'` // Télécharge l'archive zip sur le serveur GitLab de FramaGit
`user@machine:~$ unzip mkproject-master.zip && rm mkproject-master.zip` // Extraire et supprimer l'archive .zip 
`user@machine:~$ export PATH=$PATH:$HOME/script` // Exporter dans la viariable d'environnement $PATH le contenu du dossier script

## TODO
- Terminer l'option -f
- Créer les fichiers de présentation de chaque dossier (.md)
- Créer les modèles de fichiers selon la nomenclature choisie sauf pour les fichiers .odt.
