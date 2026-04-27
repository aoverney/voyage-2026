# Site voyage Pérou-Bolivie-Chili sept 2026

Site web statique pour partager le voyage avec maman.

## Test local

```bash
# Ouvrir dans le navigateur (macOS / Linux)
xdg-open index.html  # Linux
open index.html       # macOS
```

Ou simple double-clic sur `index.html`.

## Déploiement GitHub Pages

1. Créer un repo public GitHub (par ex. `voyage-2026`)
2. Push le contenu de ce dossier :

```bash
cd /home/arnaud/voyage-perou-bolivie-2026/site
git init
git add .
git commit -m "Initial site voyage AmSud sept 2026"
git branch -M main
git remote add origin https://github.com/<username>/voyage-2026.git
git push -u origin main
```

3. Activer Pages : **Settings → Pages → Source: Deploy from a branch → Branch: main / root → Save**
4. Attendre 1-2 min, l'URL apparaît : `https://<username>.github.io/voyage-2026/`
5. Partager le lien à maman

## Mise à jour du site

Modifier `index.html`, puis :

```bash
git add .
git commit -m "Update site"
git push
```

Le site se redéploie automatiquement en 1-2 min.

## Structure

- `index.html` : page unique autonome (CSS embarqué, polices Google Fonts via CDN)
- Pas de build, pas de dépendances, pas de framework
- Mobile-friendly responsive
