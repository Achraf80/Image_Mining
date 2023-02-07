ImageMining: Atelier N°1: CBIR

Achraf Ait Laydi

achrafaitlaydi@gmail.com


Table des matières :

1 Introduction
L’objectif de cet atelier est d’initier le lecteur aux systèmes de recherches basées sur le contenu (CBIR, Content Based Image Retrieval). Le CBIR permet entre autres de rechercher les images similaires à une image requête dans une base, constituées, d’images. Cette similarité est calculée non pas sur les images elles-mêmes mais par le biais d’une description (descripteur) choisie par celui qui a conçu le système. La figure ci-dessous présente une vue globale d’un système CBIR.

Un système CBIR est organisé en deux phases :

Phase hors ligne, appelée souvent indexation, où pour chaque image un vecteur descripteur sera extrait et sauvegarder sous forme de base d’indexes
Phase en ligne, appelée souvent recherche, où le système recherche les images similaires à une image requête. Le même type de descripteur sera extrait de l’image requête et comparé avec la base d’indexes.
Deux paramètres sont à prendre en considération lors de l’élaboration d’un système CBIR; le premier est la nature des descripteurs (appelés aussi caractéristiques) à utiliser pour former la base d’indexes, et le deuxième c’est la mesure de similarité à utiliser pour chercher les images les plus similaires pour une image requête. Ainsi, la recherche ce fait par mesure de distance entre descripteurs au lieu des images.

Les descripteurs utilisés pour former la base d’indexes sont généralement des descripteurs bas niveau, à savoir ; la forme, la couleur et la texture. Et la mesure de similarité utilisée peut être une simple distance euclidienne ou une projection multidimensionnelle.

2 Base d’images
Pour cet atelier nous allons utiliser une partie de la base d’images COREL. La base COREL contient 10800 images classées en 80 groupes d’images. Cette base est parfaite pour comprendre les fondamentaux du CBIR. Ici, nous allons utiliser seulement 270 images appartenant à deux groupes d’images et qui sont regroupées dans seule dossier.
Il faut charger la base aprés l'avoir décompresser sur votre espace Drive. Il est possible d'utiliser une base compresser (.*zip) et la décompresser par code python.


3 Implémentation
Afin de développer notre système CBIR nous avons opté, dans cet atelier, pour Matlab comme environnement de travail car il est très puissant dans le traitement matriciel et ainsi pour le traitement d’images de même que plusieurs fonctionnalités sont déjà implémentées permettant de créer facilement notre CBIR.
Pour la première étape qui est l’indexation, le premier code à écrire est pour parcourir toutes les images de la base de données pour extraire de chacune un vecteur descripteur convenable.

Copier la base d’images dans le dossier par défaut de Matlab pour éviter les
Ne pas écrire le code directement sur l’invite de commande mais plutôt créer un ou plusieurs fichiers *.m, les modifier et les exécuter à fur et à mesure de l’avancement de cet atelier.
