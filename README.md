# SummerIA

Instructions d'installation pour SummerIA 2017 (french AI summer school for high-school pupils) 


## Installer la suite Anaconda sur Windows 10/8/7 

**Testé** : sur Win10 (OK)

#### Étapes : 
- télécharger le .exe sur : https://www.continuum.io/downloads
    - choisir la version "Python 3.6, 64-bit installer" si vous êtes sur un ordinateur 64-bit
    - si vous êtes sur une machine 32-bit (assez rare) choisir la version "Python 3.6, 32-bit installer".
    - si vous avez un doute sur le 64 vs 32 bit [rendez-vous ici](http://www.commentcamarche.net/faq/19107-32-ou-64-bits-comment-savoir)

- une fois le *.exe téléchargé (environ 400Mo), double-cliquez dessus :
    - suivez les instructions d'installation, en laissant les paramètres par défaut
    - (sauf si vous voulez installer Anaconda dans un dossier particulier..)
    - à la fin décochez les deux cases 'learn more about ...' 
    - voilà c'est installé ! 


## Installer la suite Anaconda sur Linux 

TODO

## Installer la suite Anaconda sur Mac 

TODO


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
> Beaucoup d'entreprises, comme Google, utilisent cette plateforme pour diffuser leurs projets open-source (libres)

#### Importer l’environnement dans Anaconda


Ce dossier contient un fichier `environment.yaml` qui liste toutes les librairies utiles à la semaine. 
Notamment des libraires pour faire du traitement de l'image, de la reconnaissance de forme, etc.

- Lancez `Anaconda Navigator` (disponible dans Démarrer/Logiciel ..)
- Dans l'onglet 'Environments', cliquez sur 'Import' en bas de la colonne centrale. 
    - nom de l'environnement : `summerIA`
    - puis choisissez le fichier `environment.yaml` fraîchement téléchargé. 
    - puis `OK`

Cette opération va vous créer un environnement Python (Python 3.5 exactement), nommé `summerIA`, avec toutes les librairies nécessaires. Cela peut prendre pas mal de temps (beaucoup d'installations et de fichiers à télécharger).

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
  - **nous vous recommandons de l'installer** notamment pour faire le cours 'pré-requis' de Python
  - il suffit de cliquer sur `Install`.



#### Tester les librairies 

Nous avons créer un fichier `test.py` qui va exécuter certaines opérations de test, pour savoir si tout s'est bien installé. 
Pour ça, nous allons le faire dans `Spyder` : 

- Lancez `Anaconda Navigator`.
- Dans l'onglet `Home`, sélectionnez bien l'environnement `summerIA`, créé précédemment.
- Cliquez sur `Launch` correspondant à `Spyder`.
- Une fois ouvert : Fichier->Ouvrir... , puis sélectionner le fichier `test.py`


A FINIR ... 




