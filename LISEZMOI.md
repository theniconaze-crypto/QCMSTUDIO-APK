# QCM Studio – application Android

Le fichier `www/index.html` est votre QCM_Studio_final.html (à remplacer à chaque mise à jour).

## Obtenir l'APK sans installer Android Studio (GitHub Actions)
1. Créez un dépôt GitHub (privé possible) et envoyez-y tout le contenu de ce dossier (y compris `.github`).
2. Onglet **Actions** > « Build APK Android » > le build démarre seul (ou « Run workflow »).
3. À la fin, ouvrez l'exécution et téléchargez l'artefact **QCM-Studio-apk** (zip contenant `app-debug.apk`).
4. Copiez l'APK sur le téléphone et ouvrez-le (autoriser « Sources inconnues » pour le navigateur/gestionnaire de fichiers).

## Avec Android Studio
`npm install`, `npx cap sync android`, puis `npx cap open android` > Build > Build APK(s).

## Important : liens envoyés aux candidats
Dans l'application, l'adresse interne est `https://localhost`. Au moment de générer un lien, l'appli demande donc
l'adresse web où `QCM_Studio_final.html` est hébergé (GitHub Pages, Firebase Hosting, site de l'entreprise…).
Les candidats ouvrent le lien dans leur navigateur : le fichier doit donc aussi être publié quelque part.
