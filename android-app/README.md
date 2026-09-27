# Asmekti — app Android

Ce dossier sert uniquement à fabriquer l'app Android (APK) avec Capacitor.
Rien à faire à la main : à chaque `git push` qui change `version.json`, GitHub Actions
(`.github/workflows/android.yml`) copie le site, fabrique l'APK, le signe et le publie dans
**Releases** sous le nom `Asmekti.apk`.

Lien de téléchargement permanent :
https://github.com/Asmekti/asmekti.github.io/releases/latest/download/Asmekti.apk

Secrets GitHub nécessaires (Settings → Secrets and variables → Actions) :
- `ANDROID_KEYSTORE_B64` : la clé de signature (fichier texte fourni à part, ne jamais la publier)
- `ANDROID_KEYSTORE_PASS` : son mot de passe
