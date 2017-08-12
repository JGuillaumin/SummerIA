# SummerIA

Instructions d'installation pour SummerIA 2017 (french AI summer school for high-school pupils) 

## Anaconda


## Installer la suite Anaconda sur Windows 10/8/7 

**Testé** : sur Win10, Win7 (OK)

#### Étapes :

- télécharger le fichier *.exe sur : https://www.continuum.io/downloads (onglet "Download for Windows")
    - choisir la version "Python 3.6, 64-bit installer" si vous êtes sur un ordinateur 64-bit
    - si vous êtes sur une machine 32-bit (assez rare) choisir la version "Python 3.6, 32-bit installer".
    - si vous avez un doute sur le 64 vs 32 bit [rendez-vous ici](http://www.commentcamarche.net/faq/19107-32-ou-64-bits-comment-savoir)

- une fois le *.exe téléchargé (environ 400Mo), double-cliquez dessus :
    - suivez les instructions d'installation, en laissant les paramètres par défaut
    - (sauf si vous voulez installer Anaconda dans un dossier particulier..)
    - à la fin décochez les deux cases 'learn more about ...' 
    - voilà c'est installé ! 


## Installer la suite Anaconda sur Linux 

**Testé** : sur Ubuntu 16.04 (OK)

- télécharger le *.sh sur : https://www.continuum.io/downloads (onglet "Download for Linux")
    - choisir la version "Python 3.6, 64-bit (x86) Installer"

- une fois le *.sh téléchargé (environ 500Mo):
     - ouvrez un terminal (Ctrl + Alt +t)
     - allez dans le dossier où se trouve le *.sh, par exemple :
        `cd /home/user_name/Téléchargements/`
     - Exécuter ces commandes :

```bash
# installer Anaconda dans /opt/anaconda3, et -b vous evite de répondre à toutes les questions
sudo bash Anaconda3-4.4.0-Linux-x86_64.sh -b -p /opt/anaconda3

# ces deux lignes permettent d utiliser anaconda-navigator et conda
# sans modifier les variables d environnement
sudo ln -s /opt/anaconda3/bin/anaconda-navigator /usr/local/bin/anaconda-navigator
sudo ln -s /opt/anaconda3/bin/conda /usr/local/bin/conda
```

Et voilà tout est installé !



## Installer la suite Anaconda sur Mac

**Non testé**

- télécharger le *.pkg sur : https://www.continuum.io/downloads (onglet "Download for macOS")
    - choisir le fichier "Graphical Installer for Python 3.6)"

- double-cliquer dessus pour l'installer

**TOTO** : est-ce que le pocesseur d'un mac peut tester l'installation ?


## Créer l'environnement de travail pour SummerIA 

Maintenant il faut vous créer un environnement avec toutes les librairies nécessaires pour les ateliers et projets de la semaine. 
Un environnement vous permet de cloisonner des espaces de travail. 
Par exemple vous pouvez vous créer un environnement avec des librairies/outils dédiés aux mathématiques. Un autre pour faire des simulations de physique. 

#### Télécharger les fichiers de configuration

Rendez vous sur https://github.com/JGuillaumin/SummerIA : 

- cliquer sur 'Cloner or Download'
- télécharger le fichier ZIP ('Download ZIP')
- décompresser ce fichier dans un répertoire. 

> GitHub est un service web d'hébergement et de gestion de code informatique. 
> C'est très pratique pour travailler à plusieurs sur le même projet. 
> Beaucoup d'entreprises, comme Google, utilisent cette plateforme pour diffuser leurs projets open-source (libres), ce qui permet à tout le monde d'utiliser et d'améliorer ces outils.

#### Importer l’environnement dans Anaconda


Ce dossier contient un fichier `environment.yaml` qui liste toutes les librairies utiles à la semaine. 
Notamment des libraires pour faire du traitement de l'image, de la reconnaissance de forme, etc.

##### Windows et Max

- Lancez `Anaconda Navigator`

    - disponible dans Démarrer/Logiciel pour Windows

    - pour Mac ... à tester ?

- Dans l'onglet 'Environments', cliquez sur 'Import' en bas de la colonne centrale. 
    - nom de l'environnement : `summerIA`
    - puis choisissez le fichier `environment.yaml` fraîchement téléchargé. 
    - puis `OK`

##### Linux

Sous Linux, pas besoin de lancer une fenêtre graphique (`anaconda-navigator`) une seule ligne de commande suffit :

```bash
cd Téléchargements/SummerIA/
conda env create -f environment.yaml -n summerIA

```


Mais vous pouvez toujours lancer  `Anaconda Navigator` sous Linux, avec la commande `anaconda-navigator` dans un terminal(à ne pas fermer).


Cette opération va vous créer un environnement Python (Python 3.5 exactement), nommé `summerIA`, avec toutes les librairies nécessaires.
Cela peut prendre pas mal de temps (beaucoup d'installations et de fichiers à télécharger).

Voilà, tout est prêt pour travailler ensemble à Lyon du 20 au 26 août prochain. 
Lors des premiers jours de la semaine nous vous donnerons tous les ficihers, bases de données, et autres, pour travailler.

Maintenant, à chaque fois que vous allez travailler sur des projets lors de la SummerIA, pensez à bien choisir l'environnement 

#### Ajouter 'Spyder'

Lorsque `Anaconda Navigator` est ouvert, dans l'onglet `Home`, vous allez trouver :

- **Jupyter Notebook (déjà installé)**
  - permet d'écrire du code Python dans une page web
  - d’exécuter le code morceau par morceau
  - d'afficher des images et courbes très facilement
  - nous allons beaucoup utiliser cette façon de travailler, car très interactive !

- **Ipyton qtconsole (déjà installé)**
  - il s'agit d'un terminal python interactif
  - très similaire en beaucoup de points à Jupyter notebook 
  - mais ne fonctionne pas dans une page
  
- **Spyder (non installé)**
  - il s'agit d'un environnement de développement (IDE) pour Python
  - vous allez pouvoir écrire du code Python dans des scripts (fichiers .py) 
  - et les exécuter facilement
  - **nous vous recommandons de l'installer** notamment pour faire le cours 'prérequis' de Python
  - il suffit de cliquer sur `Install`.






