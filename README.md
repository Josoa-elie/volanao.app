# Volanao

> **"Ny volanao, ny drafitrao"** — *Ton argent, ton plan.*

**Volanao** est une application web de gestion de budget personnel conçue pour aider les utilisateurs à suivre leurs dépenses mensuelles, définir un salaire de référence, et visualiser leur santé financière en un coup d'œil.

---

## Le projet

Beaucoup de personnes ont du mal à savoir **où part leur argent** chaque mois. Volanao répond à ce problème avec une interface simple et intuitive :

- **Définir son salaire** mensuel comme référence
- **Catégoriser ses dépenses** (Nourriture, Transport, Loisirs, etc.)
- **Fixer des limites** par catégorie (optionnel)
- **Visualiser en temps réel** le reste à vivre et la progression du mois
- **Être alerté** quand une catégorie dépasse sa limite

Le nom **Volanao** vient du malagasy : *"vola"* (argent) + *"-nao"* (ton) → **"ton argent"**.

---

## Fonctionnalités

### Authentification
- Inscription / connexion avec JWT (access + refresh tokens)
- Auto-refresh silencieux du token expiré
- Routes protégées côté frontend

### Gestion des dépenses
- CRUD complet (créer, lire, modifier, supprimer)
- Filtres par mois et par catégorie
- Description optionnelle par dépense

### Gestion des catégories
- CRUD complet avec personnalisation
- Choix d'icône (emoji) et de couleur
- Limite mensuelle optionnelle par catégorie

### Budget mensuel
- Définir son salaire pour chaque mois
- Un seul budget par mois (contrainte d'unicité)
- Comparaison automatique dépenses / salaire

### Dashboard
- Vue globale du mois : salaire, dépenses, reste à vivre
- Barre de progression globale
- Détail par catégorie avec barres de progression colorées
- Alertes visuelles en cas de dépassement

### Interface
- Dark mode / Light mode
- Design responsive (mobile, tablette, desktop)
- Composants DaisyUI modernes

---

## Stack technique

### Backend
Technologie & Rôle 

**Django 5** : Framework web 
**Django REST Framework** : API REST 
**SimpleJWT** : Authentification par tokens 
**django-cors-headers** : Gestion CORS frontend/backend 
**python-decouple** : Gestion des variables d'environnement 
**PostgreSQL** : Base de données (production) 
**SQLite** : Base de données (développement) 
**WhiteNoise** : Service des fichiers statiques en prod 

### Frontend
Technologie & Rôle 
-------------------
**React 18** : Bibliothèque UI 
**Vite** : Build tool rapide 
**React Router** : Routage SPA 
**Axios** : Client HTTP + intercepteurs JWT 
**Tailwind CSS** : Styles utilitaires 
**DaisyUI** : Composants UI prêts à l'emploi 
**Context API** : Gestion d'état d'authentification 

---------------------------------------------------------------------------------------------

# Volanao

> **"Ny volanao, ny drafitrao"** — *Your money, your plan.*

**Volanao** is a personal budget management web app designed to help users track their monthly expenses, set a reference income, and visualize their financial health at a glance.

---

## The Project

Many people struggle to know **where their money goes** each month. Volanao solves this with a simple and intuitive interface:

- **Set your monthly income** as a baseline
- **Categorize your expenses** (Food, Transport, Leisure, etc.)
- **Set per-category limits** (optional)
- **Visualize in real time** your remaining balance and monthly progress
- **Get alerted** when a category exceeds its limit

The name **Volanao** comes from Malagasy: *"vola"* (money) + *"-nao"* (your) → **"your money"**.

---

## Features

### Authentication
- Sign up / sign in with JWT (access + refresh tokens)
- Silent auto-refresh of expired tokens
- Protected routes on the frontend

### Expense Management
- Full CRUD (create, read, update, delete)
- Filters by month and category
- Optional description per expense

### Category Management
- Full CRUD with customization
- Icon (emoji) and color picker
- Optional monthly limit per category

### Monthly Budget
- Set your income for each month
- One single budget per month (uniqueness constraint)
- Automatic comparison between expenses and income

### Dashboard
- Global monthly view: income, expenses, remaining balance
- Global progress bar
- Per-category breakdown with colored progress bars
- Visual alerts when a limit is exceeded

### Interface
- Dark mode / Light mode
- Responsive design (mobile, tablet, desktop)
- Modern DaisyUI components

---

## Tech Stack

### Backend

 Technology & Role 
------------------
 **Django 5**  Web framework 
 **Django REST Framework**  REST API 
 **SimpleJWT**  Token-based authentication 
 **django-cors-headers**  CORS handling between frontend/backend 
 **python-decouple**  Environment variable management 
 **PostgreSQL**  Database (production) 
 **SQLite**  Database (development) 
 **WhiteNoise**  Static file serving in production 

### Frontend

 Technology & Role 
------------------
 **React 18**  UI library 
 **Vite**  Fast build tool 
 **React Router**  SPA routing 
 **Axios**  HTTP client + JWT interceptors 
 **Tailwind CSS**  Utility-first styling 
 **DaisyUI**  Pre-built UI components 
 **Context API**  Authentication state management 
