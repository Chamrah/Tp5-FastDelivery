🚀 FastDelivery - Microservices Architecture
FastDelivery is a startup specializing in managing deliveries for multiple e-commerce platforms. To improve scalability and flexibility, the system has been redesigned using a microservices-based architecture with MongoDB, Node.js, and Express.

📌 Microservices Overview
🛍️ Product Service: Manages product catalog.

📦 Order Service: Handles customer orders.

🚚 Delivery Service: Manages order shipments.

🔐 Authentication Service: Manages users (customers & couriers).

⚙️ Key Features
✅ Independent MongoDB models for each microservice.
✅ REST API endpoints for seamless CRUD operations.
✅ JWT authentication for secure access.
✅ Stock updates & order status management.
✅ Automatic carrier assignment for deliveries.

📂 API Endpoints
🛍️ Product Service
POST /produit/ajouter → Add a new product.

GET /produit/:id → Get product details.

PATCH /produit/:id/stock → Update stock quantity.

📦 Order Service
POST /commande/ajouter → Place a new order.

GET /commande/:id → Retrieve order details.

PATCH /commande/:id/statut → Update order status.

🚚 Delivery Service
POST /livraison/ajouter → Assign a carrier & create delivery.

PUT /livraison/:id → Update delivery status.

🔐 Authentication Service
POST /auth/register → Register a new user.

POST /auth/login → Authenticate & receive a JWT token.

GET /auth/profil → Get user details (JWT required).

🛠 Tech Stack
Backend: Node.js, Express

Database: MongoDB

Authentication: JWT

Architecture: Microservices
