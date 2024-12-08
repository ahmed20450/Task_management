# Gestionnaire de Tâches en Ligne

Le **Gestionnaire de Tâches en Ligne** est une application web interactive permettant aux utilisateurs de gérer leurs tâches personnelles en ligne. Elle offre des fonctionnalités intuitives pour améliorer la productivité en simplifiant la gestion des tâches.

## Fonctionnalités

- **Création de tâches** : Ajoutez de nouvelles tâches avec un titre et une description.
- **Mise à jour de tâches** : Modifiez les informations des tâches existantes.
- **Suppression de tâches** : Supprimez les tâches terminées ou inutiles.
- **Filtrage et tri des tâches** : Classez vos tâches par priorité, statut ou date.
- **Interface utilisateur moderne et réactive** : Profitez d'une expérience fluide et accessible.

## Architecture et Technologies

### Backend

- **Langage** : PHP
- **Framework** : Symfony 6
- **ORM** : Doctrine
- **Base de données** : PostgreSQL

### Frontend

- **Moteur de rendu** : Twig (intégré avec Symfony)
- **Technologies** : HTML5, CSS3, JavaScript

### Outils supplémentaires

- **Composer** : Gestionnaire de dépendances PHP
- **Symfony CLI** : Serveur local de développement
- **Git** : Gestion de version
- **PostgreSQL** : Base de données relationnelle

## Prérequis

Assurez-vous que votre système est configuré avec les outils suivants :

- **PHP** : Version 8.0 ou supérieure
- **Composer** : Installé sur votre système
- **PostgreSQL** : Version 12 ou supérieure
- **Symfony CLI** : Installé pour gérer le serveur de développement
- **Git** : Pour cloner le projet

## Installation et Configuration

1. **Cloner le projet :**

   ```bash
   git clone <URL_DU_DEPOT>
   cd task-manager
   Installer les dépendances :

bash
Copy code
composer install
Configurer les variables d'environnement :
Copiez le fichier .env et configurez la connexion à PostgreSQL :

bash
Copy code
cp .env .env.local
Modifiez le fichier .env.local comme suit :

env
Copy code
DATABASE_URL="postgresql://postgres:root@127.0.0.1:5432/task_manager"
Créer la base de données :

bash
Copy code
php bin/console doctrine:database:create
Appliquer les migrations pour créer les tables :

bash
Copy code
php bin/console doctrine:migrations:migrate
Démarrer le serveur Symfony :

bash
Copy code
symfony server:start
