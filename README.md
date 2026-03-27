# 🛒 E-Commerce Modern Stack

![Status](https://img.shields.io/badge/Status-En%20Développement-orange)
![Version](https://img.shields.io/badge/Version-0.1.0-blue)

Une plateforme e-commerce généraliste ultra-performante(🤥​) basée sur une architecture découpée (Headless) avec Symfony et React.

---

## 🚀 Stack Technique

### Backend (API Restful)
![Symfony](https://img.shields.io/badge/Symfony-7.0+-000000?style=for-the-badge&logo=symfony&logoColor=white)
![API Platform](https://img.shields.io/badge/API%20Platform-3.2-00599C?style=for-the-badge&logo=api-platform&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-Authentication-black?style=for-the-badge&logo=json-web-tokens&logoColor=white)

### Frontend (User Interface)
![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-6.0-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-4.0-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![Zustand](https://img.shields.io/badge/State-Zustand-443E38?style=for-the-badge&logo=react)

---

## 📌 À propos du projet

Ce projet est une solution de vente en ligne moderne. L'objectif est d'allier la robustesse de **Symfony 7** pour la logique métier et la rapidité de **React 18** pour l'expérience utilisateur.

### Fonctionnalités clés (En cours) :
* **API First** : Documentation Swagger/OpenAPI auto-générée.
* **Sécurité** : Authentification stateless via LexikJWTAuthenticationBundle.
* **Performance** : Stylisation avec Tailwind CSS 4 et build ultra-rapide via Vite.
* **Gestion d'état** : Store optimisé avec Zustand pour le panier et les préférences.

---

## 🛠️ Installation (Phase Alpha)

> [!NOTE]  
> Le projet est actuellement en cours de développement. Les commandes ci-dessous concernent l'initialisation de l'environnement de travail.

### Backend
```bash
cd backend
composer install
# Configurez votre .env (DATABASE_URL)
php bin/console doctrine:database:create
php bin/console doctrine:migrations:migrate
php bin/console lexik:jwt:generate-keypair
symfony server:start -d
