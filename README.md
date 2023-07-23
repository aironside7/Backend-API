Project Description:
----------------------------------------------------------------------------------------------------------------------------------------------------

***********

(I have chosen to use the MERN stack with JavaScript instead of TypeScript, as i am more comfortable with JavaScript. This decision allows you to build your web application using the familiar technologies of MongoDB, Express.js, React, and Node.js with the convenience of JavaScript as the programming language.)
----------------------------------------------------------------------------------------------------------------------------------------------------

The FMCG (Fast-Moving Consumer Goods) App backend is a RESTful API that provides various endpoints to manage users, customers, products, and orders. It is designed to serve as the backend for an FMCG application, allowing users to register and log in, manage customer data, create, update, and delete products, and handle orders.

Endpoints and Features:

User Authentication Endpoints:

POST /api/auth/register: Register a new user by providing a username, email, and password. Returns a JWT token upon successful registration.
POST /api/auth/login: Log in as an existing user by providing the username and password. Returns a JWT token upon successful login.
Customer Management Endpoints:

POST /api/customers: Create a new customer by providing the customer's name, email, and phone number. Requires authentication and authorization (admin role).
GET /api/customers: Get a list of all customers. Requires authentication.
GET /api/customers/{id}: Get customer data by providing the customer ID. Requires authentication.
PUT /api/customers/{id}: Update customer data by providing the customer ID and new information (name, email, phone). Requires authentication.
DELETE /api/customers/{id}: Delete a customer by providing the customer ID. Requires authentication and authorization (admin role).
Product Management Endpoints:

POST /api/products: Create a new product by providing the product's name, price, and description. Requires authentication and authorization (admin role).
GET /api/products: Get a list of all products. Requires authentication.
GET /api/products/{id}: Get product data by providing the product ID. Requires authentication.
PUT /api/products/{id}: Update product data by providing the product ID and new information (name, price, description). Requires authentication and authorization (admin role).
DELETE /api/products/{id}: Delete a product by providing the product ID. Requires authentication and authorization (admin role).
Order Management Endpoints:

POST /api/orders: Create a new order by providing the customer ID and an array of product IDs. Requires authentication.
GET /api/orders: Get a list of all orders. Requires authentication and authorization (admin role).
GET /api/orders/{id}: Get order data by providing the order ID. Requires authentication.
PUT /api/orders/{id}: Update order data by providing the order ID, customer ID, and an array of product IDs. Requires authentication.
DELETE /api/orders/{id}: Delete an order by providing the order ID. Requires authentication and authorization (admin role).
Features:

User Registration and Authentication: Users can register with the system and log in using their credentials. Authentication is done via JWT tokens.
Role-Based Authorization: The API implements role-based access control, allowing certain endpoints to be accessible only to users with administrative privileges.
Customer Management: Users can create, view, update, and delete customer data, enabling efficient customer data management.
Product Management: Products can be added, viewed, updated, and deleted, providing an effective way to manage the FMCG product catalog.
Order Processing: Users can create orders by associating customers with products, allowing for the management of customer orders.
API Documentation: The API is well-documented using Swagger UI, enabling easy understanding and testing of the endpoints.
Error Handling: The API handles errors gracefully, providing meaningful error responses for various scenarios.





****


To run the code, first, install all the dependencies by using the "npm install" command in your terminal or command prompt. Once the dependencies are installed successfully, you can proceed to start the server.

After starting the server, open your web browser and navigate to "http://localhost:4000/api-docs/" to access the Swagger documentation for the API. Swagger UI provides an interactive interface that allows you to explore and test the various API endpoints easily.

By following these steps, you can check and interact with the API using the Swagger documentation, ensuring a smooth development and testing process for the FMCG App backend.
