# Test technique IAD

## Développement d'une API de gestion de contacts. 
C'est une API REST développée en PHP7 / Symfony5 et avec API Platform. La base de données utilisée est MySQL. 

Une vérification de saisie a été mise en place avant l'enregistrement en base de données sur les champs suivants : 
- Taille minimum pour le nom et le prénom,
- Age avec une valeur positive,
- Format d'email valide. 
