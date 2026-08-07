# Galaga Legacy 2

**La suite enrichie de Galaga Legacy : boucliers, tir double, tir rapide.**

Joue ici : [games.hylst.fr/galagalegacy2/](https://games.hylst.fr/galagalegacy2/)

![Galaga Legacy 2](og-image.png)

## Comment on joue

Même principe que Galaga Legacy (vagues d'ennemis en formation, tir vertical), avec un
système de power-ups plus développé : tir rapide, bouclier temporaire, tir double.

## Contrôles

| Action | Effet |
|--------|-------|
| Flèches gauche/droite ou A/D (Q/D en AZERTY) | Déplacer le vaisseau |
| Espace | Tirer |
| Tactile | Glisser pour se déplacer, tapoter pour tirer |
| Bouton « ℹ️ Infos » | Stack technique, graphismes, algorithmes |

## Ce qu'il y a dedans

- Vagues d'ennemis en formation, patterns d'attaque à la Galaga
- 3 power-ups : tir rapide, bouclier temporaire, tir double
- Rendu Canvas 2D, boucle de jeu en `requestAnimationFrame`
- Musique et effets sonores synthétisés (Web Audio API)

## L'arborescence

```
galaga-style-arcade-shooter-2-game-development/
├── index.html          # template + bloc SEO
├── vite.config.ts      # base '/galagalegacy2/' + singlefile
├── og-image.png
├── public/
└── src/
    ├── main.tsx
    ├── App.tsx          # UI, montage du Canvas
    ├── game/Game.ts      # boucle de jeu, entités, power-ups, collisions
    ├── index.css
    └── utils/cn.ts
```

## Dev

```bash
npm install
npm run dev       # http://localhost:5173/
npm run build     # dist/index.html, un seul fichier
npm run preview
```

## Stack

React 19, TypeScript 5.9 (strict), Tailwind CSS 4, Vite 7, vite-plugin-singlefile.

## Licence

MIT, Geoffroy Streit (Hylst)
