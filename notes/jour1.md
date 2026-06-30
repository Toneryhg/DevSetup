# Jour 1 — Installation de l'environnement

## Objectifs du jour

- Installer et configurer VSCode
- Installer Git et Node.js
- Découvrir les bases du terminal

## VSCode

VSCode (Visual Studio Code) est un éditeur de code gratuit et léger. J'ai installé
les extensions recommandées via le fichier `.vscode/extensions.json` du projet :

- **ESLint** — détection d'erreurs JavaScript
- **Prettier** — formatage automatique du code
- **GitLens** — visualisation de l'historique Git dans l'éditeur
- **Live Server** — prévisualisation de pages HTML en local

## Git

Git est un système de contrôle de version. Configuration globale effectuée :

```bash
git config --global user.name "MALONGA Saint Chalbhery"
git config --global user.email "saintmlg@icloud.com"
```

Vérification : `git config --list`

## Node.js

Node.js permet d'exécuter du JavaScript en dehors du navigateur. Version installée : **v24.13.1**.

Vérification : `node --version` et `npm --version`

## Premières commandes terminal

| Commande | Action |
|----------|--------|
| `pwd` | Afficher le dossier courant |
| `ls` / `dir` | Lister les fichiers |
| `cd nomDossier` | Changer de dossier |
| `mkdir nomDossier` | Créer un dossier |
| `code .` | Ouvrir le dossier dans VSCode |

## Réflexion

Comprendre la différence entre le **terminal** (interface texte) et l'**interface graphique**
est essentiel pour un développeur. Le terminal donne un contrôle direct sur le système
et sur les outils comme Git.
