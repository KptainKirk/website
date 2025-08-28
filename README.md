# Mon Site Web - GitHub Pages

Un site web moderne et responsive créé avec HTML, CSS et JavaScript, conçu pour être hébergé sur GitHub Pages.

## 🚀 Fonctionnalités

- **Design moderne et responsive** : S'adapte à tous les appareils
- **Navigation fluide** : Menu de navigation avec défilement fluide
- **Sections interactives** : À propos, services et contact
- **Formulaire de contact** : Avec validation et notifications
- **Animations** : Effets visuels au scroll et au survol
- **Performance optimisée** : Chargement rapide et expérience utilisateur fluide

## 📁 Structure du projet

```
FB/
├── index.html          # Page principale
├── styles.css          # Styles CSS
├── script.js           # JavaScript interactif
├── README.md           # Ce fichier
└── .gitignore          # Fichiers à ignorer par Git
```

## 🌐 Déploiement sur GitHub Pages

### Étape 1 : Créer un repository GitHub

1. Allez sur [GitHub](https://github.com) et connectez-vous
2. Cliquez sur le bouton "+" puis "New repository"
3. Nommez votre repository (ex: `mon-site-web`)
4. Laissez-le public
5. Cliquez sur "Create repository"

### Étape 2 : Pousser votre code

```bash
# Initialiser Git dans votre dossier local
git init

# Ajouter tous les fichiers
git add .

# Premier commit
git commit -m "Initial commit - Site web complet"

# Ajouter l'origine distante (remplacez USERNAME et REPO_NAME)
git remote add origin https://github.com/USERNAME/REPO_NAME.git

# Pousser vers GitHub
git push -u origin main
```

### Étape 3 : Activer GitHub Pages

1. Dans votre repository GitHub, allez dans "Settings"
2. Cliquez sur "Pages" dans le menu de gauche
3. Dans "Source", sélectionnez "Deploy from a branch"
4. Choisissez la branche "main" et le dossier "/ (root)"
5. Cliquez sur "Save"

Votre site sera accessible à l'adresse : `https://USERNAME.github.io/REPO_NAME`

## 🔗 Configuration du nom de domaine GoDaddy

### Étape 1 : Configurer les DNS sur GoDaddy

1. Connectez-vous à votre compte GoDaddy
2. Allez dans "My Products" → "DNS"
3. Trouvez votre domaine et cliquez sur "Manage DNS"
4. Dans la section "Records", ajoutez/modifiez :

#### Pour un domaine racine (exemple.com) :
```
Type: CNAME
Name: @
Value: USERNAME.github.io
TTL: 600 (ou 1 heure)
```

#### Pour un sous-domaine (www.exemple.com) :
```
Type: CNAME
Name: www
Value: USERNAME.github.io
TTL: 600 (ou 1 heure)
```

### Étape 2 : Configurer GitHub Pages

1. Retournez dans les paramètres de votre repository GitHub
2. Dans "Pages", ajoutez votre nom de domaine dans "Custom domain"
3. Cochez "Enforce HTTPS"
4. Sauvegardez

### Étape 3 : Créer le fichier CNAME

Créez un fichier `CNAME` à la racine de votre projet :

```bash
echo "votre-domaine.com" > CNAME
git add CNAME
git commit -m "Ajout du fichier CNAME"
git push
```

## 🎨 Personnalisation

### Modifier le contenu

- **Titre et description** : Modifiez le `<title>` et `<meta name="description">` dans `index.html`
- **Texte** : Remplacez le contenu des sections dans `index.html`
- **Couleurs** : Modifiez les variables CSS dans `styles.css`
- **Images** : Remplacez les emojis par vos propres images

### Ajouter des sections

1. Ajoutez une nouvelle section dans `index.html`
2. Créez les styles correspondants dans `styles.css`
3. Ajoutez l'animation dans `script.js` si nécessaire

## 📱 Responsive Design

Le site est entièrement responsive et s'adapte à :
- **Desktop** : Écrans larges avec mise en page en grille
- **Tablet** : Adaptation automatique des colonnes
- **Mobile** : Menu hamburger et mise en page verticale

## 🚀 Mise à jour du site

Après chaque modification :

```bash
git add .
git commit -m "Description des modifications"
git push
```

GitHub Pages se mettra à jour automatiquement en quelques minutes.

## 🔧 Dépannage

### Le site ne s'affiche pas
- Vérifiez que GitHub Pages est activé
- Attendez quelques minutes après le push
- Vérifiez les paramètres DNS sur GoDaddy

### Le nom de domaine ne fonctionne pas
- Vérifiez que le fichier CNAME est présent
- Attendez la propagation DNS (peut prendre jusqu'à 48h)
- Vérifiez la configuration DNS sur GoDaddy

### Problèmes de mise en page
- Videz le cache de votre navigateur
- Testez sur différents appareils
- Vérifiez la console du navigateur pour les erreurs

## 📞 Support

Pour toute question ou problème :
- Consultez la [documentation GitHub Pages](https://docs.github.com/en/pages)
- Vérifiez la [documentation GoDaddy DNS](https://www.godaddy.com/help)

## 📄 Licence

Ce projet est sous licence MIT. Vous êtes libre de l'utiliser et de le modifier selon vos besoins.

---

**Bon déploiement ! 🎉**
