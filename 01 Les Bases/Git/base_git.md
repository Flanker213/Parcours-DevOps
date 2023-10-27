## Les bases de GIT

Découvrez les commandes de base de GIT et apprenez à configurer votre environnement de développement pour l'utiliser.

| Commande                 | Description                                  |
|-------------------------|----------------------------------------------|
| `git init`              | Initialise un nouveau dépôt GIT            |
| `git clone <URL>`       | Clone un dépôt GIT existant                |
| `git add <fichier>`     | Ajoute des fichiers à la zone de staging   |
| `git commit -m "message"` | Valide les changements avec un message    |
| `git status`            | Affiche l'état actuel du dépôt              |
| `git log`               | Affiche l'historique des commits            |
| `git branch`            | Affiche la liste des branches              |
| `git checkout <branche>` | Change de branche                        |
| `git pull`              | Met à jour le dépôt local à partir du dépôt distant |
| `git push`              | Envoie les changements locaux au dépôt distant |
| `git diff`              | Affiche les différences entre les fichiers |
| `git reset`             | Annule les changements dans la zone de staging |
| `git remote`            | Affiche les dépôts distants configurés      |
| `git fetch`             | Récupère les dernières modifications du dépôt distant |
| `git merge <branche>`   | Fusionne une branche dans la branche actuelle |
| `git stash`             | Met de côté des modifications non validées |
| `git tag`               | Gère les étiquettes (tags)                  |
| `git revert`            | Annule un commit en créant un nouveau commit |
| `git cherry-pick`       | Applique un commit spécifique sur une branche |
| `git blame <fichier>`   | Affiche l'auteur de chaque ligne d'un fichier |
| `git clean`             | Supprime les fichiers non suivis            |
| `git config`            | Configure les paramètres de GIT            |
| `git show`              | Affiche les détails d'un commit spécifique |
| `git grep`              | Recherche du texte dans les fichiers du dépôt |
| `git archive`           | Crée une archive de l'état du dépôt         |
| `git bisect`            | Aide à trouver le commit introduisant un bogue |
| `git submodule`         | Gère les sous-modules GIT                   |
| `git remote add`        | Ajoute un dépôt distant                     |
| `git remote remove`     | Supprime un dépôt distant                   |
| `git remote rename`     | Renomme un dépôt distant                    |
| `git remote set-url`    | Modifie l'URL d'un dépôt distant             |
| `git rebase`            | Rejoue les commits sur une autre branche    |
| `git pull --rebase`     | Met à jour le dépôt local avec rébase       |
| `git log --oneline`     | Affiche l'historique en une ligne par commit |
| `git log --graph`       | Affiche l'historique sous forme de graphe   |
| `git log --author`      | Filtrage de l'historique par auteur         |
| `git log --since`       | Filtrage de l'historique par date           |
| `git log --grep`        | Filtrage de l'historique par message de commit |
| `git log --oneline --graph` | Affiche l'historique en une ligne avec graphe |
| `git log --follow <fichier>` | Suit le renommage d'un fichier          |
| `git log <branche1>..<branche2>` | Affiche les commits entre deux branches |
| `git log -- <fichier>` | Affiche l'historique d'un fichier spécifique |
| `git blame -L <début>,<fin> <fichier>` | Affiche l'auteur de lignes spécifiques d'un fichier |

[En savoir plus](https://git-scm.com/docs)
[README.md](README.md)
