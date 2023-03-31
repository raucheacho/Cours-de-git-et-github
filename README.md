# Résumé sur Git et GitHub

![le resumé de git et git hub](affiche%20git%20github.png)

## L'outil Git

Git est un système de gestion de versions de code source distribué. Il permet de suivre les modifications apportées à un projet et de collaborer avec d’autres personnes sur un même code source.

> Pour utiliser Git, il faut d’abord initialiser un nouveau projet avec “git init”, ajouter des fichiers à l’index avec “git add”, puis enregistrer les modifications avec “git commit”. On peut ensuite partager le code sur GitHub en créant un nouveau repository, en y ajoutant les fichiers avec “git remote add” et “git push”.

## Le site GitHub

GitHub est une plateforme de développement collaboratif basée sur Git. Elle permet aux développeurs de partager leur code source, de collaborer avec d'autres personnes sur des projets, de contribuer à des projets open source, de suivre les problèmes et les demandes d'amélioration, et de créer des branches et des pull requests pour proposer des modifications de code.

GitHub permet également de gérer les problèmes et les demandes d'amélioration avec son système de tickets. Les développeurs peuvent créer des branches pour travailler sur des fonctionnalités spécifiques, puis proposer leurs modifications en créant une pull request. Les autres membres de l'équipe peuvent alors commenter la demande de fusion, effectuer des révisions et finalement fusionner la branche dans la version principale du code source.

## Commande de base de git

Voici quelques commandes GIT de base que vous devez connaître :

1.Comment configurer git config
**git config:-** Peut être utilisé pour définir des valeurs de configuration spécifiques à l’utilisateur telles que le nom d’utilisateur, l’e-mail, le format de fichier, etc.

- Définir un nom d’utilisateur qui est identifiable pour le crédit lors de l’historique des versions de révision.

```bash
git config --global user.name
```

- Définir une adresse e-mail qui sera associée à chaque marqueur d’historique

```
  git config —global user.email
```

- Définir la coloration automatique de la ligne de commande pour Git pour une révision facile.

```bash
git config —global color.ui auto
```

- git init:- Initialiser un répertoire existant en tant que repository Git [ la commande Git suivante créera un repository dans le répertoire actuel ]

```bash
git init
```

- Récupérer un repository entier à partir d’un emplacement hébergé à partir de URL

```bash
git clone [url]
```

2.Git Stage & Snapshot

- **git status:-** Afficher les fichiers modifiés dans le répertoire de travail, mis en scène pour votre prochain commit

```bash
git status
```

- Ajoutez un fichier tel qu’il apparaît maintenant à votre prochain commit (stage)

```bash
git add [file]
```

- retrait d’un fichier tout en conservant les modifications dans le répertoire de travail.

```bash
git reset [file]
```

- Diff de ce qui est changé mais pas pris en compte par git

```bash
git diff
```

- Diff de ce qui est changé et pris en compte par git

```bash
git diff —staged
```

- Valider votre contenu pris en compte par git en tant que nouvel Snapshot.

```bash
git commit -m “commentez le travail que vous avez fait“
```

3.Branche et fusion de branche

Isoler le travail dans les branches, changer le contexte et intégrer les changements

- Listez vos branches. un \* apparaîtra à côté de la branche actuellement active

```bash
git branch
```

- Créer une nouvelle branche à la validation actuelle

```bash
git branch [branch name]
```

- Passez à une autre branche et utilisez-la dans votre répertoire de travail

```bash
git checkout
```

- Fusionner l’historique de la branche spécifiée dans l’historique actuel

```bash
git merge [branch]
```

- Afficher tous les commits dans l’historique de la branche actuelle

```bash
git log
```

4.Inspection & Comparaison

Examiner les journaux, des différences et des informations sur les objets

- Afficher tous les commits dans l’historique de la branche actuelle.

```bash
git log
```

- Afficher les commits sur branchA qui ne sont pas sur brancheB

```bash
git log brancheB..brancheA
```

- Montrer les validations qui ont changé le fichier, même à travers les renommages

```bash
git log —follow [file]
```

- Montrer la différence de ce qui se trouve dans la branche A qui n’est pas dans la branche B

```bash
git diff brancheB...brancheA
```

- Montrer n’importe quel objet dans Git dans un format lisible par l’homme

```bash
git show [SHA]
```

5.Partager et mettre à jour

Récupération des mises à jour d’un autre dépôt et mise à jour du dépôt local

- Ajouter une URL git en tant qu’alias

```bash
git remote add [alias] [url]
```

- Fusionner une branche distante dans votre branche actuelle pour la mettre à jour

```bash
git merge [alias]/[branch]
```

- Récupérer toutes les branches de ce dépôt distant Git

```bash
git fetch [alias]
```

- Transmettre les commits de branche locale à la branche du dépôt distant

```bash
git push [alias] [branch]
```

- Récupérer et fusionner tous les commits de la branche distante de suivi

```bash
git pull
```

6. Commits temporaires Git

Stocker temporairement les fichiers modifiés et suivis afin de changer de branche

- Enregistrer let organiser es modifications

```bash
git stash
```

- liste l'ordre de pile des modifications de fichiers.

```bash
git stash list
```

- écrire les changements du haut de la pile de réserve.

```bash
git stash pop
```

- Supprimer les changements du haut de la pile de réserve.

```bash
git stash drop
```

7. Modifications du chemin de suivi Git

Suppression de fichier de gestion des versions et changement du chemin.

- Supprimer le fichier du projet et organiser la suppression pour la validation.

```bash
git rm [file]
```

- Modifier le chemin d’un fichier existant et organiser le déplacement

```bash
git mv [existing-path] [new-path]
```

- Afficher tous les journaux de validation avec indication de tous les chemins qui ont été déplacés

```bash
git log —stat -M
```

**Comment annuler un ancien commit dans Git:**

Vous pouvez annuler un ancien commit en utilisant son identifiant de commit. Cela ouvre l’éditeur afin que vous puissiez ajouter un message de validation.

```bash
git revert [commit id here]
```

Comment supprimer une branche dans Git :

Vous pouvez supprimer une branche en utilisant la commande ci-dessous :

```bash
git branch -d [branch name]
```

### Rauche Acho

- @raucheacho, on #facebook, #youtube, #tweeter, #Instagram, #LinkedIn, [www.raucheacho.com](https://www.raucheacho.com)
- Développeur, formateur et entrepreneur
