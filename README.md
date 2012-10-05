==========
README
==========

Le site est écrit en RST (ReStructured Text), langage très utilisé dans le monde Python pour la documentation.

Vous trouverez une page qui liste la plupart des balises utilisées ici : 
http://docutils.sourceforge.net/docs/user/rst/quickref.html#hyperlink-targets

Les images, PDF et autres documents doivent être placées dans les répertoires *_static/* les plus 
proches de l'endroit le plus pertinent.

Install
========

Le déploiement utilise un environnement virtuel, ce qui permet d'éviter de modifier le python système.

Installation
-------------

    $ python bootstrap.py
    $ buildout/bin/buildout

Déploiement
-------------

Pour chaque déploiement, il suffit de lancer la commande :
    
    $ make clean html
