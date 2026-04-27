# Braze × Sephora — Cycle de vie des profils client

Page web interactive expliquant le modèle d'identité Braze à une audience marketing.

## Contenu

- **Simulateur de parcours** — 4 journeys interactifs (premier achat, multi-appareils, clic email, borne PDV)
- **10 scénarios détaillés** — en langage marketing, sans jargon technique
- **Résolution probabiliste** — section Roadmap 2025–2026
- **Tableau récapitulatif** — tous les scénarios en un coup d'œil

## Déploiement sur Vercel

### Option 1 — Import GitHub (recommandé)

1. Pusher ce repo sur GitHub
2. Aller sur [vercel.com/new](https://vercel.com/new)
3. Importer le repo GitHub
4. Vercel détecte automatiquement le site statique via `vercel.json`
5. Cliquer **Deploy** — terminé en < 30 secondes

### Option 2 — Vercel CLI

```bash
npm i -g vercel
vercel --prod
```

## Structure

```
index.html     # Page principale (auto-contenue, pas de dépendances)
vercel.json    # Configuration déploiement statique
README.md      # Ce fichier
```

## Mise à jour du contenu

Tout le contenu est dans `index.html` dans la section `<script>` :
- `journeys[]` — les 4 parcours du simulateur
- `scenarios[]` — les 10 scénarios détaillés
- `summaryData[]` — le tableau récapitulatif
