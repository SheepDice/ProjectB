Pour le moment, le notebook check_metadata recupère les infos de toutes les images pour en vérifier les caractéristiques

Il faut télécharger le dataset suivant : https://www.kaggle.com/datasets/gpiosenka/100-bird-species/discussion
L'archive est décompressée à la racine et les directory test, train et valid sont déplacés dans un directory "dataset_birds"
Le directory "dataset_birds" est dupliqué, le deuxième est appelé "dataset_bird_clean". On fera les modifications dans ce dir

Action effectuées : 
- une image est resize par le notebook  check_metadata
- L'oiseau PLUSH CRESTED JAY est supprimé car aucune image n'est à la bonne taille.
