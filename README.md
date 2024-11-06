# Vue 3 Starter Template

## Description

Un template Vue 3 moderne et robuste configuré avec TypeScript, Vite, Pinia, Vue Router et TailwindCSS. Ce starter kit fournit une base solide pour démarrer rapidement des projets Vue.js avec les meilleures pratiques et outils actuels.

## ✨ Fonctionnalités

- 🚀 [Vue 3](https://vuejs.org/) avec Composition API et `<script setup>`
- ⚡️ [Vite](https://vitejs.dev/) pour un développement ultra-rapide
- 🎯 [TypeScript](https://www.typescriptlang.org/) pour une meilleure maintenabilité
- 📦 [Pinia](https://pinia.vuejs.org/) pour la gestion d'état
- 🛣 [Vue Router](https://router.vuejs.org/) avec génération automatique des routes
- 🎨 [TailwindCSS](https://tailwindcss.com/) pour le styling
- 📝 [ESLint](https://eslint.org/) + [Prettier](https://prettier.io/) pour un code propre et formaté
- 🧪 [Vitest](https://vitest.dev/) pour les tests unitaires
- 💪 [TypeScript](https://www.typescriptlang.org/) strict activé
- 🔧 [VueUse](https://vueuse.org/) - Collection de composables Vue utiles

## 🛠 Prérequis

- Node.js 20.x ou supérieur
- npm ou yarn ou pnpm

## 🚀 Pour démarrer

1. Cloner le projet :

```bash
git clone https://github.com/FlorianBx/vue-3-starter.git
cd starter-vue
```

2. Installer les dépendances :

```bash
npm install
# ou
yarn
# ou
pnpm install
```

3. Démarrer le serveur de développement :

```bash
npm run dev
# ou
yarn dev
# ou
pnpm dev
```

## 📜 Scripts disponibles

- `dev` : Lance le serveur de développement
- `build` : Compile le projet pour la production
- `preview` : Prévisualise la version de production en local
- `test:unit` : Lance les tests unitaires
- `type-check` : Vérifie les types TypeScript
- `lint` : Lint le code avec ESLint
- `format` : Formate le code avec Prettier

## 📁 Structure du projet

```bash
starter-vue/
├── src/
│   ├── assets/         # Fichiers statiques
│   │   └── main.css    # Styles globaux
│   │
│   ├── components/     # Composants Vue réutilisables
│   │   ├── __tests__/ # Tests des composants
│   │   ├── layout/    # Composants de mise en page
│   │   │   └── LayoutDefault.vue
│   │   ├── shared/    # Composants partagés globaux
│   │   │   └── YourComponentShare.vue
│   │   └── features/  # Composants spécifiques aux features
│   │       └── auth/  # Exemple: Composants d'authentification
│   │           ├── LoginForm.vue
│   │           └── RegisterForm.vue
│   │
│   ├── composables/    # Composables Vue (logique réutilisable)
│   │   └── useSomething.ts
│   │
│   ├── stores/        # Stores Pinia centralisés
│   │   └── auth.ts
│   │
│   ├── types/         # Types TypeScript centralisés
│   │   └── auth.ts
│   │
│   ├── pages/         # Pages de l'application
│   │   ├── index.vue
│   │   ├── about.vue
│   │   ├── params/
│   │   │   └── [id].vue
│   │   └── search/
│   │       └── index.vue
│   │
│   └── App.vue
```

### 📂 Description détaillée des dossiers

- **`assets/`**: Contient les ressources statiques comme les styles CSS, images, etc.

  - `main.css`: Styles globaux et configuration TailwindCSS

- **`components/`**: Composants Vue réutilisables

  - `__tests__/`: Tests unitaires des composants
  - `layout/`: Composants de mise en page (header, footer, etc.)
  - `shared/`: Composants partagés réutilisables dans toute l'application

- **`composables/`**: Hooks Vue personnalisés et logique réutilisable

  - Exemple: `useSomething.ts` - logique métier extraite et réutilisable

- **`pages/`**: Structure automatique des routes avec `unplugin-vue-router`
  - Les fichiers `.vue` sont automatiquement convertis en routes
  - Support des routes dynamiques avec `[id].vue`
  - Les dossiers créent des sous-routes automatiquement

Cette structure suit les meilleures pratiques Vue.js et facilite :

- La séparation des préoccupations
- La réutilisation des composants
- Le test unitaire
- Le routage automatique
- L'organisation modulaire du code

## 🔧 Configuration

Le projet inclut des configurations pour :

- TypeScript (`tsconfig.json`)
- Vite (`vite.config.ts`)
- ESLint (`.eslintrc.cjs`)
- Prettier (`.prettierrc.json`)
- TailwindCSS (`tailwind.config.js`)

## 📝 Notes

- Le routage est géré automatiquement par `unplugin-vue-router` basé sur la structure des fichiers dans le dossier `pages/`
- Les tests sont configurés avec Vitest et Vue Test Utils
- Le support de TypeScript strict est activé par défaut

## 📚 Documentation des dépendances

- [Vue 3 Documentation](https://vuejs.org/)
- [Vite Documentation](https://vitejs.dev/)
- [Vue Router Documentation](https://router.vuejs.org/)
- [Pinia Documentation](https://pinia.vuejs.org/)
- [TailwindCSS Documentation](https://tailwindcss.com/)

## 📄 License

MIT
