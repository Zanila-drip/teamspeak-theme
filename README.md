# Reaper — Neon Dark + Glass

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
