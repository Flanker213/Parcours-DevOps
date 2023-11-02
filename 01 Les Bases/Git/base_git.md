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


### Environnement de travail et Configuration

L'environnement de travail est l'espace où vous effectuez vos opérations de développement. Vous pouvez créer un nouvel environnement de travail en initialisant un dépôt Git à l'aide de la commande `git init`, ou vous pouvez copier un dépôt existant depuis un emplacement distant en utilisant `git clone`. Pour personnaliser votre environnement de travail, vous pouvez configurer les paramètres de Git en utilisant `git config`. De plus, vous pouvez spécifier des fichiers et des dossiers à ignorer en créant un fichier `.gitignore`, ce qui vous permet de maintenir un environnement de travail propre et organisé en excluant des fichiers indésirables de la gestion de version.

| Notion                      | Description                                       |
|-----------------------------|---------------------------------------------------|
| **Environnement de travail** | L'espace où vous travaillez sur vos projets Git. |
| **Initialisation de dépôt** | Crée un nouveau dépôt Git avec `git init`.       |
| **Clonage de dépôt**        | Copie un dépôt Git existant avec `git clone`.    |
| **Configuration de Git**    | Personnalisation des paramètres de Git avec `git config`. |
| **Fichier .gitignore**      | Liste des fichiers et dossiers à ignorer dans Git. |

### Gestion des Fichiers

Lorsque vous travaillez avec Git, il est essentiel de comprendre l'état des fichiers dans votre dépôt. Les fichiers peuvent être suivis (tracked), en attente (staged), ou non suivis (untracked). Vous ajoutez des modifications à la zone de staging avec la commande `git add`, puis vous validez ces changements dans le dépôt en créant un commit avec `git commit`. Si vous souhaitez vérifier les différences entre les fichiers actuels et les derniers commits, vous pouvez utiliser `git diff`. De plus, si vous avez besoin d'annuler des changements avant de les valider, `git reset` est une commande utile pour cela.

| Notion               | Description                                            |
|----------------------|--------------------------------------------------------|
| **État des fichiers** | Suivis, en attente, non suivis (tracked, staged, untracked). |
| **Ajout de fichiers** | Ajoute des modifications à la zone de staging avec `git add`. |
| **Commit**           | Valide les changements dans le dépôt avec `git commit`. |
| **Différences**      | Affiche les différences entre les fichiers avec `git diff`. |
| **Annulation de changements** | Annule des modifications avec `git reset`. |

### Historique et Gestion des Commits

La gestion de l'historique et des commits est cruciale pour le suivi des modifications dans Git. L'historique des commits est accessible via `git log`, ce qui vous permet de visualiser l'historique des modifications dans le dépôt, y compris les auteurs, les dates et les messages de commit. Vous pouvez également fusionner des branches avec `git merge` pour intégrer des modifications d'une branche à une autre. Le tagging, effectué avec `git tag`, vous permet de marquer des points importants dans l'historique, tels que des versions stables. Enfin, `git revert` est utile pour annuler des commits spécifiques tout en préservant l'historique, et `git cherry-pick` vous permet d'appliquer des commits spécifiques d'une branche à une autre.

| Notion              | Description                                          |
|---------------------|------------------------------------------------------|
| **Historique**      | Liste des commits dans le dépôt avec `git log`.     |
| **Fusion de branches** | Fusionne des branches avec `git merge`.          |
| **Étiquetage (Tagging)** | Marque des points spécifiques avec `git tag`.    |
| **Revert et Cherry-pick** | Annule des commits avec `git revert` et applique des commits spécifiques avec `git cherry-pick`. |



### Comprendre le fichier .gitignore

Le fichier `.gitignore` est un élément crucial lors de l'utilisation de Git pour gérer un projet. Il permet de spécifier quels fichiers et répertoires doivent être ignorés par Git, c'est-à-dire exclus de la surveillance de version. Cela est particulièrement utile pour éviter d'inclure des fichiers temporaires, des données sensibles ou des fichiers générés automatiquement dans votre dépôt Git.

## Création du fichier .gitignore

Pour créer un fichier `.gitignore`, il vous suffit de créer un nouveau fichier nommé `.gitignore` à la racine de votre projet. Il peut également être nommé `.gitignore.md` si vous préférez le format Markdown pour la documentation.

## Syntaxe du fichier .gitignore

Le fichier `.gitignore` utilise une syntaxe simple pour spécifier les éléments à ignorer. Vous pouvez utiliser des motifs de correspondance pour exclure plusieurs fichiers ou répertoires en une seule ligne. Voici quelques exemples courants :

- Pour ignorer tous les fichiers avec une certaine extension, utilisez `*.extension`.
- Pour ignorer un répertoire, ajoutez simplement le nom du répertoire suivi d'un `/`.
- Vous pouvez également utiliser `!` pour exclure des fichiers ou des répertoires spécifiques des règles d'ignorance.

Exemple de contenu pour un fichier `.gitignore` :

```gitignore
# Ignorer tous les fichiers .log
*.log

# Ignorer le répertoire node_modules
node_modules/

# Exclure le fichier config.txt de l'ignorance
!config.txt

  
- [Documentation](https://git-scm.com/docs)
- [README.md](README.md)