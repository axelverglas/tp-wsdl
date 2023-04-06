# Service de gestion du panier

Ce fichier WSDL décrit le service de gestion du panier (Cart Management Service) qui fait partie de notre API Gateway. Le service est responsable de la gestion des opérations liées au panier, comme l'ajout d'un produit au panier.

## Type de données

### AddProductToCartRequest

- **Description** : Requête pour ajouter un produit au panier.
- **Éléments** :
  - `cartId` (xsd:string) : Identifiant unique du panier.
  - `productId` (xsd:string) : Identifiant unique du produit à ajouter au panier.
  - `quantity` (xsd:int) : Quantité du produit à ajouter au panier.

### AddProductToCartResponse

- **Description** : Réponse à la requête d'ajout d'un produit au panier.
- **Éléments** :
  - `success` (xsd:boolean) : Indique si l'ajout du produit au panier a été réalisé avec succès.

## Opérations

### AddProductToCart

- **Description** : Ajoute un produit au panier.
- **Paramètres d'entrée** :
  - `cartId` (xsd:string) : Identifiant unique du panier.
  - `productId` (xsd:string) : Identifiant unique du produit à ajouter au panier.
  - `quantity` (xsd:int) : Quantité du produit à ajouter au panier.
- **Paramètres de sortie** :
  - `success` (xsd:boolean) : Indique si l'ajout du produit au panier a été réalisé avec succès.
