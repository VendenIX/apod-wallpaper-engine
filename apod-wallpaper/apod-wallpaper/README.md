# NASA APOD Wallpaper pour Wallpaper Engine

Ce wallpaper affiche automatiquement la photo astronomique du jour (APOD)
de la NASA et se met à jour quotidiennement.

## 📦 Installation

### Étape 1 : Obtenir une clé API NASA (gratuit, 2 min)

1. Rendez-vous sur https://api.nasa.gov/
2. Remplissez le formulaire "Generate API Key" (First Name, Last Name, Email)
3. La clé est envoyée immédiatement par email (format : 40 caractères)

⚠️ La clé "DEMO_KEY" fonctionne mais est limitée à 30 requêtes/heure pour
toute la planète, donc très peu fiable. Prenez la vôtre.

### Étape 2 : Installer le wallpaper

**Méthode A — Dossier myprojects (recommandée)**

1. Ouvrez Steam et trouvez Wallpaper Engine dans votre bibliothèque
2. Clic droit → Gérer → Parcourir les fichiers locaux
3. Ouvrez le dossier `projects/myprojects/`
   (si `myprojects` n'existe pas, créez-le)
4. Copiez le dossier `apod-wallpaper` entier dedans
5. Redémarrez Wallpaper Engine
6. Le wallpaper apparaît dans "Installed" / "Workshop" → onglet vos créations

**Méthode B — Via l'éditeur Wallpaper Engine**

1. Lancez Wallpaper Engine → bouton "Open Wallpaper Editor"
2. "Create Wallpaper" → choisissez "Web"
3. Sélectionnez le fichier `index.html` de ce dossier
4. Sauvegardez le projet

### Étape 3 : Configuration

Une fois le wallpaper sélectionné, cliquez sur "Personnaliser" à droite :

- **Clé API NASA** : collez votre clé ici (remplace DEMO_KEY)
- **Afficher le panneau d'info** : ON/OFF pour le titre et description
- **Utiliser l'image HD** : utilise la version haute résolution
- **Langue de la date** : Français ou Anglais

## 🔄 Comment ça marche

- Au démarrage, le wallpaper récupère l'image APOD du jour
- Il vérifie toutes les heures si une nouvelle image est disponible
- Si l'APOD du jour est une vidéo, il utilise la miniature
- L'image HD peut faire plusieurs Mo, prévoyez une bonne connexion

## 🐛 Dépannage

**"Erreur : 403" ou "429"** → Votre clé API est invalide ou a dépassé
la limite (DEMO_KEY). Utilisez votre propre clé.

**Image noire / pas d'image** → Ouvrez la console (F12 dans l'éditeur
Wallpaper Engine) pour voir les erreurs détaillées.

**Le panneau d'info ne s'affiche pas** → Vérifiez l'option "Afficher
le panneau d'info" dans les paramètres.

## 📝 Fichiers

- `index.html` — le wallpaper lui-même (HTML/CSS/JS)
- `project.json` — métadonnées pour Wallpaper Engine
- `preview.jpg` — aperçu affiché dans la bibliothèque

Bon ciel étoilé ! 🌌
