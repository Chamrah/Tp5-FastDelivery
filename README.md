FastDelivery

FastDelivery est une startup spécialisée dans la gestion des livraisons pour plusieurs plateformes e-commerce. Afin d'améliorer la scalabilité et la flexibilité, le système a été repensé en utilisant une architecture basée sur les microservices avec MongoDB, Node.js et Express.



📌 Aperçu des Microservices


-Service Produit : Gère le catalogue des produits.

-Service Commande : Gère les commandes des clients.

-Service Livraison : Gère l'expédition des commandes.

-Service Authentification : Gère les utilisateurs (clients et transporteurs).



⚙️ Fonctionnalités Clés


✅ Modèles MongoDB indépendants pour chaque microservice.

✅ Endpoints API REST pour des opérations CRUD fluides.

✅ Authentification JWT pour un accès sécurisé.

✅ Mise à jour du stock et gestion du statut des commandes.

✅ Attribution automatique des transporteurs pour les livraisons.



📂 Endpoints API+


-Service Produit

POST /produit/ajouter → Ajouter un nouveau produit.

GET /produit/:id → Obtenir les détails d’un produit.

PATCH /produit/:id/stock → Mettre à jour la quantité en stock.


-Service Commande


POST /commande/ajouter → Passer une nouvelle commande.

GET /commande/:id → Récupérer les détails d’une commande.

PATCH /commande/:id/statut → Mettre à jour le statut d’une commande.


-Service Livraison


POST /livraison/ajouter → Assigner un transporteur et créer une livraison.

PUT /livraison/:id → Mettre à jour le statut de la livraison.


-Service Authentification


POST /auth/register → Enregistrer un nouvel utilisateur.

POST /auth/login → Authentifier et recevoir un token JWT.

GET /auth/profil → Obtenir les détails d’un utilisateur (JWT requis).
