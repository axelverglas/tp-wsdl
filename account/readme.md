# Account Management Service WSDL

Ce fichier WSDL décrit le service de gestion des comptes (Account Management Service) qui fait partie de notre API Gateway. Le service est responsable de la gestion des opérations liées aux comptes utilisateur.

## Types de données

### CreateAccountRequest

- **Description** : Requête pour créer un compte utilisateur.
- **Éléments** :
  - `email` (xsd:string) : Adresse email de l'utilisateur.
  - `password` (xsd:string) : Mot de passe de l'utilisateur.

### CreateAccountResponse

- **Description** : Réponse à la requête de création d'un compte utilisateur.
- **Éléments** :
  - `success` (xsd:boolean) : Indique si la création du compte a été réalisée avec succès.
  - `message` (xsd:string) : Fournit des informations supplémentaires sur le résultat de la création du compte.

## Opérations

### CreateAccount

- **Description** : Crée un compte utilisateur avec une adresse email et un mot de passe.
- **Paramètres d'entrée** :
  - `email` (xsd:string) : Adresse email de l'utilisateur.
  - `password` (xsd:string) : Mot de passe de l'utilisateur.
- **Paramètres de sortie** :
  - `success` (xsd:boolean) : Indique si la création du compte a été réalisée avec succès.
  - `message` (xsd:string) : Fournit des informations supplémentaires sur le résultat de la création du compte.
