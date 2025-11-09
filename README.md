# Neon Reaper Dark Theme

Un thème sombre "Neon + Glass" pour TeamSpeak avec de nombreuses variantes de couleur et un effet glassmorphism personnalisable.

## Caractéristiques
- Base sombre multi-niveaux (valeurs `--custom-value-dark*` de `TeamSpeak.css`).
- Couche **Glassmorphism** (flou + transparence + bordures subtiles) via `Glassmorphism.css`.
- 17 palettes d'accent: Blue, Pink, Purple, Orange, Green, Dark Green, Yellow, Lime, Brown, Cyan, Indigo, Magenta, Amber, Turquoise, Silver, Coral + le thème original.
- Variables centralisées pour modifier rapidement couleurs et rendu du verre.

## Structure
```
package.json
Reaper.css                (thème principal)
Glassmorphism.css         (couche verre partagée)
Blue.css / Pink.css / ... (variantes de couleur)
TeamSpeak.css             (variables et overrides de base)
```
Chaque fichier de palette importe `TeamSpeak.css` puis `Glassmorphism.css` et redéfinit uniquement les variables d'accent.

## Sélection du thème
Dans TeamSpeak (MyTeamSpeak / gestion des thèmes), choisissez le nom correspondant:
- "Reaper Blue", "Reaper Magenta", etc.
Chaque entrée est définie dans `package.json` sous `content.themes`.

## Personnalisation rapide
Ajustez dans le fichier palette choisi (ex: `Blue.css`):
```
--custom-color-accent-light
--custom-color-accent-dark
--custom-color-accent-light-t
--custom-color-accent-dark-t
--custom-color-slider1
--custom-color-slider2
```
Ces variables pilotent boutons, sliders, états actifs, surbrillance.

### Paramètres du glass (dans `Glassmorphism.css`)
```
--glass-blur        (intensité du flou, ex: 16px)
--glass-saturation  (saturation des couleurs sur les surfaces verre)
--glass-shadow      (ombrage de profondeur)
--glass-radius      (arrondi des panneaux)
--glass-bg / --glass-bg-strong (niveaux de transparence)
--glass-border      (bordure subtile)
```
Vous pouvez réduire l'impact performance en diminuant `--glass-blur` ou en commentant les blocs `@supports`.

## Créer une nouvelle variante de couleur
1. Copier un fichier existant (ex: `Blue.css` -> `MyColor.css`).
2. Changer les valeurs hex + rgba des variables accent.
3. Ajouter l'entrée dans `package.json` sous `content.themes`:
```json
{
  "name": "Reaper MyColor",
  "source": "MyColor.css",
  "image": "Reaper.png",
  "apiVersion": 1
}
```
4. Recharger / sélectionner le thème dans TeamSpeak.

## Fallback sans flou
Si `backdrop-filter` n'est pas pris en charge, un fallback plus opaque est automatiquement appliqué (`@supports not (...)`).

## Licence
MIT. Voir le champ `license` dans `package.json`.

## Contribution / idées
- Ajouter un toggle global (ex: `--enable-glass`) pour désactiver la couche verre.
- Générer des icônes dédiées par palette (changer `image` dans `package.json`).
- Ajouter une palette high-contrast (accent très clair + gris profonds).

Bon thème & amusez-vous !
