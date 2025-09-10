# Instructions pour GitHub Pages

## Étapes pour publier votre site sur GitHub

### 1. Créer un Repository GitHub

1. Connectez-vous à GitHub (https://github.com)
2. Cliquez sur le bouton "New" ou "+" pour créer un nouveau repository
3. Nommez votre repository (ex: `medieval-website` ou `mon-site-auteur`)
4. Cochez "Public" pour que le site soit accessible
5. Cliquez sur "Create repository"

### 2. Uploader les Fichiers

**Option A : Interface Web GitHub**
1. Dans votre nouveau repository, cliquez sur "uploading an existing file"
2. Glissez-déposez tous les fichiers de votre dossier `website`
3. Ajoutez un message de commit (ex: "Premier upload du site")
4. Cliquez sur "Commit changes"

**Option B : Git en ligne de commande**
```bash
git clone https://github.com/votre-username/nom-du-repository.git
cd nom-du-repository
# Copiez tous les fichiers du dossier website ici
git add .
git commit -m "Premier upload du site"
git push origin main
```

### 3. Activer GitHub Pages

1. Dans votre repository, allez dans l'onglet "Settings"
2. Descendez jusqu'à la section "Pages" dans le menu de gauche
3. Dans "Source", sélectionnez "Deploy from a branch"
4. Choisissez "main" comme branche
5. Laissez "/ (root)" comme dossier
6. Cliquez sur "Save"

### 4. Accéder à votre Site

Après quelques minutes, votre site sera accessible à :
`https://votre-username.github.io/nom-du-repository`

## Personnalisation du Site

### Modifier les Textes

- **Page d'accueil** : Éditez `index.html`
- **Personnages** : Modifiez `pages/personnages.html`
- **Extraits** : Changez le contenu dans `pages/extraits.html`
- **Livres** : Mettez à jour `pages/livres.html`
- **Contact** : Personnalisez `pages/contact.html`

### Ajouter des Images

1. Créez un dossier `images` dans votre repository
2. Uploadez vos images dans ce dossier
3. Référencez-les dans le HTML :
   ```html
   <img src="images/votre-image.jpg" alt="Description">
   ```

### Changer les Couleurs

Modifiez le fichier `css/style.css` :
- `#d4af37` : Couleur dorée principale
- `#2c1810` : Couleur brune foncée
- `#f4f1e8` : Couleur du texte clair

### Personnaliser le Formulaire de Contact

Le formulaire actuel est statique. Pour le rendre fonctionnel :

1. **Option simple** : Utilisez un service comme Formspree
   ```html
   <form action="https://formspree.io/f/votre-id" method="POST">
   ```

2. **Option avancée** : Intégrez avec Netlify Forms ou un autre service

## Maintenance

### Mettre à Jour le Site

1. Modifiez les fichiers localement
2. Uploadez les changements sur GitHub
3. Les modifications apparaîtront automatiquement sur votre site

### Sauvegardes

GitHub conserve automatiquement l'historique de vos modifications. Vous pouvez toujours revenir à une version précédente si nécessaire.

## Conseils

- **Images** : Optimisez vos images (max 1MB chacune) pour un chargement rapide
- **Mobile** : Le site est déjà responsive, testez-le sur différents appareils
- **SEO** : Ajoutez des balises meta dans le `<head>` de chaque page pour améliorer le référencement
- **Analytics** : Intégrez Google Analytics pour suivre les visiteurs

## Support

Si vous rencontrez des problèmes :
1. Vérifiez que tous les fichiers sont bien uploadés
2. Attendez 5-10 minutes après activation de GitHub Pages
3. Consultez la documentation GitHub Pages : https://pages.github.com/

