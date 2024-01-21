# E-Wallet-Springboot-Microservices-

A comprehensive e-wallet system that enables users to effortlessly transfer amounts, view their balance, recent transactions, and manage account settings. Developed with a microservices architecture and integrated with modern technologies ensuring responsive and secure user interactions.

<img width="803" alt="E-wallet" src="https://github.com/ritesh-works/E-Wallet-Springboot-Microservices-/assets/116880840/8fafe203-837e-4a74-8fc6-28993fb95e2c">

🚀 Features
P2P Transfers: Allow users to send money to other registered users.
Account Management: Fetch balance, view recent transactions, and edit account settings.
Email Notifications: Automated emails upon every transaction event.
Admin Functionalities: Endpoints for admins to fetch user details.
🛠️ Microservices
User Service: Handle user creation, updates, and queries.
Transaction Service: Oversee transaction initiation and processing.
Notification Service: Administer transactional email notifications.
Wallet Service: Manage user wallet balances and updates.
Note: All services are interconnected efficiently using Kafka.

🔧 Technologies
Spring Boot: Backend microservices framework.
Kafka: Real-time data streaming for inter-service communication.
OAuth: Authentication and authorization.
Spring Security: Secure the endpoints.
JPA: Data management and persistence.
Databases: Independent databases for each microservice.
📌 Controller Insights
Transaction Controller (TxnController)
🔗 Endpoint: /txn
Method: POST
Description: Initiate a P2P transaction.
Parameters: receiver, purpose, amount.
User Controller (UserController)
🔗 Endpoint: /user

Method: POST
Description: Register a new user.
🔗 Endpoint: /user

Method: GET
Description: Fetch authenticated user details.
🔗 Endpoint: /admin/all/users

Method: GET
Description: Get details of all registered users (admin only).
🔗 Endpoint: /admin/user/{userId}

Method: GET
Description: Retrieve specific user details using their ID (admin only).
📥 Setup & Installation
Clone: Download the repository.
Databases: Configure individual databases for each service.
Environment: Update application.properties with relevant credentials.
Kafka: Ensure the Kafka server is operational.
Run: Build and initiate each microservice using Spring Boot.
🤝 Contributions

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.
