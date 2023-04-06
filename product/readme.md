# Service de gestion du stock de produits

Ce service permet de récupérer le stock d'un produit en fonction de son ID. Le document WSDL définit le service, les opérations, les types de données et les messages associés.

### Types de données

Le WSDL définit les types de données suivants :

- `GetProductStockRequest` : Représente une demande pour obtenir le stock d'un produit, contenant un ID produit.
- `GetProductStockResponse` : Représente la réponse avec la quantité en stock du produit demandé.

### Opérations

Le service de gestion du stock de produits comprend une opération :

- `GetProductStock` : Récupère la quantité en stock d'un produit en fonction de son ID.
