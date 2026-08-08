# Site voyage Pérou-Bolivie-Chili sept 2026

Site web statique pour partager le voyage avec le groupe (mamie, Nina, David).

> 📌 **C'est la source de vérité du voyage.** Les fichiers `.md` du dossier parent sont des vues
> opérationnelles alignées sur ce site. En cas de divergence, c'est `index.html` qui a raison.

## Test local

```bash
# Ouvrir dans le navigateur (macOS / Linux)
xdg-open index.html  # Linux
open index.html       # macOS
```

Ou simple double-clic sur `index.html`.

## Déploiement GitHub Pages

✅ **Déjà en place** : repo [github.com/aoverney/voyage-2026](https://github.com/aoverney/voyage-2026),
GitHub Pages actif sur `main` / root. Le lien est partagé avec le groupe.

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
