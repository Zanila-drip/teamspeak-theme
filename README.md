# Reaper — Neon Dark + Glass

![Aperçu du thème](Thumbnail.png)

Un thème TeamSpeak sombre avec accents néon et effet "verre" (glassmorphism).

## Ce que ça fait (version courte)
- Fond sombre + couleurs d’accent (bleu, rose, violet, orange, vert, etc.).
- Effet verre: flou + transparence + bordure douce sur les panneaux (si supporté par votre système). 
- Plusieurs variantes prêtes à l’emploi: "Reaper Blue", "Reaper Magenta", "Reaper Indigo", etc.

## Installer / Utiliser
1) Téléchargez ce dossier (ou le .zip) du thème.
2) TeamSpeak → Settings → Appearance → Themes → Importer (ou copiez le dossier dans le répertoire de thèmes de TeamSpeak).
3) Redémarrez TeamSpeak si nécessaire.
4) Dans la liste, sélectionnez la variante voulue (ex: "Reaper Blue").

## Personnaliser vite fait
- Couleur: ouvrez la variante (ex: `Blue.css`) et changez les variables:
  `--custom-color-accent-light`, `--custom-color-accent-dark` (+ versions `-t`), `--custom-color-slider1/2`.
- Verre: dans `Glassmorphism.css`, ajustez `--glass-blur` (flou), `--glass-radius` (arrondi), `--glass-bg` (transparence).

Notes:
- Si le flou (`backdrop-filter`) n’est pas supporté, un rendu sans flou s’applique automatiquement.
- Sur machines modestes, diminuez `--glass-blur` pour de meilleures perfs.

Licence: MIT.

---

# Reaper — Neon Dark + Glass (EN)

Dark TeamSpeak theme with neon accents and a subtle “glass” (glassmorphism) effect.

## What it does (short)
- Dark base + accent colors (blue, pink, purple, orange, green, etc.).
- Glass effect: blur + transparency + soft border on panels (if supported by your system).
- Many ready-to-use variants: "Reaper Blue", "Reaper Magenta", "Reaper Indigo", and more.

## Install / Use
1) Download this folder (or the theme .zip).
2) TeamSpeak → Settings → Appearance → Themes → Import (or copy the folder into TeamSpeak’s themes directory).
3) Restart TeamSpeak if needed.
4) In the list, pick your variant (e.g. "Reaper Blue").

## Quick customize
- Color: open the chosen variant (e.g. `Blue.css`) and tweak variables:
  `--custom-color-accent-light`, `--custom-color-accent-dark` (+ `-t` versions), `--custom-color-slider1/2`.
- Glass: in `Glassmorphism.css`, adjust `--glass-blur` (blur), `--glass-radius` (roundness), `--glass-bg` (transparency).

Notes:
- If `backdrop-filter` isn’t supported, a no-blur fallback is applied automatically.
- On lower-end machines, reduce `--glass-blur` for better performance.

License: MIT.
