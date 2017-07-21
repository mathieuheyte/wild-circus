Lien vers une ressource Git intéressante.
https://github.com/nvie/gitflow

Pour créer un nouveau commit:

En faisant git status, vous devriez voir les fichiers que vous avez modifiés en rouge. Cela signifie qu’ils ne seront pas pris en compte lorsque vous allez faire un commit.

Il faut explicitement préciser les fichiers que vous voulez « commiter ». Pour cela, trois possibilités :

faire git add nomfichier1 nomfichier2 pour ajouter les fichiers à la liste de ceux devant faire l’objet d’un commit, puis faire un git commit. Si vous faites ungit status après ungit add, vous les verrez alors en vert ;
faire git commit -a pour « commiter » tous les fichiers qui étaient listés dans git status dans les colonnes « Changes to be committed » et « Changed but not updated » (qu’ils soient en vert ou en rouge) ;
faire git commit nomfichier1 nomfichier2 pour indiquer lors du commit quels fichiers précis doivent être « commités ».
