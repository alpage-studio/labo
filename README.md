# Labo de série

Un look pour toute la pellicule, une correction propre à chaque photo.

- **Importer** toute une série d'un coup (JPEG, PNG, WebP, ou RAW via l'aperçu intégré).
- **Choisir un look** dans la bande du haut : chaque look est montré sur ta propre photo.
- **Enregistrer** : sur téléphone, une seule feuille de partage envoie toutes les photos vers la galerie ; sur ordinateur, un ZIP ou des fichiers séparés.

Tout se calcule sur l'appareil. Aucune photo n'est envoyée. Fonctionne hors ligne une fois installée.

## Fichiers

| Fichier | Rôle |
|---|---|
| `index.html` | toute l'application (HTML, CSS, JS) |
| `manifest.webmanifest` | nom, icônes, mode plein écran pour l'installation |
| `sw.js` | hors ligne ; **monter `VERSION` à chaque publication** |
| `jszip.min.js` | JSZip 3.10.1 (MIT), pour l'export ZIP |
| `icon-*.png`, `apple-touch-icon.png` | icônes |

## Publier sur GitHub Pages

1. Sur github.com, compte `alpage-studio` : **New repository** → nom `labo`, Public, sans README.
2. Pousser ce dossier sur `main` :
   ```
   git remote add origin https://github.com/alpage-studio/labo.git
   git push -u origin main
   ```
3. Dans le dépôt : **Settings → Pages → Source : Deploy from a branch → `main` / `(root)`** → Save.
4. Une à deux minutes plus tard : `https://alpage-studio.github.io/labo/`

## Installer sur le téléphone

- **iPhone (Safari)** : ouvrir l'adresse → bouton Partager → **Sur l'écran d'accueil**.
- **Android (Chrome)** : ouvrir l'adresse → menu ⋮ → **Installer l'application**.

## Mettre à jour

Modifier les fichiers, monter `VERSION` dans `sw.js`, commiter, pousser. L'application se met à jour à la prochaine ouverture en ligne.
