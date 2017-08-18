```bahs

conda create --name test-wagon  python=3.5
source activate test-wagon
pip install wagon

wagon create -r requirements.txt keras

zenith@zenith:~/Data/SummerIA/SummerIA/test_wagon$ ls -alh
total 105M
drwxrwxrwx 1 root root  400 Aug 18 10:41 .
drwxrwxrwx 1 root root 4.0K Aug 18 10:32 ..
-rwxrwxrwx 1 root root 105M Aug 18 10:41 Keras-2.0.6-py35-none-linux_x86_64.wgn
-rwxrwxrwx 1 root root   68 Aug 18 10:40 README.md
-rwxrwxrwx 1 root root   31 Aug 18 10:37 requirements.txt

#105Mo de source code téléchargé et assemblé
# va installer les librairies depuis le fichier *.wgn !
# sans utiliser internet
wagon install Keras-2.0.6-py35-none-linux_x86_64.wgn

conda env export --file env_content.txt
# les librairies du *.wgn sont bien instllées dans l'env conda !
```



**TODO :**
- écrire le fichier `requirements.txt` avec toutes les dependances
- comprendre pourquoi on est obligé de donné en argument à `wagon create` le nom d'une des librairies
- test sous Windows !!!


**INSTALL**
- télécharger l'installers d'Anaconda
- créer un environnemnt Python3.5 vide `summerIA`
- y installer `wagon`
- installer toutes les dependances depuis un fichier `*.wgn`

Seulement les étapes 2 et 3 demandent une connexion internet (environ 20Mo)
Le reste (installer Anaconda et *.wgn) seront diffusés par clefs USB ou par réseau local.

