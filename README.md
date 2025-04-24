# 🔐 Auth Microservice (Laravel)

Microservice d'authentification modulaire avec **Email, OAuth2 (Google/Facebook/GitHub/LinkedIn) et SMS**.  
Parfait pour intégrer une authentification sécurisée dans n'importe quelle application.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)  
**Auteur** : [Abdoul Wakilou Tiga](https://linkedin.com/in/abdoul-wakilou-tiga)  
📞 `+229 01 51 97 91 63` | ✉️ `abdoulwakiloutiga@gmail.com`

---

## 🛠️ Fonctionnalités

- ✅ Inscription / Connexion par **email** (avec vérification).
- 🔐 Authentification **OAuth2** (Google, Facebook, GitHub, LinkedIn).
- 📱 Authentification et notifications **par SMS** (Twilio / Africa’s Talking).
- 🔑 Authentification **API avec JWT ou Laravel Sanctum**.
- 🧱 Architecture **modulaire**, prête pour Docker/Kubernetes.

---

## 🚀 Installation

```bash
composer create-project laravel/laravel auth-microservice
cd auth-microservice

# Dépendances d'authentification
composer require laravel/sanctum laravel/socialite

# Publier les fichiers de Sanctum
php artisan vendor:publish --provider="Laravel\Sanctum\SanctumServiceProvider"

# Lancer les migrations
php artisan migrate
