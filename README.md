# 🚀 Application AWS

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Application AWS** est un projet personnel permettant de gérer des machines virtuelles (VM) sur **AWS Cloud** via une interface web moderne et une API sécurisée.  
Le projet combine une interface **Frontend React** et une API **Backend Node.js**, intégrant **Terraform** et **Ansible** pour l'automatisation de l'infrastructure sur **AWS Cloud**.

👉 [Lien du dépôt GitHub](https://github.com/Steph-mss/Application-AWS)

---

## 🗂️ Architecture du projet

Application-AWS/
├── frontend/ # Interface utilisateur React
├── backend/ # API Node.js + gestion des VMs (Terraform / Ansible)
└── README.md # Ce fichier

markdown
Copier
Modifier

---

## ✨ Fonctionnalités principales

### ✅ Authentification & Gestion des utilisateurs

- Inscription, connexion, déconnexion
- Réinitialisation de mot de passe
- Middleware d'authentification JWT
- Rafraîchissement de token
- Gestion des sessions sécurisée

### ⚙️ Gestion des machines virtuelles (VM) sur AWS Cloud

- Création et suppression de VMs sur **AWS Cloud**
- Téléchargement des configurations VPN
- Récupération du mot de passe Windows
- Infrastructure provisionnée sur AWS via **Terraform**
- Configuration automatisée via **Ansible**

### ✉️ Notifications

- Envoi d’emails (ex: réinitialisation de mot de passe) via service Gmail

### 🔐 Sécurisation

- Authentification via **JWT**
- Protection des routes API
- Gestion des CORS

### 💻 Interface utilisateur

- Tableau de bord de gestion des VMs AWS
- Formulaires d’inscription / connexion
- Feedback utilisateur (modales, messages d'erreurs, loading)
- Gestion globale des erreurs via `ErrorBoundary`

---

## 🛠️ Prérequis

- **Node.js** ≥ 14.x
- **npm** ou **yarn**
- **Base de données** (configurable dans `config/db.js` pour le backend)
- **Terraform** installé localement
- **Ansible** installé localement
- Compte **AWS Cloud** configuré (avec les bonnes permissions IAM)
- Variables d’environnement `.env` correctement configurées pour le backend

---

## 🚀 Installation

### 1️⃣ Cloner le projet

```bash
git clone https://github.com/Steph-mss/Application-AWS.git
cd Application-AWS
2️⃣ Installation du Frontend
bash
Copier
Modifier
cd frontend
npm install
3️⃣ Installation du Backend
bash
Copier
Modifier
cd ../backend
npm install
▶️ Lancement de l'application
Démarrer le Backend
bash
Copier
Modifier
cd backend
npm start
ou en mode développement :

bash
Copier
Modifier
npm run dev
Démarrer le Frontend
bash
Copier
Modifier
cd frontend
npm start
Accéder à l’application via : http://localhost:3000

🔍 Structure détaillée
Backend
Authentification : JWT, refresh token, gestion des sessions

Gestion des VMs AWS : intégration avec Terraform & Ansible

Services API REST pour la création et la gestion des VMs sur AWS

Envoi d’emails via service Gmail

Sécurisation : CORS + Middleware JWT

Frontend
Interface utilisateur en React

Gestion des VMs AWS : création, suppression, téléchargement VPN

Authentification sécurisée

UX optimisée : feedback utilisateur, gestion d’erreurs globale

✅ Contribution
Les contributions sont les bienvenues !
Si vous souhaitez contribuer :

Forkez le projet

Créez une branche (git checkout -b feature/ma-feature)

Committez vos modifications (git commit -m 'Ajout de ma feature')

Poussez vers votre fork (git push origin feature/ma-feature)

Ouvrez une pull request

📜 Licence
Ce projet est sous licence MIT.

💡 Auteur
Projet personnel développé par Steph-mss.
