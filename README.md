![Penya Vigatanes](https://img.shields.io/badge/Penya-Vigatanes-blue)

# 🏉 Penya Vigatanes - Application Communautaire

Application web pour la gestion et le suivi de la communauté Penya Vigatanes (supporters de l'USAP).

## ✨ Fonctionnalités

- 📊 **Pronostics** - Faites vos prédictions sur les matchs USAP
- 📈 **Classement** - Suivez le classement des pronostiqueurs
- 📅 **Calendrier** - Matchs USAP et planning des repas Penya
- 📰 **Actualités** - Flux Instagram officiel de l'USAP
- 👥 **Espace Responsable** - Gestion interne de la Penya

## 🚀 Installation

### Prérequis
- Node.js (v16 ou supérieur)
- npm ou yarn
- MongoDB (local ou cloud)

### Configuration

1. **Cloner le dépôt**
```bash
git clone https://github.com/fab78547/penya-vigatanes-app.git
cd penya-vigatanes-app
```

2. **Installer les dépendances**
```bash
npm install-all
```

3. **Configuration d'environnement**
Créez un fichier `.env` à la racine du projet :
```bash
cp .env.example .env
```

Modifiez `.env` avec vos paramètres :
```
PORT=5000
MONGODB_URI=mongodb://localhost:27017/penya-vigatanes
INSTAGRAM_ACCESS_TOKEN=your_token_here
INSTAGRAM_BUSINESS_ACCOUNT_ID=your_account_id_here
NODE_ENV=development
```

### Démarrage

**Terminal 1 - Backend (Node.js)**
```bash
npm run dev
```

**Terminal 2 - Frontend (React)**
```bash
npm run client
```

L'application sera accessible sur `http://localhost:3000`

## 📁 Structure du Projet

```
penya-vigatanes-app/
├── client/                 # Application React
│   ├── public/
│   └── src/
│       ├── pages/         # Pages de l'application
│       ├── App.js         # Composant principal
│       └── index.js
├── routes/                # Routes API Express
│   ├── pronostics.js
│   ├── classement.js
│   ├── calendrier.js
│   ├── actualites.js
│   └── responsables.js
├── server.js              # Configuration Express
├── package.json
└── README.md
```

## 🔧 Développement

### APIs disponibles

- `GET /api/pronostics` - Liste des pronostics
- `GET /api/classement` - Classement des pronostiqueurs
- `GET /api/calendrier` - Matchs et repas
- `GET /api/actualites` - Actualités Instagram
- `GET /api/responsables` - Informations des responsables

### Ajouter une nouvelle fonctionnalité

1. Créer une nouvelle route dans `/routes`
2. Ajouter une page React dans `/client/src/pages`
3. Ajouter le lien dans la navigation du composant `App.js`

## 🔐 Sécurité

- Utilisez des variables d'environnement pour les tokens sensibles
- Ne commitez jamais le fichier `.env`
- Validez toujours les données côté serveur

## 📝 À faire

- [ ] Système d'authentification utilisateur
- [ ] Intégration complète API Instagram
- [ ] Système de base de données MongoDB
- [ ] Page de gestion des profils utilisateur
- [ ] Notifications en temps réel
- [ ] Tests unitaires
- [ ] Déploiement en production

## 📄 Licence

MIT

## 👥 Contributeurs

- fab78547 - Créateur

## 📞 Contact

Pour plus d'informations : penya-vigatanes@example.com

---

**Allez Vigatanes ! 🏉**
