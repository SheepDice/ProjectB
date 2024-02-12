Pour le moment, le notebook check_metadata recupère les infos de toutes les images pour en vérifier les caractéristiques

Il faut télécharger le dataset suivant : https://www.kaggle.com/datasets/gpiosenka/100-bird-species/discussion
L'archive est décompressée à la racine et les directory test, train et valid sont déplacés dans un directory "dataset_birds"
Le directory "dataset_birds" est dupliqué, le deuxième est appelé "dataset_bird_clean". On fera les modifications dans ce dir

Action effectuées : 
- une image est resize par le notebook  check_metadata
- L'oiseau PLUSH CRESTED JAY est supprimé car aucune image n'est à la bonne taille.

Il faudra voir si le Plush Crested Jay peut être gardé, mais peu probable : 
- il faudrait probablement supprimer plusieurs images aux ratio height/width trop éloigné de 1 (224/224)
- Les images resizées perdraient de la qualité. On parle ici de resize et pas de crop car trop compliqué à mettre rapidement en place
- La conséquence, c'est avoir une classe qui est beaucoup moins bien représentée (moins d'image et de plus mauvaise qualité)
- Supprimer une classe parmi 525, sachant que les 525 ne représente pas la totalité des espèces d'oieaux, loin de là, c'est tout a fait acceptable.
