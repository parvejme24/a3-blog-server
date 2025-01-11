<!-- # Blog Server
Live link: https://a3-blog-server.vercel.app/

A blog application backend that supports user authentication, blog management, and user blocking functionality. This project is built with Node.js, Express, MongoDB (via Mongoose), and TypeScript.

## Features

- **User Authentication**: Users can register, login, and manage their sessions.
- **Role-Based Access Control**: Users can have different roles (`admin`, `user`) with varying access to the application.
- **Blog Management**: Admin and users can create, update, delete, and view blogs.
- **User Management**: Admin can block users.

## Requirements

- Node.js (>=16.x)
- MongoDB instance (local or cloud)

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/parvejme24/a3-blog-server.git

  ```bash
      cd a3-blog-server -->

# Blog Server 🚀

**Live Link**: [https://a3-blog-server.vercel.app/](https://a3-blog-server.vercel.app/)

A backend for a blog application that supports user authentication, blog management, and user blocking functionality. This project is built with **Node.js**, **Express**, **MongoDB** (via Mongoose), and **TypeScript**.

---

## ✨ Features

- **User Authentication**:  
  Users can register, log in, and manage their sessions.
- **Role-Based Access Control**:  
  Users have different roles (`admin`, `user`) with varying access levels.
- **Blog Management**:  
  Admins and users can create, update, delete, and view blogs.
- **User Management**:  
  Admins can block users.

---

## 🛠️ Requirements

- **Node.js** (>=16.x)
- **MongoDB** instance (local or cloud)

---

## 🚀 Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/parvejme24/a3-blog-server.git
   ```

2. Navigate to the project directory:

   ```bash
   cd a3-blog-server
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Create a `.env` file in the root directory and add the following environment variables:

   ```env
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   ```

5. Start the development server:

   ```bash
   npm run dev
   ```

---

## 📚 Available Scripts

- **`npm run dev`**: Start the server in development mode.
- **`npm run build`**: Build the project for production.
- **`npm start`**: Start the server in production mode.

---

## 🔐 Environment Variables

| Variable     | Description                   |
| ------------ | ----------------------------- |
| `PORT`       | Port on which the server runs |
| `MONGO_URI`  | MongoDB connection string     |
| `JWT_SECRET` | Secret key for JWT token      |

---

## 🏗️ Project Structure

```bash
├── src
│   ├── controllers
│   ├── models
│   ├── routes
│   ├── middlewares
│   ├── utils
│   └── index.ts
├── .env
├── .gitignore
├── package.json
└── tsconfig.json
```

---

## 📄 API Endpoints

### Auth Routes

| Method | Endpoint           | Description         |
| ------ | ------------------ | ------------------- |
| POST   | /api/auth/register | Register a new user |
| POST   | /api/auth/login    | Login a user        |

### Blog Routes

| Method | Endpoint       | Description             |
| ------ | -------------- | ----------------------- |
| GET    | /api/blogs     | Get all blogs           |
| POST   | /api/blogs     | Create a new blog       |
| PUT    | /api/blogs/:id | Update an existing blog |
| DELETE | /api/blogs/:id | Delete a blog           |

### User Routes

| Method | Endpoint             | Description   |
| ------ | -------------------- | ------------- |
| GET    | /api/users           | Get all users |
| PATCH  | /api/users/:id/block | Block a user  |

---

## 🤝 Contributions

Contributions are welcome! Please fork the repository and submit a pull request.

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 💬 Contact

If you have any questions, feel free to reach out:

- **GitHub**: [parvejme24](https://github.com/parvejme24)
- **Email**: parvej@example.com
