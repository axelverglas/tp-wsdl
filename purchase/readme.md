# Purchase Management Service WSDL

Ce fichier WSDL décrit le service de gestion des achats (Purchase Management Service) qui fait partie de notre API Gateway. Le service est responsable de la gestion des opérations liées aux achats et utilise l'API Stripe pour le traitement des paiements.

## Types de données

### ProcessPurchaseRequest

- **Description** : Requête pour traiter un achat.
- **Éléments** :
  - `cartId` (xsd:string) : Identifiant unique du panier.
  - `stripeToken` (xsd:string) : Token unique généré par l'API Stripe pour le paiement.

### ProcessPurchaseResponse

- **Description** : Réponse à la requête de traitement d'un achat.
- **Éléments** :
  - `success` (xsd:boolean) : Indique si le traitement de l'achat a été réalisé avec succès.
  - `message` (xsd:string) : Fournit des informations supplémentaires sur le résultat du traitement de l'achat.

## Opérations

### ProcessPurchase

- **Description** : Traite un achat en utilisant l'API Stripe pour le paiement.
- **Paramètres d'entrée** :
  - `cartId` (xsd:string) : Identifiant unique du panier.
  - `stripeToken` (xsd:string) : Token unique généré par l'API Stripe pour le paiement.
- **Paramètres de sortie** :
  - `success` (xsd:boolean) : Indique si le traitement de l'achat a été réalisé avec succès.
  - `message` (xsd:string) : Fournit des informations supplémentaires sur le résultat du traitement de l'achat.
