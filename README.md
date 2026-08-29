# Wake - GPS Minimal PWA

Une Progressive Web App (PWA) de navigation GPS ultra-minimaliste, fluide et sobre, conçue pour mobile (iOS/Safari & Android) et prête à être déployée sur **GitHub Pages**.

---

## 🧭 Fonctionnalités

- **Interface 100% épurée** : Carte plein écran (Leaflet + OpenStreetMap), sans boutons superflus.
- **Marqueur GPS précis** : Point bleu franc avec bordure blanche nette et indicateur de cap/orientation.
- **Tracé d'Itinéraire OSRM** : Ligne bleue épaisse et contrastée calculée via l'API publique OSRM au simple clic/toucher sur la carte ou via recherche.
- **Suivi en temps réel** : `watchPosition` haute précision avec actualisation automatique du trajet et bouton de recentrage.
- **Écran allumé en continu** : Utilise l'API Screen Wake Lock pour éviter la mise en veille pendant les trajets.
- **100% PWA & iOS Safari** : Compatible "Ajouter à l'écran d'accueil", icônes haute résolution et Service Worker pour le fonctionnement hors-ligne / app shell.

---

## 🚀 Déploiement sur GitHub Pages (Gratuit & HTTPS)

> **Important** : L'API de géolocalisation et les Service Workers nécessitent obligatoirement une connexion sécurisée **HTTPS** (fournie gratuitement par GitHub Pages).

### Étape 1 : Créer un dépôt sur GitHub
1. Rendez-vous sur [github.com/new](https://github.com/new).
2. Nommez le dépôt (ex: `wake` ou `wake-gps`).
3. Choisissez **Public** et créez le dépôt.

### Étape 2 : Publier les fichiers
Dans votre terminal local, placez-vous dans ce dossier et exécutez :
```bash
git init
git add .
git commit -m "Initial commit - Wake GPS"
git branch -M main
git remote add origin https://github.com/<votre-utilisateur>/<votre-depot>.git
git push -u origin main
```

### Étape 3 : Activer GitHub Pages
1. Sur la page de votre dépôt GitHub, cliquez sur **Settings** (Paramètres).
2. Dans le menu de gauche, cliquez sur **Pages**.
3. Sous **Branch**, sélectionnez `main` et le dossier `/(root)`, puis cliquez sur **Save**.
4. Patientez ~1 minute : votre PWA sera accessible à l'adresse :  
   `https://<votre-utilisateur>.github.io/<votre-depot>/`

---

## 📱 Installation sur iPhone (iOS / Safari)

1. Ouvrez l'URL GitHub Pages dans **Safari** sur votre iPhone.
2. Appuyez sur le bouton **Partager** (icône rectangle avec flèche vers le haut au bas de Safari).
3. Faites défiler vers le bas et sélectionnez **Sur l'écran d'accueil** (ou *Add to Home Screen*).
4. Nommez-le "Wake" et validez.
5. L'application s'ouvre désormais en plein écran sans les barres du navigateur !
