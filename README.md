# 🎓 EspritHub - Plateforme Étudiante

Une plateforme tout-en-un pour les étudiants d'ESPRIT : accédez à vos cours, TD et examens, réservez vos salles et organisez votre temps facilement.

---

## 📋 Table des matières

- [Vue d'ensemble](#-vue-densemble)
- [Membres de l'équipe](#-membres-de-léquipe)
- [Structure du projet](#-structure-du-projet)
- [Instructions d'installation](#-instructions-dinstallation)
- [Comment exécuter le projet](#-comment-exécuter-le-projet)
- [Problèmes rencontrés et solutions](#-problèmes-rencontrés-et-solutions)
- [Spécifications techniques](#-spécifications-techniques)

---

## 👥 Membres de l'équipe

| Nom | Responsabilité | Pages |
|-----|-----------------|-------|
| **Marwa** | Lead Developer & Design | `index.html`, `historiquesalles.html` |
| **[Ajouter nom]** | [Responsabilité] | `details.html`, autres pages |

---

## 📁 Structure du projet

```
esprit-hub/
├── public/
│   ├── index.html              # Page d'accueil
│   ├── historiquesalles.html   # Page historique des réservations
│   ├── details.html            # Page de détails
│
├── assets/
│   ├── home/                   # Images pour la page d'accueil
│   ├── pageons/                # Images pour la page Ons
│   ├── pagesahar/              # Images pour la page Sahr
│
├── src/
│   ├── input.css               # Source CSS (Tailwind)
│
├── style.css                   # CSS compilé (généré automatiquement)
├── bg.png                      # Image de fond du header
├── package.json                # Configuration du projet
├── package-lock.json
├── tailwindcss.exe            # Exécutable Tailwind CLI
├── README.md                  # Ce fichier
└── .git/                      # Repository Git (à initialiser)
```

---

## 🚀 Instructions d'installation

### Prérequis
- **Node.js** v14+ (vérifiez avec `node --version`)
- **npm** (installé avec Node.js)

### Étapes

1. **Cloner le repository** (si depuis GitHub)
   ```powershell
   git clone https://github.com/votre-username/esprit-hub.git
   cd esprit-hub
   ```

2. **Installer les dépendances**
   ```powershell
   npm install
   ```

3. **Vérifier l'installation**
   ```powershell
   npm --version
   node --version
   ```

---

## ▶️ Comment exécuter le projet

### Option 1 : Avec serveur local HTTP (Recommandé)

**Terminal 1 - Compiler le CSS en mode watch :**
```powershell
cd "g:\marwa c\projet\esprit-hub"
npm run build:css
```

**Terminal 2 - Lancer un serveur HTTP :**
```powershell
npm install -g http-server  # (Première fois seulement)
http-server
```

Puis ouvrez votre navigateur et allez à : `http://localhost:8080`

---

### Option 2 : Ouverture directe du fichier

1. Naviguez vers le dossier `public/`
2. Double-cliquez sur `index.html`
3. Le site s'ouvre dans votre navigateur par défaut

**Note :** Cette méthode peut causer des problèmes CORS pour certaines ressources.

---

## ⚙️ Scripts npm

| Commande | Description |
|----------|-------------|
| `npm run build:css` | Compile le CSS Tailwind en mode watch (mise à jour automatique) |
| `npm install` | Installe les dépendances du projet |

---

## 🛠️ Problèmes rencontrés et solutions

### Problème 1 : "Tailwind CSS n'est pas compilé"
**Symptôme :** Le site s'affiche sans style.
**Solution :** 
- Assurez-vous que `npm run build:css` est en cours d'exécution
- Vérifiez que `style.css` existe et contient les classes Tailwind
- Videz le cache du navigateur (Ctrl+F5)

### Problème 2 : "Port 8080 déjà utilisé"
**Symptôme :** Erreur "Address already in use" lors du lancement du serveur.
**Solution :**
```powershell
# Utilisez un autre port
http-server -p 3000
# Puis allez à http://localhost:3000
```

### Problème 3 : "Fichiers images non trouvées"
**Symptôme :** Images manquantes dans les pages.
**Solution :**
- Vérifiez que les chemins dans `<img src=...>` sont corrects
- Assurez-vous que le dossier `assets/` est présent
- Les chemins doivent être relatifs au fichier HTML

### Problème 4 : "npm command not found"
**Symptôme :** Erreur "npm is not recognized" en PowerShell.
**Solution :**
- Installez Node.js depuis https://nodejs.org
- Redémarrez PowerShell après l'installation
- Vérifiez avec `npm --version`

---

## 📱 Spécifications techniques

### Stack technologique
- **HTML5** : Structure sémantique
- **Tailwind CSS v4.1.17** : Framework CSS utility-first
- **Google Fonts** : Outfit (titres), Lato (corps)
- **JavaScript** : (À ajouter selon les besoins)

### Breakpoints responsifs (Tailwind)
- **Mobile** : < 640px (par défaut)
- **Tablet (sm)** : ≥ 640px
- **Desktop (md)** : ≥ 768px
- **Large (lg)** : ≥ 1024px

### Palette de couleurs

| Couleur | Hex | Utilisation |
|---------|-----|-------------|
| Rouge foncé | `#8E1616` | Fond, accents, titres |
| Beige/Crème | `#F8EEDF` | Fond footer, texte clair |
| Or/Accent | `#E8C999` | Boutons, highlights |
| Texte clair | `#EEF2D5` | Texte sur fond rouge |
| Blanc | `#FFFFFF` | Cartes, conteneurs |

### Polices
- **Outfit** : Utilisée pour les titres et éléments importants
- **Lato** : Utilisée pour le texte courant et descriptions
- **Inter** : Font par défaut (fallback)

---

## 🎯 Critères de validation

### Points d'évaluation (100 points)
- ✅ **Respect de la maquette Figma** : 50%
- ✅ **Responsive Design** : 30%
- ✅ **Collaboration (GitHub)** : 10%
- ✅ **Déploiement (GitHub Pages)** : 10%

### Checklist de livraison

- [ ] Toutes les pages sont créées et fonctionnelles
- [ ] CSS Tailwind est correctement utilisé (pas de CSS personnalisé)
- [ ] Responsive design testé sur mobile/tablet/desktop
- [ ] Repository Git initialisé avec commits réguliers
- [ ] README.md complet et à jour
- [ ] Déploiement sur GitHub Pages effectué
- [ ] Aucune erreur console dans le navigateur

---

## 📞 Contact & Support

**Email :** contact@esprithub.tn  
**Téléphone :** +216 70 685 685

---

## 📄 Licence

ISC - Tous droits réservés © 2025 ESPRITHUB

---

**Dernière mise à jour :** 3 Décembre 2025
