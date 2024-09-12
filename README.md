# User Management Service

Simple user management service built with Node.js, Express, MongoDB, and JWT for authentication for a versatile learning platform. It features user registration, login, and profile management, with JWT-based authentication. The MongoDB database is used for scalable and dynamic data management.

## Features

- User registration
- User login with JWT authentication
- User profile management
- MongoDB for storage
- Middleware for security and rate limiting

## Prerequisites

Make sure you have the following installed:
- [Node.js](https://nodejs.org/en/download/) (v14+)
- [MongoDB](https://www.mongodb.com/)

## Setup

1. **Clone the Project**

```bash
git clone https://github.com/tris02/learning_platform_server_arch.git
cd user-management-service
```

2. **Install dependencies**

```bash
npm install
```

3. **Environment variables**

Create a .env file in the root directory and set the following variables:

```bash
MONGO_URI=mongodb://your_mongo_user:your_password@your_mongo_host:27017
JWT_SECRET=your_jwt_secret
PORT=3000
```

4. **Run the server**

```bash
npm start
```

The server will run on http://localhost:3000.

## Project Structure

```
user-management-service/
├── node_modules/
├── src/
│   ├── config/
│   │   └── database.js
│   ├── controllers/
│   │   └── userController.js
│   ├── middlewares/
│   │   └── authMiddleware.js
│   ├── models/
│   │   └── userModel.js
│   ├── routes/
│   │   └── userRoutes.js
│   └── index.js
├── .env
├── package-lock.json
├── package.json
├── README.md
└── .gitignore
```