# Test technique IAD

## Développement d'une API de gestion de contacts. 
C'est une API REST développée en PHP7 / Symfony5 et avec API Platform. La base de données utilisée est MySQL. 

Une vérification de saisie a été mise en place avant l'enregistrement en base de données sur les champs suivants : 
- Taille minimum pour le nom et le prénom,
- Age avec une valeur positive,
- Format d'email valide. 

## Installation du projet
Clonez le projet à l'adresse suivante: https://github.com/ylion75/IAD-test

Exécutez ensuite les commandes suivantes: 
1. composer install afin d'installer les dépendances composer du projet,
2. Installez la base de données MySQL. Afin de la paramétrer, modifiez la variable d'environnement dans le fichier .env du projet : 
DATABASE_URL="mysql://root:@127.0.0.1:3306/iad?serverVersion=5.7"
Puis créer la base de données avec la commande suivante: symfony console doctrine:database:create
3. Exécutez la migration en base de donnée: symfony console doctrine:migration:migrate
4. Vous pouvez maintenant lancer le serveur symfony avec: symfony server:start
5. L'API peut être testée avec Swagger sur: http://127.0.0.1:8000/api
