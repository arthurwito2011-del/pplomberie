# Pplomberie – maquette de site

Site statique (HTML + CSS, sans dépendance) pour Pplomberie, plombier à Caen.
Maquette de démonstration : textes et horaires à valider avec l'entreprise.

## Structure

```
pplomberie/
├── index.html
├── css/style.css
├── .nojekyll
├── .gitignore
└── .github/workflows/deploy.yml   # déploiement automatique GitHub Pages
```

## Tester en local

Ouvrez simplement `index.html` dans un navigateur, ou lancez un serveur local :

```bash
python3 -m http.server 8000
# puis http://localhost:8000
```

## Mettre sur GitHub

1. Créez un dépôt vide sur https://github.com/new (par exemple `pplomberie`), sans README.
2. Dans le dossier du projet :

```bash
git init -b main
git add .
git commit -m "Première version du site"
git remote add origin https://github.com/VOTRE-COMPTE/pplomberie.git
git push -u origin main
```

## Déployer sur GitHub Pages

1. Sur GitHub : **Settings → Pages → Build and deployment → Source : GitHub Actions**.
2. Chaque `git push` sur `main` redéploie le site automatiquement (onglet **Actions** pour suivre).
3. Le site est publié sur `https://VOTRE-COMPTE.github.io/pplomberie/`.

Pour un domaine personnalisé : **Settings → Pages → Custom domain**, puis configurez le DNS chez votre registrar.

## À faire avant mise en ligne réelle

- Valider textes, horaires et zone d'intervention avec l'entreprise
- Intégrer le plan Google Maps (iframe)
- Retirer le bandeau « Maquette de démonstration »
