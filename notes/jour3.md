# Jour 3 — Maîtriser les bases de Git

## Objectifs du jour

- Maîtriser les commandes Git essentielles
- Créer le repository DevSetup
- Pousser le premier commit sur GitHub

## Les 4 commandes fondamentales

### 1. `git init`
Initialise un dépôt Git dans le dossier courant. Crée le dossier caché `.git`
qui stocke tout l'historique.

### 2. `git add`
Ajoute des fichiers à la **zone de staging** (préparation du prochain commit).

```bash
git add fichier.md      # un fichier
git add .               # tous les fichiers modifiés
```

### 3. `git commit`
Enregistre un snapshot permanent avec un message descriptif.

```bash
git commit -m "docs: ajouter les notes du jour 1"
```

### 4. `git push`
Envoie les commits locaux vers le dépôt distant (GitHub).

```bash
git push -u origin main
```

## Workflow Git utilisé pour ce projet

```
Modifier des fichiers
       ↓
   git add .
       ↓
git commit -m "message"
       ↓
  git push origin main
```

## Historique de ce repo

Pour garder un historique propre (critère d'évaluation : 3+ commits), j'ai séparé
les modifications en commits logiques :

1. Structure initiale (README + .gitignore)
2. Notes du jour 1
3. Notes des jours 2 et 3
4. Configuration dev (bonus) sur la branche `dev`
5. Merge de `dev` dans `main`

## Branches

- **main** : branche principale, code stable
- **dev** : branche de développement pour les ajouts bonus

```bash
git checkout -b dev    # créer et basculer sur dev
git checkout main      # revenir sur main
git merge dev          # fusionner dev dans main
```

## Commandes utiles supplémentaires

| Commande | Description |
|----------|-------------|
| `git status` | Voir l'état des fichiers |
| `git log --oneline` | Historique compact |
| `git remote -v` | Voir les dépôts distants |
| `git diff` | Voir les modifications non commitées |

## Réflexion

Git est l'outil le plus important d'un développeur. Il permet de :
- **Sauvegarder** chaque étape du travail
- **Revenir en arrière** si quelque chose casse
- **Collaborer** sans écraser le travail des autres
- **Prouver** sa progression (portfolio sur GitHub)

Un bon message de commit est court, en anglais ou français, et décrit **pourquoi**
la modification a été faite, pas seulement **quoi** a changé.
