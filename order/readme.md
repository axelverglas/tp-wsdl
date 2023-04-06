# Service de gestion de commandes

Le service permet de créer des commandes avec des informations sur le client et les articles commandés

## Types de données

Le WSDL définit les types de données suivants :

- `Order` : Représente une commande, contenant un ID client et une liste d'articles.
- `OrderItem` : Représente un article de la commande, contenant un ID produit et une quantité.

### Opérations

Le service de gestion des commandes comprend une opération :

- `CreateOrder` : Crée une nouvelle commande avec les informations fournies sur le client et les articles commandés.
