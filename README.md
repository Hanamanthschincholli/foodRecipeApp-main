📖 About the Food Recipe App

This project is a backend application built with Node.js, Express.js, and MongoDB.
It’s designed to support a food recipe sharing platform, where users can register/login and manage recipes.

1. Server Setup (server.js)

Starts the backend server.

Configures middlewares (JSON parsing, CORS, authentication).

Connects to the database.

Registers routes for users and recipes.

2. Database Connection (config/connectionDb.js)

Uses Mongoose to connect the app with a MongoDB database.

3. Data Models (models/)

User model (user.js)

Defines user schema (username, email, password, etc.).

Handles authentication-related data.

Recipe model (recipe.js)

Defines recipe schema (title, description, ingredients, instructions, etc.).

Links recipes to a user (creator).

4. Controllers (controller/)

User controller (user.js)

Handles user registration, login, authentication with JWT.

Recipe controller (recipe.js)

Manages CRUD operations for recipes (create, read, update, delete).

5. Middleware (middleware/auth.js)

Protects routes with JWT authentication.

Ensures only logged-in users can access certain endpoints.

6. Environment Config (.env)

Stores sensitive data like MONGO_URI and JWT_SECRET.

🚀 What the App Can Do

User Authentication

Register new users.

Login users and issue JWT tokens.

Recipe Management

Add new recipes.

View all recipes.

Edit/update existing recipes.

Delete recipes.

Database Integration

Stores users and recipes in MongoDB.

Secure Authentication

Uses JWT for secure user sessions.

Uses bcrypt for password hashing.

📂 Why This File Is Useful

This project can be used as:

A starter backend for recipe-sharing apps.

A learning project for Node.js + Express + MongoDB + JWT authentication.

A template for any CRUD-based app with authentication.
