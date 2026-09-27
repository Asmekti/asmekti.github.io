# Asmekti Learn — ⴰⵙⵎⴽⵜⵉ

Application de rappel de cours pour les stagiaires OFPPT (ISIA Agadir) : français / العربية, fonctionne sans Internet après la première ouverture.

## Publier sur GitHub Pages (une seule fois)

**Avec git (recommandé)**
```bash
cd asmekti-pwa
git init && git add . && git commit -m "Asmekti Learn — module Microbiologie"
git branch -M main
git remote add origin https://github.com/VOTRE_COMPTE/asmekti.git
git push -u origin main
```
Puis sur GitHub : **Settings → Pages → Source : Deploy from a branch → main / (root) → Save**.
Après 1 à 2 minutes, l'app est en ligne : `https://VOTRE_COMPTE.github.io/asmekti/`

**Sans git (glisser-déposer sur github.com)** — GitHub accepte 100 fichiers par envoi, donc en 3 fois :
1. Créer le dépôt public `asmekti`, puis « uploading an existing file » : glisser `index.html`, `sw.js`, `manifest.webmanifest`, `favicon.ico`, `.nojekyll` et le dossier `icons` → Commit.
2. « Add file → Upload files » : glisser les dossiers `img/A` et `img/B` → Commit.
3. Même chose avec `img/C` et `img/D` → Commit.

⚠️ Le fichier `.nojekyll` est caché sur Mac/Windows : l'afficher avant de glisser (il n'est pas obligatoire, mais il accélère la publication).

## Mettre à jour
1. Changer `VERSION` / `VDATE` et ajouter une entrée en tête de `NEWS` (fichier `news.py` du générateur).
2. Pour un module ou une séance ajoutés, lui donner `"since": "<nouvelle version>"` → étiquette « Nouveau » chez les stagiaires qui avaient une version plus ancienne.
3. Régénérer, remplacer les fichiers, puis `git add . && git commit -m "Version x.y" && git push`.

Côté stagiaire : à l'ouverture avec Internet, la nouvelle version se télécharge en arrière-plan, un bandeau « Nouvelle version disponible — Mettre à jour » apparaît, puis la fenêtre « Quoi de neuf ? » (FR / ع) s'affiche une seule fois. La progression est conservée.

## Côté stagiaire
- **Android (Chrome)** : ouvrir le lien → menu ⋮ → « Installer l'application ».
- **iPhone (Safari)** : ouvrir le lien → Partager → « Sur l'écran d'accueil ».
Attendre quelques secondes sur la première page (wifi conseillé, ~11 Mo) : ensuite l'app marche hors ligne.
