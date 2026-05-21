# Click Bible Challenge

Application web de suivi quotidien de lecture de la Bible avec comparaison de temps d'ecran (reseaux sociaux). L'application s'appuie sur une authentification Google et un stockage en temps reel sur Firebase.

## Fonctionnalites principales

- **Authentification** : Connexion et deconnexion via Google Accounts.
- **Verset et Lecture du jour** : Affichage dynamique de la lecture recommandee selon un calendrier predefini dans l'application (du 12/05/2025 au 31/07/2025).
- **Formulaire de suivi quotidien** :
  - Saisie de la date et du passage lu.
  - Saisie du temps passe sur les réseaux sociaux.
  - Choix du mode de lecture (seul, avec quelqu'un, en groupe).
  - Zone de notes textuelles pour enregistrer ses pensees ou resumes.
- **Historique en temps reel** : Affichage, modification et suppression des entrees passees associees a l'utilisateur connecte.

## Technologies utilisees

- **Frontend** : HTML5, CSS3 (Police Nunito), Vanilla JavaScript
- **Backend et Database** : Firebase Web SDK (v7)
  - **Firebase Authentication** : Gestion des sessions utilisateurs
  - **Cloud Firestore** : Stockage NoSQL temps reel des entrees de lecture

## Structure des fichiers

- `index.html` : Structure de l'interface utilisateur et integration des scripts.
- `style.css` : Mise en page et style visuel general de l'application.
- `index.js` : Calendrier de lecture predefini et logique d'affichage de la lecture du jour.
- `firebase.js` : Initialisation de l'application Firebase et gestion de l'authentification Google.
- `form.js` : Gestion de la soumission du formulaire, requetes Firestore (CRUD) et affichage dynamique de l'historique des lectures.

## Installation et Lancement local

1. Clonez le depot sur votre machine locale.
2. Configurez votre projet Firebase et remplacez les cles de configuration dans `firebase.js`.
3. Lancez un serveur local pour executer l'application (par exemple avec l'extension VS Code Live Server ou `python3 -m http.server 8000`).
