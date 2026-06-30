# DevSetup

Ce repository documente la mise en place de mon environnement de développement
dans le cadre de ma formation (Phase 1 · Module 0 · Semaine 1).

## Contenu

- Configuration de VSCode, Git et Node.js
- Notes d'apprentissage dans le dossier `notes/`
- Configuration de développement (Nodemon, EditorConfig, extensions VSCode)

## Comment utiliser ce repo

1. **Cloner** le dépôt :
   ```bash
   git clone https://github.com/Toneryhg/DevSetup.git
   cd DevSetup
   ```

2. **Ouvrir** le dossier avec VSCode (ou Cursor) :
   ```bash
   code .
   ```

3. **Installer les extensions recommandées** lorsque VSCode vous le propose
   (fichier `.vscode/extensions.json`).

4. **Consulter les notes** dans le dossier `notes/` pour suivre ma progression
   jour par jour.

5. **Lancer le script de développement** (bonus Nodemon) :
   ```bash
   npm install
   npm run dev
   ```

## Outils installés

| Outil    | Version vérifiée |
|----------|------------------|
| VSCode   | Installé         |
| Git      | 2.53.0           |
| Node.js  | v24.13.1         |

## Commandes Git utilisées

| Commande | Description |
|----------|-------------|
| `git init` | Initialiser un dépôt local |
| `git add .` | Ajouter les fichiers au staging |
| `git commit -m "message"` | Enregistrer un snapshot |
| `git push -u origin main` | Envoyer les commits sur GitHub |
| `git checkout -b dev` | Créer et basculer sur une branche |
| `git merge dev` | Fusionner la branche dev dans main |

## Structure du projet

```
DevSetup/
├── .editorconfig
├── .gitignore
├── .vscode/extensions.json
├── README.md
├── package.json
├── index.js
└── notes/
    ├── jour1.md
    ├── jour2.md
    └── jour3.md
```

## Bonus réalisés

- **Nodemon** : rechargement automatique avec `npm run dev`
- **EditorConfig** : conventions de formatage partagées (`.editorconfig`)
- **Branche dev** : créée, développée puis fusionnée dans `main`

## Auteur

MALONGA Saint Chalbhery — SEMAINE 1 — Environnement & Outils
