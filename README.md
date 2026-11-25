# Courses Famille

Application mobile de listes de courses familiales, publiée avec GitHub Pages.

## Fonctionnalités

- listes partagées et mises à jour en temps réel avec Firebase Firestore ;
- profils famille, commentaires, archives et réutilisation de listes ;
- installation sur l’écran d’accueil grâce au manifeste PWA ;
- cache hors ligne de l’interface via un service worker.

## Configuration Firebase

Le site attend un projet Firebase avec :

1. une application Web ;
2. Authentication avec la méthode « Anonyme » activée ;
3. Cloud Firestore ;
4. des règles autorisant uniquement les utilisateurs authentifiés à lire et écrire les données de l’application.

La configuration Web Firebase doit être copiée dans `FIREBASE_USER_CONFIG` dans `index.html`.
Les règles prêtes à déployer se trouvent dans `firestore.rules`.

## Publication

GitHub Pages doit servir la branche `main` depuis la racine du dépôt.
