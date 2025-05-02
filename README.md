# 🚀 Starter Kit Tailwind CSS 4.0 avec Vite

Un kit de démarrage rapide et simple pour créer des projets avec Tailwind CSS 4.0 et Vite.

## ✨ Introduction

Ce projet vous offre une configuration prête à l'emploi pour démarrer rapidement avec Tailwind CSS 4.0 et Vite, vous permettant de vous concentrer immédiatement sur le développement de votre interface.

## 🚀 Démarrer un nouveau projet

### Option 1 : Configuration manuelle

1. **Créer un nouveau projet Vite**
   ```bash
   npm create vite@latest mon-projet-tailwind -- --template vanilla
   cd mon-projet-tailwind
   ```

2. **Installer les dépendances**
   ```bash
    npm install -D tailwindcss postcss autoprefixer
    npm install -D tailwindcss @tailwindcss/vite
   ```

3. **Créer un fichier vite.config.js à la racine du projet**
   ```javascript
   import { defineConfig } from 'vite'
   import tailwindcss from '@tailwindcss/vite'
   
   export default defineConfig({
     plugins: [
       tailwindcss(),
     ],
   })
   ```

4. **Configurer les fichiers CSS**  
   Créez ou modifiez le fichier `src/index.css` :
   ```css
   @import "tailwindcss";
   ```

5. **Modifier le fichier main.js**
   ```javascript
   import './index.css'
   ```

6. **Utiliser les classes Tailwind dans votre HTML**
   ```html
   <h1 class="text-9xl text-blue-600">Hello World</h1>
   ```

### Option 2 : Cloner ce starter kit

1. **Cloner le dépôt**
   ```bash
   git clone https://github.com/votre-nom/tailwindcss-startkit.git
   cd tailwindcss-startkit
   ```

2. **Installer les dépendances**
   ```bash
   npm install
   ```

3. **Lancer le serveur de développement**
   ```bash
   npm run dev
   ```

## 📁 Structure du projet

```
tailwindcss-startkit/
├── src/
│   ├── main.js      # Point d'entrée JavaScript
│   └── index.css    # Style avec import Tailwind CSS
├── index.html       # Page HTML principale
├── vite.config.js   # Configuration Vite
└── package.json     # Dépendances et scripts
```

## 💡 Fonctionnalités

- ⚡️ **Vite** - Bundler ultra-rapide avec HMR (Hot Module Replacement)
- 🎨 **Tailwind CSS 4.0** - Framework CSS utilitaire
- 🧩 **@tailwindcss/vite** - Plugin officiel pour l'intégration Tailwind/Vite

## 📚 Documentation

- [Tailwind CSS](https://tailwindcss.com/)
- [Vite](https://vitejs.dev/)

## 📋 Commandes disponibles

```bash
# Démarrer le serveur de développement
npm run dev

# Construire pour la production
npm run build

# Prévisualiser la version de production
npm run preview
```

---

🔧 Créé avec ❤️ pour simplifier le développement frontend