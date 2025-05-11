# Site Web de la Jeunesse Ouvrière Chrétienne (JOC)

Ce projet est un site web pour la Jeunesse Ouvrière Chrétienne, avec un design utilisant les couleurs vert et blanc, un arrière-plan de verdure, et un espace administrateur pour gérer les événements.

## Fonctionnalités
- Page d'accueil avec présentation de la JOC
- Section "À propos"
- Liste des événements (ajout/suppression via l'espace admin)
- Formulaire de contact
- Espace administrateur (mot de passe : `joc2025`)
- Design responsive avec couleurs vert (#27ae60, #219653) et blanc
- Arrière-plan de verdure

## Instructions d'installation
1. Téléchargez et décompressez le fichier ZIP.
2. Placez les fichiers dans un dossier sur votre ordinateur.
3. Lancez un serveur local pour tester le site :
   - Avec Python : `python -m http.server 8000`
   - Avec Node.js : `npx serve`
   - Ou utilisez une extension comme "Live Server" dans VS Code
4. Ouvrez votre navigateur et accédez à `http://localhost:8000`.

## Accès à l'espace administrateur
1. Cliquez sur le lien "Administration" dans la navigation.
2. Entrez le mot de passe `joc2025` (sensible à la casse, sans espaces).
3. Une fois connecté, vous pouvez ajouter ou supprimer des événements.

## Personnalisation
- **Arrière-plan** : Pour changer l'image de verdure, modifiez l'URL dans le CSS (`body { background-image: url('votre-image.jpg') }`) ou placez une image dans le dossier `assets` et mettez à jour le chemin.
- **Couleurs** : Modifiez les codes hexadécimaux (#27ae60, #219653, #f0f9f4) dans le CSS pour ajuster les teintes.
- **Contenu** : Éditez le texte dans `index.html` pour personnaliser les sections.

## Hébergement
Pour déployer le site :
- Utilisez un service comme GitHub Pages, Netlify, ou Vercel.
- Téléversez les fichiers dans le répertoire racine du serveur.
- Assurez-vous que l'image de fond est accessible (URL publique ou hébergée avec le site).

## Dépannage
- **Mot de passe non fonctionnel** : Vérifiez la casse (`joc2025`), utilisez un serveur local (pas `file://`), et ouvrez la console du navigateur (F12 > Console) pour les erreurs.
- **Section admin non visible** : Vérifiez que le lien "Administration" fonctionne et que `.admin-login` n'a pas `display: none` dans l'inspecteur d'éléments.
- **Erreurs JavaScript** : Effacez `localStorage` (`localStorage.clear()` dans la console) et rechargez la page.

## Remarques
- Ce projet utilise `localStorage` pour stocker les événements, ce qui est local au navigateur. Pour une solution persistante, envisagez un backend (par exemple, Node.js + MongoDB).
- Le mot de passe (`joc2025`) est codé en dur. Pour plus de sécurité, implémentez un système d'authentification (par exemple, Firebase Auth).

Pour toute question ou personnalisation supplémentaire, contactez l'auteur du projet.  terminer
