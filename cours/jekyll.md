# Jekyll #

Jekyll est un générateur de site codé en Ruby. De plus, les sites en HTTPS sont mieux référencés.
L'objectifs de Jekyll est de permettre de voir les modifications sans passer par GitHub. 
On accède au site en allant sur : http:username.github/flatfile

## Commande ##

Commande d'insatallation

gem install jekyll
sudo apt install jekyll
gem install bundler -> gestion de paquet

jekyll serve -> lance le serveur
jekyl build -> création d'uun dossier avec l'ensemble du site

les fichiers "_nomdossier" ne sont pas générés par le site. De ce fait il ne faut pas travailler dans ce genre de fichier.

## Layout ##

Le layout est un gabarit. Il permet de concerver des données sur les pages souhaitées sans avoir à recopier le code pour chaque page.

mkdir _layouts -> creation d'un repertoire layout 
touch default.html -> creation dans le répertoire layout le fichier default 

Dans ce fichier, il faut écrire le code corresepondant aux directives voulues et correspondant au gabarit souhaité. 
Pour laisser la place au contenu (le main) on écrit: {{ content }}. Puis dans le fichier index on écrit en plus du main et entre les lignes en pointillées ce code-ci : layout: default
