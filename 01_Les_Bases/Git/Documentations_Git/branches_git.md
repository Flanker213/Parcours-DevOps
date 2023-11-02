# Documentation sur les Branches Git

## (1/5) Définition des Branches Git
Les branches Git sont des copies indépendantes de votre code source, créées à partir de la branche principale (généralement "master" ou "main"). Elles permettent de travailler sur différentes fonctionnalités ou correctifs de manière isolée, sans affecter la version principale du projet. Voici comment créer une nouvelle branche et la basculer :

### Créer une nouvelle branche
```bash
git branch ma_nouvelle_branche
```

### Basculer vers la nouvelle branche
```bash
git checkout ma_nouvelle_branche
```

## (2/5) Fusionner (Merge) des Branches
La fusion (merge) est le processus de combinaison des modifications de deux branches différentes. Par exemple, pour fusionner une branche "ma_nouvelle_branche" dans "master," faites ce qui suit :

### Basculer sur la branche "master"
```bash
git checkout master
```

### Fusionner "ma_nouvelle_branche" dans "master"
```bash
git merge ma_nouvelle_branche
```

## (3/5) Conflits de Fusion (Merge Conflict)
Les conflits surviennent lorsque Git ne peut pas automatiquement fusionner les modifications. Pour résoudre un conflit, éditez manuellement les fichiers en conflit, puis effectuez un commit :

```bash
# Après avoir résolu le conflit, ajoutez les fichiers modifiés à l'index
git add fichier_en_conflit

# Effectuez un commit pour valider la résolution du conflit
git commit -m "Résolution du conflit"
```

## (4/5) Réorganiser (Rebase) des Branches
Le rébase permet de replacer les modifications d'une branche sur une autre. Cela crée une apparence linéaire de l'historique. Voici comment réorganiser une branche :

### Basculer sur la branche à réorganiser
```bash
git checkout ma_branche_a_reorganiser
```

### Réorganiser la branche sur la branche cible
```bash
git rebase branche_cible
```

## (5/5) Branches Distantes (Remote Branch)
Les branches distantes suivent les versions du dépôt distant. Pour récupérer (pull) les dernières modifications d'une branche distante :

### Récupérer les modifications d'une branche distante
```bash
git pull origin ma_branche_distante
```

### Créer une nouvelle branche distante
```bash
git push origin ma_branche_locale:ma_branche_distante
```
