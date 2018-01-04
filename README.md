# formation-boudet-tpg

## COMMANDE AVEC GIT BASH
``cd``: naviguer dans les dossiers

``touch {nomfichier}`` : creer un fichier

```git init``` : demarrer un projet git dans le dossier

``git status`` : infos sur la branch, si un commit est à faire etc...

``git add`` : 
- ``.`` : ajoute tout le dossier pour un commit

- ``{nomfichier}`` : ajoute un fichier spécifique

``git commit`` : enregistre un état
- ``-m “message”`` : pour donner la description du commit
- ``--amend`` : rajoute les modif dans le dernier commit effectué 
``Git config`` : 
- ``--Global``
- ``--System``
- ``--Local``
- ``-f``
-  ``--blob``


Git log : état de l’historique du dépôt

Git checkout:
- {num_de_version}: retourne à une ancienne version, choisir avec git log, on peut saisir que les 4 premiers caracs (pas moins)
- master: retourne à la dernière version
- -- .\todo.txt : Si on veut récupérer la dernière version du fichier contenu dans HEAD
- nombranche : change de branche 

HEAD nomfichier : fait revenir un fichier à l’état du head
-b nombranche : creer une branch et switch direct dessus

git branch :
- nombranche : creer une nouvelle branche

Git merge :
- Nombranche : fusionne la branche actuelle avec celle donné

git stash : met de côté les modifs depuis le dernier commit, sans faire de commit, pour quand on veut changer de tâche de travail sans avoir fini celle en cours. Ne pas oublier de faire git add pour les fichiers creer entre temps
- pop : récuperer le stash

Git reset :
- Nomfichier : supprime le fichier
- --hard HEAD : revenir à l’état du head
- --hard HEAD^ : supprime le dernier commit et switch au précédent


git cherry-pick 33da3c9 : prend un commit d’une autre branche et l’ajoute à la branche actuelle, sans prendre ce qui provient des autres commit.
git fetch : regarde et récupère l’état du serveur distant

Git pull : récupère les derniers commit de ma branche depuis le serveur

Git rebase :
-i : donne des indications sur ce qu’il faut faire avant le rebase

MANIP UTILES

. Après touch .gitignore
Sur unix : $ echo "*.data" >> .gitignore
Sur unix : $ echo "temp/" >> .gitignore
Windows : ouvrir le fichier et ajouter manuellement dedans

Gerer un conflit de merge
Ouvrir les fichiers incriminés, git à ajouter les lignes des deux branches, en choisir une puis refaire add > commit

Repository
Creer un repo sur github sans readme, suivre instructions de on veut push un projet
