# youssef-bssat-evaluation-finaleH26

# Application de Bibliothèque API & Client
Cette application permet de consulter les livres disponibles et les emprunts en cours d'un utilisateur à l'aide de son adresse courriel.
---
## 🛠️ Configuration et Installation
### Prérequis
- [Node.js](https://nodejs.org/) installé sur votre machine.
- Une base de données MySQL configurée.
### 1. Serveur (Backend)
1. Ouvrez un terminal dans le dossier `server` :
   ```bash
   cd bibliotheque/server
Installez les dépendances :
bash
npm install
Créez un fichier .env à la racine du dossier server et configurez les variables d'environnement suivantes :
env
PORT=5000
DB_HOST=localhost
DB_USER=votre_utilisateur
DB_PASSWORD=votre_mot_de_passe
DB_NAME=nom_de_la_base_de_donnees
Lancez le serveur de développement :
bash
npm start
2. Client (Frontend)
Ouvrez un terminal dans le dossier client :
bash
cd bibliotheque/client
Installez les dépendances :
bash
npm install
Lancez l'application React :
bash
npm run dev
📖 Documentation de l'API (Swagger)
L'API est documentée de manière interactive avec Swagger. Une fois le serveur lancé, vous pouvez y accéder à l'adresse suivante :

👉 http://localhost:5000/api-docs

Endpoints Principaux
GET /api/livres : Récupère la liste de tous les livres disponibles à l'emprunt (disponible = 1).
GET /api/livres/emprunts?email= : Récupère les livres actuellement empruntés (non retournés) par un utilisateur spécifique grâce à son adresse courriel.
GET /api/emprunts?email= : Alias direct pour récupérer les livres empruntés par courriel.
